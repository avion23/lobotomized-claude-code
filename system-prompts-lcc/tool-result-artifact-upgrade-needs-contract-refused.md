<!--
name: 'Tool Result: Artifact upgrade needs contract refused'
description: >-
  Says nothing was published because an upgrade stamps the current contract, and
  how to publish without it
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_UPGRADE_NEEDS_CONTRACT_REFUSED_VAR_0
-->
Nothing was published: an upgrade stamps the current contract. Tell the user that the upgrade has to be published from ${TOOL_RESULT_ARTIFACT_UPGRADE_NEEDS_CONTRACT_REFUSED_VAR_0}. To publish the content anyway, publish without the contract field (a stored contract stays as it is; if none is stored the page is published without one).
