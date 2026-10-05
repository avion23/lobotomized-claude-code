<!--
name: 'Output withheld: PostToolUse hook stopped'
description: >-
  Message explaining that a completed command's output is withheld because
  something that ran after it (most likely a PostToolUse hook) was stopped
  before finishing and may have needed to check that output.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_OUTPUT_WITHHELD_POSTTOOLUSE_HOOK_STOPPED_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_OUTPUT_WITHHELD_POSTTOOLUSE_HOOK_STOPPED_VAR_1
-->
(output withheld: the command COMPLETED on ${TOOL_RESULT_REMOTE_TOOL_OUTPUT_WITHHELD_POSTTOOLUSE_HOOK_STOPPED_VAR_0} and was not interrupted. What ran after it here — a PostToolUse hook, most likely — was stopped ${TOOL_RESULT_REMOTE_TOOL_OUTPUT_WITHHELD_POSTTOOLUSE_HOOK_STOPPED_VAR_1} before it finished, and it may have been meant to check this output, so only the output is withheld. Do not re-run the command just to see the output unless it is safe to repeat.)
