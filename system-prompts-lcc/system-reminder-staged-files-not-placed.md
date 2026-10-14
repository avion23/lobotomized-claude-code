<!--
name: 'System Reminder: Staged files not placed'
description: >-
  Lists handed-off files that may be missing or stale because they did not
  arrive at the current worker.
ccVersion: 2.1.300
variables:
  - SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_0
  - SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_1
  - SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_2
  - SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_3
  - SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_4
  - SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_5
-->
${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_0.length} ${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_1?"file":"files"} may not have arrived here, so ${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_1?"this path":"these paths"} may be missing or hold an older copy: ${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_0.slice(0,SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_2).map(SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_3).join(", ")}${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_4>0?`, and ${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_4} more`:""}${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_5.has("no_space")?`
At least one of these copies failed with "no space left on device". Make space before the file is sent again. Ask the user before you delete one of their files.`:""}${SYSTEM_REMINDER_STAGED_FILES_NOT_PLACED_VAR_5.has("name_too_long")?`
At least one of these names is too long for the file system here (the usual limit is 255 bytes). That file can arrive only after the name is made shorter.`:""}
