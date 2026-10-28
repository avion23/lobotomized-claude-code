<!--
name: 'Tool Result: Reissue call with the hook-produced input'
description: >-
  Clause quoting the hook-produced input and telling Claude to issue the call
  once more with exactly that input so auto mode reviews it
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_QUOTED_INPUT_VAR_0
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_QUOTED_INPUT_VAR_1
  - TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_QUOTED_INPUT_VAR_2
-->
The hook produced this input: ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_QUOTED_INPUT_VAR_0.json}. In your next response, issue the ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_QUOTED_INPUT_VAR_1} call once more with exactly that input so auto mode reviews it. Put nothing else in that response but other calls whose denial quoted an input like this one. If it is denied again, do not retry; ${TOOL_RESULT_AUTO_MODE_HOOK_REWRITE_REISSUE_QUOTED_INPUT_VAR_2}
