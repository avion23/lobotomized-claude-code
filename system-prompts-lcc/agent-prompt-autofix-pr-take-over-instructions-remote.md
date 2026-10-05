<!--
name: 'Autofix PR poll prompt: take-over instructions (remote)'
description: >-
  Cloud/remote-environment branch of the take-over instructions embedded in the
  recurring 30-minute autofix-pr polling cron's agent prompt
ccVersion: 2.1.284
variables:
  - AGENT_PROMPT_AUTOFIX_PR_TAKE_OVER_INSTRUCTIONS_REMOTE_VAR_0
-->
the user removes \`${AGENT_PROMPT_AUTOFIX_PR_TAKE_OVER_INSTRUCTIONS_REMOTE_VAR_0}\` on GitHub, which makes PR Steward stand down and archives its session; don't remove it yourself, since PR Steward ignores removals by the Claude GitHub App, which this cloud session may act as
