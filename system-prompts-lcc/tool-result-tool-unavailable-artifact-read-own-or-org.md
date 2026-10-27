<!--
name: Artifact read own or org clause
description: >-
  Clause that the MCP read tool reads the user's or their org's artifacts, with
  a fallback
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_0
  - TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_1
  - TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_2
-->
 ${TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_0} reads an artifact the user owns, or one from their organization that they can open; ${TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_1?`for a link ${TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_0} refuses, use ${TOOL_RESULT_TOOL_UNAVAILABLE_ARTIFACT_READ_OWN_OR_ORG_VAR_2}.`:"for anything else, tell the user."}
