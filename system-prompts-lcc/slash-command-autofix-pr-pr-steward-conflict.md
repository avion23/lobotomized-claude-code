<!--
name: 'Slash Command: /autofix-pr PR Steward conflict'
description: >-
  Fragment of the /autofix-pr result explaining that another agent (typically PR
  Steward) is already watching or working the PR, that removing the label stands
  it down and archives its session, and that a stale label should be removed
  before running /autofix-pr again
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_AUTOFIX_PR_PR_STEWARD_CONFLICT_VAR_0
-->
Removing it makes PR Steward stand down on this PR and archives its session. Once it has, remove \`${SLASH_COMMAND_AUTOFIX_PR_PR_STEWARD_CONFLICT_VAR_0}\` too if it is still on, and run /autofix-pr again.
