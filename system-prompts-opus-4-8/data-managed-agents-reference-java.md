<!--
name: 'Data: Managed Agents reference — Java'
description: Managed Agents reference for Java SDK
ccVersion: 2.1.185
-->
# Managed Agents — Java

> **Bindings not shown here:** This README covers the most common managed-agents flows for Java. If you need a class, method, namespace, field, or behavior that isn't shown, WebFetch the Java SDK repo **or the relevant docs page** from `shared/live-sources.md` rather than guess. Do not extrapolate from cURL shapes or another language's SDK.

> **Agents are persistent — create once, reference by ID.** Store the agent ID returned by `client.beta().agents().create` and pass it to every subsequent `client.beta().sessions().create`; do not call `agents().create` in the request path. The Anthropic CLI is one convenient way to create agents and environments from version-controlled YAML — its URL is in `shared/live-sources.md`. The examples below show in-code creation for completeness; in production the create call belongs in setup, not in the request path.

## Installation

```xml
<dependency>
    <groupId>com.anthropic</groupId>
    <artifactId>anthropic-java</artifactId>
</dependency>
```

## Client Initialization

```java
import com.anthropic.client.okhttp.AnthropicOkHttpClient;

// Default (uses ANTHROPIC_API_KEY env var)
var client = AnthropicOkHttpClient.fromEnv();
```

---

## Create an Environment

```java
import com.anthropic.models.beta.environments.BetaCloudConfigParams;
import com.anthropic.models.beta.environments.BetaUnrestrictedNetwork;
import com.anthropic.models.beta.environments.EnvironmentCreateParams;

var environment = client.beta().environments().create(EnvironmentCreateParams.builder()
    .name("my-dev-env")
    .config(BetaCloudConfigParams.builder()
        .networking(BetaUnrestrictedNetwork.builder().build())
        .build())
    .build());
System.out.println("Environment ID: " + environment.id()); // env_...
```

---
