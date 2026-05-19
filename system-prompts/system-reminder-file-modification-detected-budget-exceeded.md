<!--
name: 'System Reminder: File modification detected (budget exceeded)'
description: >-
  Reminder when a file changed mid-turn but the diff was dropped due to snippet
  budget
ccVersion: 2.1.142
variables:
  - FILE_OBJECT
-->
Note: ${FILE_OBJECT.filename} was modified, either by the user or by a linter. Take it into account as you proceed and don't revert it unless asked. The diff was omitted because other modified files in this turn already exceeded the snippet budget; use the Read tool if you need the current content.
