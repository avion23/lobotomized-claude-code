<!--
name: 'Tool Result: Workflow script ambiguous slash'
description: >-
  Syntax error that a '/' in the script body could be a regex or a division,
  asking to end the previous statement with ';'
ccVersion: 2.1.304
variables:
  - TOOL_RESULT_WORKFLOW_SCRIPT_AMBIGUOUS_SLASH_VAR_0
  - TOOL_RESULT_WORKFLOW_SCRIPT_AMBIGUOUS_SLASH_VAR_1
-->
Line ${TOOL_RESULT_WORKFLOW_SCRIPT_AMBIGUOUS_SLASH_VAR_0}, column ${TOOL_RESULT_WORKFLOW_SCRIPT_AMBIGUOUS_SLASH_VAR_1} of the script body (counted after the meta statement, if any): this '/' could be read either as the start of a regular expression or as a division, so the script was not run. End the statement before it with ';' (or parenthesize the expression) so it reads one way.
