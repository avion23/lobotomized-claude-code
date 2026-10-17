<!--
name: 'Tool result: cloud session changes stay on machine'
description: >-
  Trailer saying which commits and uncommitted changes stay on this machine,
  with an optional push hint.
ccVersion: 2.1.302
variables:
  - TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_0
  - TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_1
  - TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_2
  - TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_3
-->
${TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_0!==null?` Commits that ${TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_0} lacks, and any uncommitted changes, stay on this machine`:TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_1?" Later commits and any uncommitted changes stay on this machine":` ${TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_2.aheadCount===0?"Uncommitted changes":TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_2.aheadCount===1?"That commit and any uncommitted changes":`Those ${TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_2.aheadCount} commits and any uncommitted changes`} stay on this machine`}${TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_3||TOOL_RESULT_CLOUD_SESSION_CHANGES_STAY_ON_MACHINE_VAR_2.aheadCount===0?"; push the branch to start from it":""}.
