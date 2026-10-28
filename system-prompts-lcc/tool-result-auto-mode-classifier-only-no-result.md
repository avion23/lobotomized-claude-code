<!--
name: 'Tool Result: Classifier-only tool got no safety result'
description: >-
  Deny message when only auto mode's safety check can allow the tool and it gave
  no result
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_CLASSIFIER_ONLY_NO_RESULT_VAR_0
-->
${TOOL_RESULT_AUTO_MODE_CLASSIFIER_ONLY_NO_RESULT_VAR_0.name} was not run: only auto mode's safety check can allow it, and that check gave no result. No permission prompt is raised for this tool. This is not a judgment that the action is unsafe. Continue with work that doesn't need it, then tell the user that it was not run and why.
