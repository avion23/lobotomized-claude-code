<!--
name: Code review reused finding limit
description: >-
  Notice that a previously selected max-findings value was reused for the
  review.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_CODE_SET_MAX_FINDINGS_LAST_TIME_VAR_0
  - SLASH_COMMAND_CODE_SET_MAX_FINDINGS_LAST_TIME_VAR_1
  - SLASH_COMMAND_CODE_SET_MAX_FINDINGS_LAST_TIME_VAR_2
-->
${SLASH_COMMAND_CODE_SET_MAX_FINDINGS_LAST_TIME_VAR_0==="you"?"You":"The user"} set \`--max-findings ${SLASH_COMMAND_CODE_SET_MAX_FINDINGS_LAST_TIME_VAR_1}\` last time. ${SLASH_COMMAND_CODE_SET_MAX_FINDINGS_LAST_TIME_VAR_2}
