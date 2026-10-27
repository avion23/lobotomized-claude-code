<!--
name: 'Tool Result: MCP file input resolves elsewhere'
description: >-
  Error that a file can't be attached because its path resolves to another path;
  call again with the resolved path
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_0
  - TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_1
  - TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_2
-->
Cannot attach "${TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_0}": it resolves to another path${TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_1===void 0?", through a link or a name that is stored otherwise":`, "${TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_1}"`}. A file is attached only by the path it resolves to, so that the path that is approved names the file that is sent. If that is the file you mean, call again with ${TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_1===void 0?"the path it resolves to":"that path"}. ${TOOL_RESULT_MCP_FILE_INPUT_RESOLVES_ELSEWHERE_VAR_2}
