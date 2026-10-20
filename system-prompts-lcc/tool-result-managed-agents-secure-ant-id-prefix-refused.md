<!--
name: 'Tool Result: managed-agents-secure ant ID prefix refused'
description: >-
  PreToolUse callback denial that a command holds an agent_/env_/vlt_ ID with a
  non-production prefix
ccVersion: 2.1.304
-->
Claude Code did not run this command: it holds an ID starting agent_, env_ or vlt_ then staging_, local_, vrtx_ or bdrk_, which `ant` commands may not use. Do not run the command another way: tell the developer which ID was refused and ask where it came from. If this is part of /claude-api managed-agents-secure, mark each report row that needs it CAN'T TELL.
