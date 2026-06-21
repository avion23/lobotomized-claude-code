<!--
name: 'Data: Managed Agents reference — Go'
description: Managed Agents reference for Go SDK
ccVersion: 2.1.185
-->
# Managed Agents — Go

> **Bindings not shown here:** This README covers the most common managed-agents flows for Go. If you need a class, method, namespace, field, or behavior that isn't shown, WebFetch the Go SDK repo **or the relevant docs page** from \`shared/live-sources.md\` rather than guess. Do not extrapolate from cURL shapes or another language's SDK.

> **Agents are persistent — create once, reference by ID.** Store the agent ID returned by \`agents.New\` and pass it to every subsequent \`sessions.New\`; do not call \`agents.New\` in the request path. The Anthropic CLI is one convenient way to create agents and environments from version-controlled YAML — its URL is in \`shared/live-sources.md\`. The examples below show in-code creation for completeness; in production the create call belongs in setup, not in the request path.

## Installation

\`\`\`bash
go get github.com/anthropics/anthropic-sdk-go
\`\`\`

## Client Initialization

\`\`\`go
import (
    "context"

    "github.com/anthropics/anthropic-sdk-go"
    "github.com/anthropics/anthropic-sdk-go/option"
)

// Default (uses ANTHROPIC_API_KEY env var)
client := anthropic.NewClient()

// Explicit API key
client := anthropic.NewClient(
    option.WithAPIKey("your-api-key"),
)

ctx := context.Background()
\`\`\`

---

## Create an Environment

\`\`\`go
environment, err := client.Beta.Environments.New(ctx, anthropic.BetaEnvironmentNewParams{
    Name: "my-dev-env",
    Config: anthropic.BetaEnvironmentNewParamsConfigUnion{
        OfCloud: &anthropic.BetaCloudConfigParams{
            Networking: anthropic.BetaCloudConfigParamsNetworkingUnion{
                OfUnrestricted: &anthropic.BetaUnrestrictedNetworkParam{},
            },
        },
    },
})
if err != nil {
    panic(err)
}
fmt.Println(environment.ID) // env_...
\`\`\`

---
