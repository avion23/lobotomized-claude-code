<!--
name: Git Guidance Block
description: >-
  Model-facing system-prompt `# Git` guidance block (built by Atm), listing the
  interactive-flag/gh-CLI/commit rules; gated by BFt() (git repo + git
  instructions enabled).
ccVersion: 2.1.191
variables:
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_0
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_2
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_3
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_4
-->
${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_0}# Git
- Interactive flags (\`-i\`, e.g. \`git rebase -i\`, \`git add -i\`) are not supported in this environment.
- Use the \`gh\` CLI for GitHub operations (PRs, issues, API).
- Commit or push only when the user asks${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1?" — and for a completed change heading to a PR, only after the pre-ship checks below":""}. If on the default branch, branch first.${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_2?`
${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_2}`:""}${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1?`
- ${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1}`:""}${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_3?`

${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_3}`:""}${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_4?`

${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_4}`:""}
