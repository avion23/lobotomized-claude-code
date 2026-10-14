<!--
name: 'Tool Result: Artifact clear needs contract refused'
description: >-
  Says nothing was cleared, stored grants stay live, and the clear must come
  from a contract-capable session
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_CLEAR_NEEDS_CONTRACT_REFUSED_VAR_0
-->
Nothing was cleared: clearing a stored declaration needs the current contract, so any stored grants are still live. Tell the user that, and that the declaration has to be cleared from ${TOOL_RESULT_ARTIFACT_CLEAR_NEEDS_CONTRACT_REFUSED_VAR_0}.
