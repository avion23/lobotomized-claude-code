<!--
name: 'Data: Personal hooks load errors notice (with note)'
description: >-
  Notice that some hooks in the user settings file have errors and won't run,
  listing them, followed by an extra note
ccVersion: 2.1.304
variables:
  - DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_0
  - DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_1
  - DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_2
  - DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_3
-->
Some hooks in ${DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_0} have errors and won't run in this session. Your other hooks and settings still apply. The hooks with errors:
${DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_1(DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_2)}
${DATA_PERSONAL_HOOKS_LOAD_ERRORS_NOTICE_WITH_NOTE_VAR_3}
