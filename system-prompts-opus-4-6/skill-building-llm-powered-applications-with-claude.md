<!--
name: 'Skill: Building LLM-powered applications with Claude'
description: >-
  Guides Claude in building LLM-powered applications using the Anthropic SDK,
  covering language detection, API surface selection (Claude API vs Managed
  Agents), model defaults, thinking/effort configuration, and language-specific
  documentation reading
ccVersion: 2.1.185
-->
# Building LLM-Powered Applications with Claude

Choose the right surface, detect the project language, then read the relevant language-specific documentation.

## Before You Start

Scan the target file (or, if none, the prompt and project) for non-Anthropic provider markers — `import openai`, `from openai`, `langchain_openai`, `OpenAI(`, `gpt-4`, `gpt-5`, file names like `agent-openai.py` or `*-generic.py`, or any instruction to keep the code provider-neutral. If you find any, stop and tell the user this skill produces Claude/Anthropic SDK code; ask whether to switch the file to Claude or write a non-Claude implementation. Do not put Anthropic SDK calls into a non-Anthropic file.

## Output Requirement

When asked to add, modify, or implement a Claude feature, call Claude through one of:

1. **The official Anthropic SDK** for the project's language (`anthropic`, `@anthropic-ai/sdk`, `com.anthropic.*`, etc.). Default whenever a supported SDK exists.
2. **Raw HTTP** (`curl`, `requests`, `fetch`, `httpx`, etc.) — only when the user explicitly asks for cURL/REST/raw HTTP, the project is a shell/cURL project, or the language has no official SDK.

Don't mix the two, and don't fall back to OpenAI-compatible shims.

Don't guess SDK usage. Function names, class names, namespaces, method signatures, and import paths must come from explicit documentation — the `{lang}/` files in this skill, or the official SDK repos/docs in `shared/live-sources.md`. If the binding you need isn't documented in the skill files, WebFetch the relevant SDK repo from `shared/live-sources.md` before writing code. Do not infer Ruby/Java/Go/PHP/C# APIs from cURL shapes or another language's SDK.

If WebFetch or repository access fails (network restricted, timeouts, clone blocked): do not keep retrying — write code from the patterns and namespace/package tables in the `{lang}/` file, run the compiler or interpreter on it, and iterate on the error output.

## Defaults

Unless the user requests otherwise: use {{OPUS_NAME}} — model string `{{OPUS_ID}}`. Default to adaptive thinking (`thinking: {type: "adaptive"}`) for anything non-trivial. Default to streaming for long input/output or high `max_tokens` (avoids request timeouts) — use `.get_final_message()` / `.finalMessage()` if you don't need per-event handling.

## API Drift — Your Training Prior May Be Stale

Several common Claude API shapes changed in 2025–2026. Verify against the `{lang}/` files in this skill before writing:

| Area | Stale prior | Current API |
|---|---|---|
| Extended thinking | `thinking: {type: "enabled", budget_tokens: N}` | On Claude 4.6+ models: `thinking: {type: "adaptive"}`. `budget_tokens` is deprecated on Opus 4.6 / Sonnet 4.6 and rejected with a 400 on Fable 5 / Opus 4.8 / 4.7. Pre-4.6 models still use `budget_tokens`. |
| Web search / web fetch tool type | `web_search_20250305`, `web_fetch_20250910` | `web_search_20260209`, `web_fetch_20260209` (dynamic filtering) on Opus 4.8/4.7/4.6 and Sonnet 4.6. Older models keep the basic variants; on Vertex AI only basic `web_search_20250305` is available (web fetch is not on Vertex). |
| PHP parameter names | snake_case wire names as named args (`max_tokens`) | Top-level named args are camelCase (`maxTokens`). Nested array keys vary by feature — copy the exact key from the documented example; do not bulk-convert. |

The `{lang}/` files in this skill are authoritative over recalled patterns.

---

## Subcommands

If the User Request at the bottom is a bare subcommand string (no prose), search every **Subcommands** table in this document — including any in appended sections — and follow the matching Action column. This lets users invoke flows via `/claude-api <subcommand>`. If no table matches, treat the request as normal prose.

| Subcommand | Action |
|---|---|
| `migrate` | Migrate existing Claude API code to a newer model. Read `shared/model-migration.md` and follow it in order: Step 0 (confirm scope — ask which files/directories before any edit), Step 1 (classify each file), then the per-target breaking-changes section. Execute it, don't summarize. If the user didn't name a target model, ask which model to migrate to in the same turn as the scope question. |

---

## Language Detection

Before reading code examples, determine the language:

1. **Infer from project files:**

   - `*.py`, `requirements.txt`, `pyproject.toml`, `setup.py`, `Pipfile` → **Python** — read from `python/`
   - `*.ts`, `*.tsx`, `package.json`, `tsconfig.json` → **TypeScript** — read from `typescript/`
   - `*.js`, `*.jsx` (no `.ts` present) → **TypeScript** — JS uses the same SDK, read from `typescript/`
   - `*.java`, `pom.xml`, `build.gradle` → **Java** — read from `java/`
   - `*.kt`, `*.kts`, `build.gradle.kts` → **Java** — Kotlin uses the Java SDK, read from `java/`
   - `*.scala`, `build.sbt` → **Java** — Scala uses the Java SDK, read from `java/`
   - `*.go`, `go.mod` → **Go** — read from `go/`
   - `*.rb`, `Gemfile` → **Ruby** — read from `ruby/`
   - `*.cs`, `*.csproj` → **C#** — read from `csharp/`
   - `*.php`, `composer.json` → **PHP** — read from `php/`

2. **Multiple languages detected:** check which the user's current file or question relates to; if still ambiguous, ask which language they're using for the Claude API integration.

3. **Can't infer** (empty project, no source, unsupported language): use AskUserQuestion with options Python, TypeScript, Java, Go, Ruby, cURL/raw HTTP, C#, PHP. If AskUserQuestion is unavailable, default to Python and say so.

4. **Unsupported language** (Rust, Swift, C++, Elixir, etc.): suggest cURL/raw HTTP from `curl/`, note community SDKs may exist, offer Python or TypeScript as reference.

5. **User wants cURL/raw HTTP:** read from `curl/`.

### Language-Specific Feature Support

| Language   | Tool Runner | Managed Agents | Notes                                 |
| ---------- | ----------- | -------------- | ------------------------------------- |
| Python     | Yes (beta)  | Yes (beta)     | Full support — `@beta_tool` decorator |
| TypeScript | Yes (beta)  | Yes (beta)     | Full support — `betaZodTool` + Zod    |
| Java       | Yes (beta)  | Yes (beta)     | Beta tool use with annotated classes  |
| Go         | Yes (beta)  | Yes (beta)     | `BetaToolRunner` in `toolrunner` pkg  |
| Ruby       | Yes (beta)  | Yes (beta)     | `BaseTool` + `tool_runner` in beta    |
| C#         | Yes (beta)  | Yes (beta)     | `BetaToolRunner` + raw JSON schema    |
| PHP        | Yes (beta)  | Yes (beta)     | `BetaRunnableTool` + `toolRunner()`   |
| cURL       | N/A         | Yes (beta)     | Raw HTTP, no SDK features             |

> **Managed Agents code examples:** read your language's `{lang}/managed-agents/README.md` (or `curl/managed-agents.md`) plus the language-agnostic `shared/managed-agents-*.md` concept files. C# uses `client.Beta.Agents` and related namespaces. **Agents are persistent — create once, reference by ID** (see the Managed Agents section below).

---

## Which Surface Should I Use?

> **Start simple.** Single calls and workflows handle most cases. Reach for agents only when the task genuinely requires open-ended, model-driven exploration.

| Use Case                                        | Tier            | Recommended Surface       | Why                                                          |
| ----------------------------------------------- | --------------- | ------------------------- | ------------------------------------------------------------ |
| Classification, summarization, extraction, Q&A  | Single LLM call | **Claude API**            | One request, one response                                    |
| Batch processing or embeddings                  | Single LLM call | **Claude API**            | Specialized endpoints                                        |
| Multi-step pipelines with code-controlled logic | Workflow        | **Claude API + tool use** | You orchestrate the loop                                     |
| Custom agent with your own tools                | Agent           | **Claude API + tool use** | Maximum flexibility                                          |
| Server-managed stateful agent with workspace    | Agent           | **Managed Agents**        | Anthropic runs the loop and hosts the tool-execution sandbox |
| Persisted, versioned agent configs              | Agent           | **Managed Agents**        | Agents are stored objects; sessions pin to a version         |
| Long-running multi-turn agent with file mounts  | Agent           | **Managed Agents**        | Per-session containers, SSE event stream, Skills + MCP       |

> Use Managed Agents when you want Anthropic to run the agent loop *and* host the container where tools execute (file ops, bash, code execution all run in the per-session workspace). Use Claude API + tool use when you host the compute or run a custom tool runtime — tool runner for automatic looping, or the manual loop for fine-grained control (approval gates, custom logging, conditional execution).

> **Cloud-provider access.** See `shared/platform-availability.md` for per-feature availability on **Claude Platform on AWS**, **Amazon Bedrock**, **Google Vertex AI**, and **Microsoft Foundry**. That table is the single source of truth in this skill; do not infer availability from anywhere else.

### Decision Tree

```
What does your application need?

0. Which provider?
   ├── First-party API or Claude Platform on AWS → continue (full surface available; per-feature exceptions in shared/platform-availability.md).
   └── Amazon Bedrock, Google Vertex AI, or Microsoft Foundry → Claude API (+ tool use for agents); see shared/platform-availability.md for per-feature support.

1. Single LLM call (classification, summarization, extraction, Q&A)
   └── Claude API — one request, one response

2. Want Anthropic to run the agent loop and host a per-session
   container where Claude executes tools (bash, file ops, code)?
   └── Yes → Managed Agents — server-managed sessions, persisted agent configs,
       SSE event stream, Skills + MCP, file mounts.

3. Workflow (multi-step, code-orchestrated, with your own tools)
   └── Claude API with tool use — you control the loop

4. Open-ended agent (model decides its trajectory, your own tools, you host the compute)
   └── Claude API agentic loop (maximum flexibility)
```

### Should I Build an Agent?

Before the agent tier, check all four:

- **Complexity** — multi-step and hard to fully specify in advance?
- **Value** — does the outcome justify higher cost and latency?
- **Viability** — is Claude capable at this task type?
- **Cost of error** — can errors be caught and recovered (tests, review, rollback)?

If any answer is "no", stay at a simpler tier.

---

## Architecture

Everything goes through `POST /v1/messages`. Tools and output constraints are features of this single endpoint, not separate APIs.

**User-defined tools** — you define tools (decorators, Zod schemas, raw JSON); the SDK's tool runner calls the API, executes your functions, and loops until done. For full control, write the loop manually.

**Server-side tools** — Anthropic-hosted. Code execution is fully server-side (declare it in `tools`, Claude runs code automatically). Computer use can be server-hosted or self-hosted.

**Structured outputs** — constrains the response format (`output_config.format`) and/or tool parameter validation (`strict: true`). Use `client.messages.parse()` to validate responses against your schema. The old `output_format` parameter is deprecated; use `output_config: {format: {...}}` on `messages.create()`.

**Supporting endpoints** — Batches (`POST /v1/messages/batches`), Files (`POST /v1/files`), Token Counting (`POST /v1/messages/count_tokens` — see `shared/token-counting.md`), and Models (`GET /v1/models`, `GET /v1/models/{id}` — live capability/context-window discovery).

---

## Current Models (cached: 2026-06-04)

| Model             | Model ID            | Context        | Input $/1M | Output $/1M |
| ----------------- | ------------------- | -------------- | ---------- | ----------- |
| {{FABLE_NAME}}    | `{{FABLE_ID}}`      | 1M             | $10.00     | $50.00      |
| {{MYTHOS_NAME}} (Project Glasswing only) | `{{MYTHOS_ID}}` | 1M | $10.00     | $50.00      |
| Claude Opus 4.8   | `claude-opus-4-8`   | 1M             | $5.00      | $25.00      |
| Claude Opus 4.7   | `claude-opus-4-7`   | 1M             | $5.00      | $25.00      |
| Claude Opus 4.6   | `claude-opus-4-6`   | 1M             | $5.00      | $25.00      |
| Claude Sonnet 4.6 | `claude-sonnet-4-6` | 1M             | $3.00      | $15.00      |
| Claude Haiku 4.5  | `claude-haiku-4-5`  | 200K           | $1.00      | $5.00       |

Default to `{{OPUS_ID}}`. Use a different model only when the user names one ("use sonnet", "use haiku"); cost is the user's call, not yours. Use `{{FABLE_ID}}` ({{FABLE_NAME}}, Anthropic's most capable widely released model — different API behavior, see below) only when the user asks for it by name or for "the most capable model". {{MYTHOS_NAME}} (`{{MYTHOS_ID}}`, Project Glasswing only) has the same capabilities, pricing, and API surface as Fable 5 — everything in the Fable 5 section applies to both. Use the exact ID strings above — they're complete; don't append date suffixes (use `claude-sonnet-4-6`, not `claude-sonnet-4-6-20251114`). For an older model not in the table ("opus 4.5", "sonnet 3.7"), read `shared/models.md` for the exact ID rather than constructing one.

### {{FABLE_NAME}} (`{{FABLE_ID}}`) — key API differences from Opus-tier

1M context (max is the default), 128K max output. See `shared/model-migration.md` → Migrating to {{FABLE_NAME}}.

- **Thinking always on** — omit `thinking` (or send `{type: "adaptive"}`). `{type: "disabled"}` and `{type: "enabled", budget_tokens: N}` both 400. Control depth via `output_config.effort` (`low` through `xhigh`, plus `max`).
- **Raw chain of thought never returned** — regular `thinking` blocks (not `redacted_thinking`); `display: "summarized"` gives a summary, `"omitted"` (default) leaves the field empty. Replay: pass thinking blocks back exactly as received on the same model (empty-text blocks included — the API rejects *modified* blocks, not read ones); a different model drops them silently (before pricing, so unbilled — nothing to strip).
- **Tokenizer** — same as Opus 4.8 (introduced with 4.7); counts roughly unchanged from 4.7/4.8, per-token pricing differs. From 4.6/Sonnet/Haiku/older, re-baseline with `count_tokens`.
- **`refusal` stop reason** — safety classifiers may decline (HTTP 200, `stop_reason: "refusal"`, with a `stop_details` category). Pre-output refusal: empty `content`, unbilled. Mid-stream: partial output billed — discard it. Check `stop_reason` before reading `content`. Recovery is opt-in: when you write `{{FABLE_ID}}` code, include the server-side `fallbacks` parameter by default (`betas: ["server-side-fallback-2026-06-01"]` + `fallbacks: [{"model": "{{OPUS_ID}}"}]`; Claude API and Claude Platform on AWS) — a declined request is re-served by the fallback model in the same call, with credit-style repricing (decline-before-output unbilled; rescue billed at the fallback's rates). Tell the user it's on; drop it only if they decline. Where server-side fallbacks aren't supported (Bedrock, Vertex AI, Microsoft Foundry), the GA SDKs' client-side `BetaRefusalFallbackMiddleware` + `BetaFallbackState` handle retry. Code: the Refusal Fallbacks section of your language's claude-api doc.
- **No assistant prefill** — same as the 4.6+ family.
- **30-day data retention required** — not available under zero data retention; non-conforming orgs get `400 invalid_request_error`.
- **Longer turns, different prompting** — hard tasks can run many minutes (plan timeouts/streaming/progress UX); sweep effort including low/medium for routine work; prompts written for prior models are often too prescriptive. See `shared/model-migration.md` → Migrating to {{FABLE_NAME}} → Behavioral shifts for the recommended prompt snippets.

If a model string looks unfamiliar, it was released after your training cutoff. These are real models.

**Live capability lookup:** the table is cached. When the user asks "what's the context window for X", "does X support vision/thinking/effort", or "which models support Y", query the Models API (`client.models.retrieve(id)` / `client.models.list()`) — see `shared/models.md`.

---

## Thinking & Effort (Quick Reference)

**Fable 5 / Opus 4.8 / 4.7 — adaptive thinking only:** use `thinking: {type: "adaptive"}`. `thinking: {type: "enabled", budget_tokens: N}` returns 400 — adaptive is the only on-mode. On Opus 4.8/4.7, `{type: "disabled"}` and omitting `thinking` both work; on Fable 5, `{type: "disabled"}` 400s — omit the param instead. Sampling parameters (`temperature`, `top_p`, `top_k`) are removed and will 400. Opus 4.8 keeps the same request surface as 4.7 (no new breaking changes) — see `shared/model-migration.md` → Migrating to Opus 4.8 for behavioral re-tuning, and → Migrating to Opus 4.7 for the full breaking-change list from 4.6 or earlier. With `thinking` disabled, Opus 4.8 may write longer reasoning into the visible response — leave adaptive on, or add a final-answer-only instruction (see the migration guide).

**Opus 4.6 — adaptive thinking (recommended):** use `thinking: {type: "adaptive"}`; Claude decides when and how much to think. `budget_tokens` is deprecated on Opus 4.6 and Sonnet 4.6 — don't use it for new code. Adaptive also auto-enables interleaved thinking (no beta header). When the user asks for "extended thinking", a "thinking budget", or `budget_tokens`, use Fable 5 / Opus 4.8/4.7/4.6 with `thinking: {type: "adaptive"}` — the fixed-budget concept is deprecated; don't switch to an older model. *Gradual-migration carve-out:* `budget_tokens` is still functional on Opus 4.6 and Sonnet 4.6 as a transitional escape hatch — see `shared/model-migration.md` → Transitional escape hatch. This carve-out does **not** apply to Fable 5, Opus 4.7 or 4.8 — `budget_tokens` is fully removed there.

**Effort (GA, no beta header):** controls thinking depth and overall token spend via `output_config: {effort: "low"|"medium"|"high"|"max"}` (inside `output_config`, not top-level). Default is `high` (= omitting it). `max` is supported on Fable 5, Opus 4.6+, and Sonnet 4.6 (not Haiku or earlier Sonnets). Opus 4.7 added `"xhigh"` (between `high` and `max`) — best for most coding/agentic use on Fable 5 / 4.7/4.8 and the default in Claude Code; use a minimum of `high` for intelligence-sensitive work. Works on Fable 5, Opus 4.5/4.6/4.7/4.8 and Sonnet 4.6; errors on Sonnet 4.5 / Haiku 4.5. On Fable 5, Opus 4.7/4.8 effort matters more than on any prior Opus — re-tune when migrating, and run long-horizon/agentic tasks at `high`/`xhigh` with the full task spec up front. Lower effort means fewer, more-consolidated tool calls and terser confirmations. Use `max` when correctness matters more than cost; `low` for subagents or simple tasks.

**Thinking display — `"omitted"` by default on Fable 5 / Mythos 5 / Opus 4.8 / 4.7:** `display: "summarized"` returns a readable summary; `"omitted"` (default on all four — a silent change from Opus 4.6 where it was `"summarized"`) streams `thinking` blocks with empty text. If you stream reasoning to users, the default looks like a long pause; set `thinking: {type: "adaptive", display: "summarized"}` explicitly.

**Task Budgets (beta, Fable 5 / Opus 4.7 / 4.8):** `output_config: {task_budget: {type: "tokens", total: N}}` tells the model its token allowance for a full agentic loop — it sees a running countdown and self-moderates (minimum 20,000; beta header `task-budgets-2026-03-13`). Distinct from `max_tokens`, an enforced per-response ceiling the model isn't aware of. See `shared/model-migration.md` → Task Budgets.

**Sonnet 4.6:** supports adaptive thinking; `budget_tokens` deprecated — use adaptive.

**Older models (only if explicitly requested):** for Sonnet 4.5 or another older model, use `thinking: {type: "enabled", budget_tokens: N}` where `budget_tokens` < `max_tokens` (minimum 1024). Don't pick an older model just because the user mentions `budget_tokens`.

---

## Fast Mode (Quick Reference)

**Research preview, Opus 4.8 / 4.7 only** (Opus 4.6 fast mode is deprecated and being removed; after removal, `speed: "fast"` on 4.6 silently falls back to standard speed). Fast mode runs the same model at up to 2.5x higher output tokens per second, at premium pricing. Three things required on every request: use the **beta** messages endpoint (`client.beta.messages.…`), pass the beta flag `fast-mode-2026-02-01`, and set `speed: "fast"` as a top-level request parameter.

```python
client.beta.messages.create(
    model="claude-opus-4-8", max_tokens=4096,
    speed="fast", betas=["fast-mode-2026-02-01"],
    messages=[...],
)
```

| Language | Beta flag | Speed parameter |
|---|---|---|
| Python | `betas=["fast-mode-2026-02-01"]` | `speed="fast"` |
| TypeScript / Ruby | `betas: ["fast-mode-2026-02-01"]` | `speed: "fast"` |
| Go | `[]anthropic.AnthropicBeta{anthropic.AnthropicBetaFastMode2026_02_01}` | `Speed: anthropic.BetaMessageNewParamsSpeedFast` |
| Java | `.addBeta(AnthropicBeta.FAST_MODE_2026_02_01)` | `.speed(MessageCreateParams.Speed.FAST)` |
| C# | `Betas = ["fast-mode-2026-02-01"]` | `Speed = Speed.Fast` (`Anthropic.Models.Beta.Messages`) |
| PHP | `betas: ['fast-mode-2026-02-01']` | `speed: 'fast'` |
| cURL | `anthropic-beta: fast-mode-2026-02-01` header | `"speed": "fast"` in body |

`response.usage.speed` reports which speed was used. Not available with Batch API, Priority Tier, Claude Platform on AWS, or third-party platforms.

---

## Task Budgets (Quick Reference)

**Beta, Fable 5 / Opus 4.8 / 4.7.** Set `task_budget` inside `output_config` on `client.beta.messages.stream(...)` with beta flag `task-budgets-2026-03-13` — use streaming so the large `max_tokens` doesn't hit HTTP timeouts:

```python
with client.beta.messages.stream(
    model="claude-opus-4-8", max_tokens=128000,
    output_config={"effort": "high", "task_budget": {"type": "tokens", "total": 64000}},
    betas=["task-budgets-2026-03-13"],
    messages=[...], tools=[...],
) as stream:
    response = stream.get_final_message()
```

`task_budget` fields: `type` (always `"tokens"`), `total`, and optional `remaining` (defaults to `total`). The budget counts what Claude generates and the tool results it reads this turn — not the full history you resend each request. Only pass `remaining` when you compact or rewrite history between requests and the server can no longer derive prior spend.

---

## Provider Clients (Quick Reference)

When targeting Claude on a third-party platform, use that platform's dedicated client class — not the first-party `Anthropic()` client with a `base_url` override. After construction the client exposes the same `messages.create` / `.stream` surface.

### Amazon Bedrock

Use the **Mantle** client (Messages-API Bedrock endpoint). Bedrock model IDs take an `anthropic.` prefix. Region is required.

| Language | Client |
|---|---|
| Python | `from anthropic import AnthropicBedrockMantle` → `AnthropicBedrockMantle(aws_region="…")` |
| TypeScript | `import { AnthropicBedrockMantle } from "@anthropic-ai/bedrock-sdk"` → `new AnthropicBedrockMantle({ awsRegion: "…" })` |
| Go | `bedrock.NewMantleClient(ctx, bedrock.MantleClientConfig{ AWSRegion: "…" })` |
| Java | `AnthropicOkHttpClient.builder().backend(BedrockMantleBackend.fromEnv()).build()` |
| C# | `new AnthropicBedrockMantleClient(new() { AwsRegion = "…" })` (package `Anthropic.Bedrock`) |
| PHP | `use Anthropic\Bedrock\MantleClient;` → `new MantleClient(awsRegion: '…')` |
| Ruby | `Anthropic::BedrockMantleClient.new(aws_region: "…")` |

`AnthropicBedrock` / `BedrockClient` / `BedrockBackend` (without `Mantle`) are the legacy path — prefer Mantle for new code.

### Microsoft Foundry

| Language | Client |
|---|---|
| Python | `from anthropic import AnthropicFoundry` → `AnthropicFoundry(api_key=…, resource="…")` |
| TypeScript | `import AnthropicFoundry from "@anthropic-ai/foundry-sdk"` → `new AnthropicFoundry({ … })` |
| Java | `AnthropicOkHttpClient.builder().backend(FoundryBackend.fromEnv()).build()` |
| C# | `new AnthropicFoundryClient(new AnthropicFoundryApiKeyCredentials(…))` (package `Anthropic.Foundry`) |
| PHP | `Foundry\Client::withCredentials(…)` |

Go and Ruby have no Foundry client — Ruby's fallback is `Anthropic::Client.new(base_url: "<foundry endpoint>")`.

### Google Cloud Vertex AI

Two required constructor args: GCP `project_id` and `region`. Vertex model IDs take **no prefix** — current-generation models use the bare first-party ID (e.g. `"{{OPUS_ID}}"`); dated-snapshot models use an `@` version separator (e.g. `claude-opus-4-5@20251101`). Auth is GCP ADC; no Anthropic API key.

| Language | Client |
|---|---|
| Python | `from anthropic import AnthropicVertex` → `AnthropicVertex(project_id="…", region="…")` (install `"anthropic[vertex]"`) |
| TypeScript | `import { AnthropicVertex } from "@anthropic-ai/vertex-sdk"` → `new AnthropicVertex({ projectId, region })` |
| Go | `anthropic.NewClient(vertex.WithGoogleAuth(ctx, region, projectID))` |
| Java | `AnthropicOkHttpClient.builder().backend(VertexBackend.builder().region("…").project("…").build()).build()` |
| C# | `new AnthropicClient { Backend = new VertexBackend(projectId, region) }` (package `Anthropic.Vertex`) |
| PHP | `Vertex\Client::fromEnvironment(location: '…', projectId: '…')` — note `location`, not `region` |
| Ruby | `Anthropic::VertexClient.new(region: "…", project_id: "…")` |

---

## Compaction (Quick Reference)

**Beta, Fable 5, Opus 4.8/4.7/4.6 and Sonnet 4.6.** For conversations that may exceed 1M context, enable server-side compaction: the API summarizes earlier context as it nears the trigger threshold (default 150K tokens). Beta header `compact-2026-01-12`.

Append `response.content` (not just the text) back to your messages every turn. Compaction blocks must be preserved — the API uses them to replace compacted history on the next request; appending only the text string silently loses compaction state.

See `{lang}/claude-api/README.md` (Compaction section) for code examples; full docs via WebFetch in `shared/live-sources.md`.

---

## Context Editing (Quick Reference)

**Beta.** Context editing **clears** old tool results or thinking blocks from the conversation before the model sees it; it is **not compaction** (which summarizes). On `client.beta.messages.*` with beta `context-management-2025-06-27`, pass `context_management.edits` with a strategy type:

```python
client.beta.messages.create(
    model="{{OPUS_ID}}", max_tokens=4096,
    betas=["context-management-2025-06-27"],
    context_management={"edits": [{"type": "clear_tool_uses_20250919"}]},
    tools=[...], messages=[...],
)
```

Strategy types: `clear_tool_uses_20250919` (clears old tool results; optional `clear_tool_inputs: true` also clears the tool_use params) and `clear_thinking_20251015` (clears thinking blocks). Do **not** use `compact_20260112` or beta `compact-2026-01-12` — those are the separate compaction feature.

---

## Mid-Conversation System Messages (Quick Reference)

**{{OPUS_NAME}} only; no beta header.** Append `{"role": "system", "content": "…"}` to the `messages` array (not the top-level `system` field) to add an operator instruction mid-conversation without invalidating the cached prefix. Use the regular `client.messages.create` — there is no beta. A mid-conversation system message must follow a `user` message (or an `assistant` message ending in server-tool use), and must be either the last entry in `messages` or be followed by an `assistant` turn — it cannot be `messages[0]`. Availability: `shared/platform-availability.md`. See `shared/prompt-caching.md` § Mid-conversation system messages.

---

## Prompt Caching (Quick Reference)

**Prefix match.** Any byte change in the prefix invalidates everything after it. Render order is `tools` → `system` → `messages`. Keep stable content first (frozen system prompt, deterministic tool list); put volatile content (timestamps, per-request IDs, varying questions) after the last `cache_control` breakpoint.

**Mid-conversation operator instructions** ({{OPUS_NAME}} only; no beta header): append `{"role": "system", ...}` to `messages[]` instead of editing top-level `system`. Preserves the cached prefix and is the prompt-injection-safe operator channel. See `shared/prompt-caching.md` § Mid-conversation system messages.

**Top-level auto-caching** (`cache_control: {type: "ephemeral"}` on `messages.create()`) is simplest when you don't need fine-grained placement. Max 4 breakpoints per request. Minimum cacheable prefix is ~1024 tokens — shorter prefixes silently won't cache.

**Verify with `usage.cache_read_input_tokens`** — if it's zero across repeated requests, a silent invalidator is at work (`datetime.now()` in system prompt, unsorted JSON, varying tool set).

For placement patterns, architectural guidance, and the silent-invalidator audit checklist: read `shared/prompt-caching.md`. Language-specific syntax: `{lang}/claude-api/README.md` (Prompt Caching section).

---

## Managed Agents (Beta)

A third surface: server-managed stateful agents with Anthropic-hosted tool execution. Create a persisted, versioned Agent config (`POST /v1/agents`), then start Sessions that reference it. Each session provisions a container as the agent's workspace — bash, file ops, and code execution run there; the agent loop runs on Anthropic's orchestration layer and acts on the container via tools. The session streams events; you send messages and tool results back.

Availability: `shared/platform-availability.md`. For agents on Bedrock / Vertex / Foundry (where Managed Agents is unsupported), use Claude API + tool use.

**Mandatory flow:** Agent (once) → Session (every run). `model`/`system`/`tools` live on the agent, never the session. See `shared/managed-agents-overview.md` for the full reading guide, beta headers, and pitfalls.

**Beta headers:** `managed-agents-2026-04-01` — the SDK sets this automatically for all `client.beta.{agents,environments,sessions,vaults,memory_stores,deployments,deployment_runs}.*` calls. Skills API uses `skills-2025-10-02` and Files API uses `files-api-2025-04-14`, passed automatically except for `/v1/skills` and `/v1/files`.

**Subcommands** — invoke with `/claude-api <subcommand>`:

| Subcommand | Action |
|---|---|
| `managed-agents-onboard` | Walk the user through setting up a Managed Agent from scratch. Read `shared/managed-agents-onboarding.md` and run its interview script: describe → configure the agent → environment → session — defaults and inline suggestions do the work, with a viability gate (job vs tools/credentials/data) before any code is emitted. Do not summarize — run the interview. |

**Reading guide:** start with `shared/managed-agents-overview.md`, then the topical `shared/managed-agents-*.md` files (core, environments, tools, events, outcomes, multiagent, webhooks, memory, scheduled-deployments, client-patterns, onboarding, api-reference). For Python, TypeScript, Go, Ruby, PHP, and Java read `{lang}/managed-agents/README.md`; for cURL read `curl/managed-agents.md`. **Agents are persistent — create once, reference by ID.** Store the agent ID returned by `agents.create` and pass it to every subsequent `sessions.create`; don't call `agents.create` in the request path. The Anthropic CLI (`ant`) creates agents and environments from version-controlled YAML — see `shared/anthropic-cli.md`. If a binding isn't shown in the README, WebFetch the relevant entry from `shared/live-sources.md`. C# uses `client.Beta.Agents`.

**When the user wants to set up a Managed Agent from scratch** ("how do I get started", "walk me through creating one", "set up a new agent"): read `shared/managed-agents-onboarding.md` and run its interview — same flow as `managed-agents-onboard`.

**When the user asks "how do I write the client code for X":** read `shared/managed-agents-client-patterns.md` — lossless stream reconnect, `processed_at` queued/processed gate, interrupt, `tool_confirmation` round-trip, the idle/terminated break gate, post-idle status race, stream-first ordering, file-mount gotchas, keeping credentials host-side via custom tools, etc.

**When the user wants the agent to run on a schedule** (cron, "every night", "weekly report"): read `shared/managed-agents-scheduled-deployments.md` — deployments fire sessions autonomously on a cron cadence, with per-firing run records and lifecycle controls (pause/unpause/archive).

---

## Server Tools (Quick Reference)

Server-side tools run on Anthropic's infrastructure — no client-side execution loop. Declare in `tools`; results arrive as content blocks in the same response. No beta header unless noted. Use the latest type variant your model supports. The `_20260209` web search / web fetch variants (dynamic filtering) require Opus 4.8/4.7/4.6 or Sonnet 4.6.

| Tool | `type` | `name` | Key optional params | Result block type |
|---|---|---|---|---|
| Web search | `web_search_20260209` | `web_search` | `max_uses`, `allowed_domains`/`blocked_domains`, `user_location` | `web_search_tool_result` → `.content` is a list of `web_search_result` |
| Web fetch | `web_fetch_20260209` | `web_fetch` | `max_uses`, `allowed_domains`/`blocked_domains`, `citations`, `max_content_tokens` | `web_fetch_tool_result` → `.content` is a `web_fetch_result` with a `document` block |
| Code execution | `code_execution_20250825` | `code_execution` | none | `bash_code_execution_tool_result` → `.content.stdout` / `.stderr` / `.return_code` |
| Tool search (regex) | `tool_search_tool_regex_20251119` | `tool_search_tool_regex` | mark other tools `defer_loading: true` | `tool_search_tool_result` |
| Tool search (BM25) | `tool_search_tool_bm25_20251119` | `tool_search_tool_bm25` | mark other tools `defer_loading: true` | `tool_search_tool_result` |

`web_search_20260209` / `web_fetch_20260209` have built-in dynamic filtering — code execution runs under the hood, so do **not** separately declare `code_execution` in `tools`. For models older than Opus 4.6 / Sonnet 4.6, use basic variants `web_search_20250305` / `web_fetch_20250910`; on Vertex AI only basic `web_search_20250305` is available. `code_execution_20260120` (REPL persistence + programmatic tool calling) runs on Opus 4.5+ / Sonnet 4.5+. **Go SDK only**: `code_execution_20250825` lives under `client.Beta.Messages.New` with the `code-execution-2025-08-25` beta. Provider availability varies by tool — see `shared/platform-availability.md`. See `shared/tool-use-concepts.md` for `pause_turn` handling.

## Document & File Input (Quick Reference)

**PDF (base64, no beta):** `{"type": "document", "source": {"type": "base64", "media_type": "application/pdf", "data": <b64 string>}}` in user content, placed before the text block. Base64 string must have no newlines. Limits: 32 MB request, 600 pages (100 for 200k-context models).

**Files API (beta `files-api-2025-04-14`):** upload via `client.beta.files.upload(...)` → response `id` is the `file_id`. Reference it as `{"type": "document", "source": {"type": "file", "file_id": "..."}}` for PDF/text, or `{"type": "image", ...}` for images — the content-block type must match the file's MIME type. The beta header is required on both the upload and the `messages.create` that references the file. Availability: `shared/platform-availability.md`.

**Citations (no beta):** set `citations: {enabled: true}` on each `document` content block (all or none). Response splits into multiple `text` blocks; cited blocks carry a `citations` array with `cited_text`, `document_index`, `document_title`, and a location by `type`: `char_location` (`start_char_index`/`end_char_index`) for plain text, `page_location` (`start_page_number`/`end_page_number`, 1-indexed) for PDF, `content_block_location` for custom content. Incompatible with `output_config.format`.

## Tool Use Patterns (Quick Reference)

**Strict tool use (no beta):** set `strict: true` as a top-level field on the tool definition (alongside `name`/`description`/`input_schema`), not on `tool_choice`. Schema must have `additionalProperties: false` + `required`. Guarantees `tool_use.input` validates exactly.

**Parallel tool use (default on):** one assistant message may contain multiple `tool_use` blocks. Execute them concurrently, then return all `tool_result` blocks in a single user message. For a failed tool, return `tool_result` with `is_error: true` — don't drop it.

**Tool Runner (SDK beta helper):** drives the tool-call loop for you via `client.beta.messages.*`. Python: `@beta_tool` decorator + `client.beta.messages.tool_runner(...)` → `runner.until_done()`. TypeScript: `betaZodTool({...})` + `client.beta.messages.toolRunner(...)` → `await runner`. Go: `toolrunner.NewBetaToolFromJSONSchema(...)` + `client.Beta.Messages.NewToolRunner(...)`. Ruby: `Anthropic::BaseTool` subclass + `client.beta.messages.tool_runner(...)`. PHP: `BetaRunnableTool` + `->toolRunner(...)`. C#: `BetaToolRunner` via `client.Beta.Messages.ToolRunner(...)`.

**Programmatic tool calling (no beta header):** Claude calls your custom tool from inside code execution. Add `{"type": "code_execution_20260120", "name": "code_execution"}` and set `"allowed_callers": ["code_execution_20260120"]` on your custom tool. Opus 4.5+ / Sonnet 4.5+. Not compatible with `strict: true`, `disable_parallel_tool_use`, forced `tool_choice`, or MCP tools.

## Other API Surfaces (Quick Reference)

**Message Batches (no beta; availability: `shared/platform-availability.md`):** `client.messages.batches.create(requests=[{custom_id, params}, ...])` → poll `client.messages.batches.retrieve(id).processing_status` until `"ended"` → stream `client.messages.batches.results(id)`. Each result has `.custom_id` + `.result.type` (`succeeded`/`errored`/`canceled`/`expired`); on success read `.result.message.content`. Results arrive in any order — key by `custom_id`, never by position.

**Models API (no beta; availability: `shared/platform-availability.md`):** `client.models.list()` and `client.models.retrieve("{{OPUS_ID}}")`. Each model object has `id`, `display_name`, `created_at`, and — since Mar 2026 — `max_input_tokens`, `max_tokens`, and `capabilities`. There is no `context_window` field.

**Stop details (GA, Opus 4.7+):** `response.stop_details` is populated only when `stop_reason == "refusal"` (fields: `type: "refusal"`, `category: "cyber"|"bio"|null`, `explanation`). It is `null` for every other `stop_reason` — guard before reading.

**Client config (no beta):** `timeout` default 10 min; units differ by SDK — Python/Ruby: seconds; TypeScript: milliseconds; Go `option.WithRequestTimeout(time.Duration)`; Java `Duration`; C# `TimeSpan`. `max_retries`/`maxRetries` default 2. Timeouts are retried — wall-clock can reach `timeout × (max_retries+1)`.

## Workload Identity Federation (Quick Reference)

**GA, no beta header.** Construct the normal zero-arg client; the SDK auto-detects WIF when all of `ANTHROPIC_FEDERATION_RULE_ID`, `ANTHROPIC_ORGANIZATION_ID`, `ANTHROPIC_SERVICE_ACCOUNT_ID`, and `ANTHROPIC_IDENTITY_TOKEN_FILE` (or `ANTHROPIC_IDENTITY_TOKEN`) are set, exchanges the JWT at `/v1/oauth/token`, and auto-refreshes. `ANTHROPIC_API_KEY` or `ANTHROPIC_AUTH_TOKEN` (even empty) outrank WIF; a set `ANTHROPIC_PROFILE` also wins — unset all three, don't blank them.

---

## Reading Guide

After detecting the language, read based on what the user needs.

### Quick Task Reference

**Single text classification/summarization/extraction/Q&A:** `{lang}/claude-api/README.md`
**Chat UI or real-time response display:** `{lang}/claude-api/README.md` + `{lang}/claude-api/streaming.md`
**Long-running conversations (may exceed context window):** `{lang}/claude-api/README.md` — Compaction section
**Migrating to a newer model or replacing a retired one:** `shared/model-migration.md`
**Prompt caching / "why is my cache hit rate low":** `shared/prompt-caching.md` + `{lang}/claude-api/README.md` (Prompt Caching section)
**Count tokens in a file / prompt / diff:** `shared/token-counting.md` — use `messages.count_tokens`, never `tiktoken`
**Function calling / tool use / agents:** `{lang}/claude-api/README.md` + `shared/tool-use-concepts.md` + `{lang}/claude-api/tool-use.md`
**Agent design (tool surface, context management, caching strategy):** `shared/agent-design.md`
**Batch processing (non-latency-sensitive):** `{lang}/claude-api/README.md` + `{lang}/claude-api/batches.md`
**File uploads across multiple requests:** `{lang}/claude-api/README.md` + `{lang}/claude-api/files-api.md`
**Managed Agents:** `shared/managed-agents-overview.md` + the other `shared/managed-agents-*.md` files, plus `{lang}/managed-agents/README.md` (or `curl/managed-agents.md`). See the Managed Agents section above for the persistence and reading details.

### Claude API (Full File Reference)

Read the language-specific folder (`{language}/claude-api/`):

1. **`{language}/claude-api/README.md`** — read first. Installation, quick start, common patterns, error handling.
2. **`shared/tool-use-concepts.md`** — function calling, code execution, memory, structured outputs (concepts).
3. **`shared/agent-design.md`** — designing an agent: bash vs. dedicated tools, programmatic tool calling, tool search/skills, context editing vs. compaction vs. memory, caching principles.
4. **`{language}/claude-api/tool-use.md`** — language-specific tool use examples (tool runner, manual loop, code execution, memory, structured outputs).
5. **`{language}/claude-api/streaming.md`** — chat UIs and incremental display.
6. **`{language}/claude-api/batches.md`** — many offline requests; runs asynchronously at 50% cost.
7. **`{language}/claude-api/files-api.md`** — sending the same file across multiple requests.
8. **`shared/prompt-caching.md`** — adding or optimizing caching; prefix stability, breakpoint placement, silent-invalidator anti-patterns.
9. **`shared/error-codes.md`** — debugging HTTP errors / error handling.
10. **`shared/model-migration.md`** — upgrading models, replacing retired models, translating `budget_tokens`/prefill patterns.
11. **`shared/live-sources.md`** — WebFetch URLs for the latest official docs.

> For Java, Go, Ruby, C#, PHP, and cURL — a single file each covers the basics; read that plus `shared/tool-use-concepts.md` and `shared/error-codes.md` as needed.

---

## When to Use WebFetch

Use WebFetch for the latest documentation when the user asks for "latest"/"current" info, cached data seems incorrect, or they ask about features not covered here. Live URLs are in `shared/live-sources.md`.

## Common Pitfalls

- Don't truncate inputs when passing files or content. If content exceeds the context window, notify the user and discuss options (chunking, summarization) rather than silently truncating.
- **Fable 5 / Opus 4.8 / 4.7 thinking:** adaptive only. `thinking: {type: "enabled", budget_tokens: N}` returns 400 — `budget_tokens` is fully removed (with `temperature`, `top_p`, `top_k`). Use `thinking: {type: "adaptive"}`. 4.8 inherits this surface from 4.7 with no new breaking changes; Fable 5 adds one — an explicit `{type: "disabled"}` 400s (accepted on 4.7/4.8), so omit the param instead.
- **Opus 4.6 / Sonnet 4.6 thinking:** use `thinking: {type: "adaptive"}` — don't use `budget_tokens` for new code (deprecated on both; transitional escape hatch in `shared/model-migration.md` doesn't apply to 4.7/4.8). For older models, `budget_tokens` < `max_tokens` (minimum 1024), or it errors.
- **Prefill removed (Fable 5 + 4.6/4.7/4.8):** last-assistant-turn prefills return 400 on Fable 5, Opus 4.6/4.7/4.8 and Sonnet 4.6. Use structured outputs (`output_config.format`) or system-prompt instructions to control format.
- **Fable 5 `refusal` stop reason:** check `stop_reason` before reading `response.content[0]` — pre-output refusal has empty `content`; mid-stream refusal bills partial output (discard it). Fallbacks are opt-in — new `{{FABLE_ID}}` code should include the server-side `fallbacks` parameter by default; see the {{FABLE_NAME}} section above.
- **Confirm migration scope before editing:** when a user asks to migrate without a named file/directory/list, ask which scope first. Don't edit until confirmed. Proceed without asking only when an exact file/directory/list is named. See `shared/model-migration.md` Step 0.
- **`max_tokens` defaults:** don't lowball it — hitting the cap truncates mid-thought. Non-streaming: default `~16000`. Streaming: default `~64000`. Go lower only with a reason: classification (`~256`), cost caps, deliberately short outputs, or `max_tokens: 0` for cache pre-warming (see `shared/prompt-caching.md` → Pre-warming).
- **128K output tokens:** Fable 5, Opus 4.6/4.7/4.8 support up to 128K `max_tokens`, but the SDKs require streaming for values that large. Use `.stream()` with `.get_final_message()` / `.finalMessage()`.
- **Tool call JSON parsing (Fable 5 + 4.6/4.7/4.8):** may produce different JSON string escaping in tool-call `input`. Always parse with `json.loads()` / `JSON.parse()` — never raw string matching.
- **Structured outputs (all models):** use `output_config: {format: {...}}`, not the deprecated `output_format` parameter.
- **Don't reimplement SDK functionality:** use `stream.finalMessage()` instead of wrapping `.on()` events in `new Promise()`; use typed exception classes (`Anthropic.RateLimitError`, etc.) instead of string-matching errors; use SDK types instead of redefining interfaces.
- **Error handling — catch a chain, not one broad class.** `NotFoundError` → `RateLimitError` → `APIStatusError` → `APIConnectionError`. Per-language class names: `shared/error-codes.md`.
- **Don't research SDK types — write first.** Write the code file and let the compiler's error point you to the right name. A quick `strings` / `jar tf` / `javap` against the installed SDK is acceptable (seconds), but don't escalate beyond that.
- **Bash and text editor tools are Anthropic-defined, schema-less.** Declare `{"type": "bash_20250124", "name": "bash"}` / `{"type": "text_editor_20250728", "name": "str_replace_based_edit_tool"}` — no `input_schema`.
- **Advisor tool model pairing.** The advisor tool's `model` must be at least as capable as the request's top-level `model`. An invalid pair returns 400. Pairing table in `shared/tool-use-concepts.md` § Advisor. Availability: `shared/platform-availability.md`.
- **Agent Skills ≠ Managed Agents.** To have Claude generate a `.pptx`/`.xlsx`/etc. via Agent Skills, call `client.beta.messages.create` with `container={"skills": [...]}`, the `code_execution_20250825` tool, and both `code-execution-2025-08-25` + `skills-2025-10-02` betas. Do not use `client.beta.agents` / `sessions` / `environments` — those are Managed Agents.
- **MCP connector needs both halves.** `mcp_servers=[{type:"url", url, name}]` alone is rejected — also add `tools=[{type:"mcp_toolset", mcp_server_name:<same name>}]` with beta `mcp-client-2025-11-20`. Availability: `shared/platform-availability.md`.
- **Context editing ≠ compaction.** Context editing *clears* tool results and thinking blocks; compaction *summarizes* history. For context editing, use `context_management.edits` with type `clear_tool_uses_20250919` or `clear_thinking_20251015` on `client.beta.messages.*` with beta `context-management-2025-06-27` — not the `compact_20260112` type or `compact-2026-01-12` beta.
- **`inference_geo` is a direct top-level request parameter** — `client.messages.create(..., inference_geo="us")`. Do not put it in `extra_body`. Supported on Opus 4.6 / Sonnet 4.6 and later.
- **Fine-grained tool streaming is not a beta feature.** Set `eager_input_streaming: true` on the tool definition and call the regular `client.messages.stream(...)`. No beta header.
- **Cache diagnostics is beta.** Use `client.beta.messages.*` with beta `cache-diagnosis-2026-04-07`. Pass `diagnostics: {previous_message_id: null}` on the first turn and `diagnostics: {previous_message_id: <previous response id>}` on subsequent turns.
- **Memory tool type is `memory_20250818`.** Declare `{"type": "memory_20250818", "name": "memory"}`. Go uses the beta-namespace type on `client.Beta.Messages.New`.
- **Use a model the feature actually supports.** Fast mode is Opus 4.8 / 4.7 only; task budgets are Fable 5 / Opus 4.8 / 4.7 only; the advisor tool requires a valid executor↔advisor pair. If the user's prompt names an unsupported model, substitute a supported one and note it.
- **Bedrock / Foundry: use the platform client class.** For Bedrock use the `…BedrockMantle…` client with `anthropic.`-prefixed model IDs; `AnthropicBedrock`/`BedrockBackend` without `Mantle` is the legacy path. For Foundry use `AnthropicFoundry` / `FoundryBackend` / `AnthropicFoundryClient`.
- **Don't define custom types for SDK data structures.** Use `Anthropic.MessageParam`, `Anthropic.Tool`, `Anthropic.ToolUseBlock`, `Anthropic.Message`, etc.
- **Report and document output:** for reports/documents/visualizations, the code execution sandbox has `python-docx`, `python-pptx`, `matplotlib`, `pillow`, and `pypdf` pre-installed. Claude can generate formatted files (DOCX, PDF, charts) and return them via the Files API.
- **Server-tool errors don't raise.** Web search and web fetch errors return HTTP 200 with a result block whose `content` is a single error object (e.g. `{error_code: "max_uses_exceeded"}`). For web search, a success `content` is a *list*; an error `content` is an *object* — branch on that before indexing.
- **Code execution output block type:** `code_execution_20250825` returns `bash_code_execution_tool_result` — not the legacy bare `code_execution_tool_result`.
- **Tool search: never defer everything.** The search tool itself must not have `defer_loading: true`, and at least one tool in `tools` must be non-deferred, or the API returns 400.
- **`strict: true` goes on the tool, not `tool_choice`.**
- **Parallel tool results go in ONE user message.**
- **Citations + structured outputs are incompatible.** Enabling `citations: {enabled: true}` on a document while also setting `output_config.format` returns a 400.
- **Batch results are unordered.** Match by `custom_id`, never by position.
- **Vertex model IDs have no prefix.** Unlike Bedrock's `anthropic.`-prefixed IDs, Vertex takes the bare first-party ID for current-generation models; dated-snapshot models use an `@` separator (e.g. `claude-haiku-4-5@20251001`).
- **`stop_details` is `null` unless `stop_reason == "refusal"`.** Guard before reading `.category`.
- **WIF auth: unset `ANTHROPIC_API_KEY`, `ANTHROPIC_AUTH_TOKEN`, and `ANTHROPIC_PROFILE`.** Even empty values outrank WIF in the SDK's precedence chain. `unset` them, don't blank them.
