<!--
name: 'Tool result: workflow agent disallowedTools case mismatch (tail)'
description: >-
  Closing fragment of the agent() refusal when a deny entry differs from an
  existing tool only by case.
ccVersion: 2.1.296
-->
tool names are case-sensitive. Refusing the spawn rather than running it with this deny silently dropped.
