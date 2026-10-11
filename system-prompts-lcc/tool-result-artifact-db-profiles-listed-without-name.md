<!--
name: 'Tool Result: Artifact DB Profiles — people listed without a name'
description: Lists the ids of people the service returned without a display name.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_ARTIFACT_DB_PROFILES_LISTED_WITHOUT_NAME_VAR_0
  - TOOL_RESULT_ARTIFACT_DB_PROFILES_LISTED_WITHOUT_NAME_VAR_1
-->

Listed without a name here: ${TOOL_RESULT_ARTIFACT_DB_PROFILES_LISTED_WITHOUT_NAME_VAR_0.map(TOOL_RESULT_ARTIFACT_DB_PROFILES_LISTED_WITHOUT_NAME_VAR_1).join("; ")}.
