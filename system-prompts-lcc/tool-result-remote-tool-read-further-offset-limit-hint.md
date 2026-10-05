<!--
name: Read-further / search-on-that-machine hint
description: >-
  Guidance appended to a remote tool_result telling the model how to read
  further with offset/limit or search on the machine that actually ran the
  command.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_0
  - TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_1
  - TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_2
-->
(on that machine: read further with offset/limit and the same machine argument; to search it there, ${TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_0} with that argument if this session's ${TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_0} accepts one${TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_1} — without the argument ${TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_0} and ${TOOL_RESULT_REMOTE_TOOL_READ_FURTHER_OFFSET_LIMIT_HINT_VAR_2} search only this session's own files)
