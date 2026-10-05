<!--
name: 'Slash Command: /autofix-pr PR Steward may have stalled'
description: >-
  Part of the /autofix-pr deferred-to-PR-Steward guidance, telling the model
  that if PR Steward isn't actually active it may have stopped without clearing
  its label, and to remove the label and re-run /autofix-pr.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_AUTOFIX_PR_STEWARD_ACTIVE_RACE_VAR_0
-->
if PR Steward isn't active, it may have stopped without clearing \`${SLASH_COMMAND_AUTOFIX_PR_STEWARD_ACTIVE_RACE_VAR_0}\`. Remove that label on GitHub and run /autofix-pr again.
