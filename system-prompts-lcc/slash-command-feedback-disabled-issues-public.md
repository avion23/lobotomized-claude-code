<!--
name: 'Slash command: feedback disabled, issues public note'
description: >-
  Wrapper that appends the warning that GitHub issues are public, so
  confidential details should be left out, to the feedback-disabled sentence.
ccVersion: 2.1.302
variables:
  - SLASH_COMMAND_FEEDBACK_DISABLED_ISSUES_PUBLIC_VAR_0
  - SLASH_COMMAND_FEEDBACK_DISABLED_ISSUES_PUBLIC_VAR_1
-->
${`${SLASH_COMMAND_FEEDBACK_DISABLED_ISSUES_PUBLIC_VAR_0} is disabled by your organization's policy. To report a bug, open an issue at ${SLASH_COMMAND_FEEDBACK_DISABLED_ISSUES_PUBLIC_VAR_1()}.`} Issues are public, so leave out anything confidential.
