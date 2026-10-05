<!--
name: Remote command completed but answer withheld
description: >-
  tool_result text for when the command finished on the remote machine but its
  (too-large/refused) result could not be carried back; effects stand, do not
  re-run just to see output.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_ANSWER_COMPLETED_NOT_RETURNED_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_ANSWER_COMPLETED_NOT_RETURNED_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_ANSWER_COMPLETED_NOT_RETURNED_VAR_2
-->
The command ran to completion on ${TOOL_RESULT_REMOTE_TOOL_ANSWER_COMPLETED_NOT_RETURNED_VAR_0}, but its result ${TOOL_RESULT_REMOTE_TOOL_ANSWER_COMPLETED_NOT_RETURNED_VAR_1}, so it was not returned. Its effects stand — do not re-run it just to see the output.${TOOL_RESULT_REMOTE_TOOL_ANSWER_COMPLETED_NOT_RETURNED_VAR_2}
