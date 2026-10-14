<!--
name: 'Tool Result: Git bundle Windows unholdable names no add all'
description: >-
  Warns not to run git add . or git commit -a because tracked names Windows
  cannot hold would be recorded as deletions
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_GIT_BUNDLE_WINDOWS_UNHOLDABLE_NAMES_NO_ADD_ALL_VAR_0
  - TOOL_RESULT_GIT_BUNDLE_WINDOWS_UNHOLDABLE_NAMES_NO_ADD_ALL_VAR_1
-->
${TOOL_RESULT_GIT_BUNDLE_WINDOWS_UNHOLDABLE_NAMES_NO_ADD_ALL_VAR_0} Do not run \`git add .\` or \`git commit -a\` here: this checkout tracks ${TOOL_RESULT_GIT_BUNDLE_WINDOWS_UNHOLDABLE_NAMES_NO_ADD_ALL_VAR_1} file ${TOOL_RESULT_GIT_BUNDLE_WINDOWS_UNHOLDABLE_NAMES_NO_ADD_ALL_VAR_1===1?"name":"names"} that Windows cannot hold, which git lists as deleted, and either command would record the ${TOOL_RESULT_GIT_BUNDLE_WINDOWS_UNHOLDABLE_NAMES_NO_ADD_ALL_VAR_1===1?"deletion":"deletions"}.
