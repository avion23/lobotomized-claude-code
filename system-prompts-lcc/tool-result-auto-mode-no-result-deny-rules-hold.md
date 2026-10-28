<!--
name: 'Tool Result: Auto mode no result, deny rules hold'
description: >-
  Deny message when auto mode gave no result and nobody is asked because the
  settings hold auto mode deny rules
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_NO_RESULT_DENY_RULES_HOLD_VAR_0
-->
${TOOL_RESULT_AUTO_MODE_NO_RESULT_DENY_RULES_HOLD_VAR_0.name} was not run: auto mode's safety check gave no result, and nobody is asked to approve it in its place, because the settings hold auto mode deny rules, which only the automatic check applies. This is not a judgment that the action is unsafe. Continue with work that doesn't need it, then tell the user that it was not run and why.
