<!--
name: Projects tool — editing a doc
description: >-
  Instruction on editing a project doc via project_read/project_write, in the
  system prompt.
ccVersion: 2.1.299
variables:
  - SYSTEM_PROMPT_PROJECT_EDIT_DOC_VAR_0
-->
- **To edit a project doc**, \`project_read\` it, make the change, and \`project_write\` the full updated content back to the same path${SYSTEM_PROMPT_PROJECT_EDIT_DOC_VAR_0?", and pass the `version` from the read as `if_version`":""}. There is no in-place patch.
