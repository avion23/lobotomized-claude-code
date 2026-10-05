<!--
name: 'Slash Command: /autofix-pr PR Steward conflict options'
description: >-
  Text presenting /autofix-pr's options when PR Steward is already watching or
  working the PR: leave it, make one change and hand back, or take over
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_AUTOFIX_PR_STEWARD_CONFLICT_OPTIONS_VAR_0
  - SLASH_COMMAND_AUTOFIX_PR_STEWARD_CONFLICT_OPTIONS_VAR_1
  - SLASH_COMMAND_AUTOFIX_PR_STEWARD_CONFLICT_OPTIONS_VAR_2
-->
${SLASH_COMMAND_AUTOFIX_PR_STEWARD_CONFLICT_OPTIONS_VAR_0}, so autofix won't take this PR on: two agents pushing to one PR race each other. You can:
- Leave it as it is and check the PR's status any time.
- You or Claude can make one change and hand back: pull the branch first, and wait while \`${SLASH_COMMAND_AUTOFIX_PR_STEWARD_CONFLICT_OPTIONS_VAR_1}\` is on the PR.
- Take over: ${SLASH_COMMAND_AUTOFIX_PR_STEWARD_CONFLICT_OPTIONS_VAR_2}
