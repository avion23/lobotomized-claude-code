<!--
name: Read Offset Param (Verbose)
description: >-
  Verbose-branch (XCe() true) description of the Read tool's offset parameter,
  including the tail-N hint for reading the end of a large file
ccVersion: 2.1.181
variables:
  - TOOL_PARAMETER_READ_OFFSET_VERBOSE_VAR_0
  - TOOL_PARAMETER_READ_OFFSET_VERBOSE_VAR_1
  - TOOL_PARAMETER_READ_OFFSET_VERBOSE_VAR_2
-->
The line number to start reading from. Only provide if the file is too large to read at once. Negative offsets are not supported (use ${TOOL_PARAMETER_READ_OFFSET_VERBOSE_VAR_0()?`${TOOL_PARAMETER_READ_OFFSET_VERBOSE_VAR_1} tail -N`:`${TOOL_PARAMETER_READ_OFFSET_VERBOSE_VAR_2} Get-Content -Tail N`} to read the end of a file).
