<!--
name: Built-in gh supported-command alternatives
description: >-
  Replacement command suggestions shown when the model invokes an unsupported gh
  subcommand through Bash.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_0
  - TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_1
  - TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_2
-->
Instead of \`gh ${TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_0}\`:
${TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_1.map((TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_2)=>`  ${TOOL_RESULT_BASH_INSTEAD_OF_GH_VAR_2}`).join(`
`)}
