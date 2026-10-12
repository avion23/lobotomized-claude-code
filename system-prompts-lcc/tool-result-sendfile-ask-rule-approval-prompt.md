<!--
name: 'Tool Result: SendFile ask-rule approval prompt'
description: >-
  SendFile permission ask message when an ask rule covers SendFile; returned to
  the model when prompts are unavailable.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_SENDFILE_ASK_RULE_APPROVAL_PROMPT_VAR_0
  - TOOL_RESULT_SENDFILE_ASK_RULE_APPROVAL_PROMPT_VAR_1
-->
Send ${TOOL_RESULT_SENDFILE_ASK_RULE_APPROVAL_PROMPT_VAR_0.files.length} ${TOOL_RESULT_SENDFILE_ASK_RULE_APPROVAL_PROMPT_VAR_1(TOOL_RESULT_SENDFILE_ASK_RULE_APPROVAL_PROMPT_VAR_0.files.length,"file")} to '${TOOL_RESULT_SENDFILE_ASK_RULE_APPROVAL_PROMPT_VAR_0.to}'? SendFile reads file contents.
