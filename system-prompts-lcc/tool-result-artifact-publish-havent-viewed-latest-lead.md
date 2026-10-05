<!--
name: 'Publish refused: latest artifact version not viewed (lead)'
description: >-
  Lead sentence of the tool_result returned by efr(e) when a publish is refused
  because Claude has not viewed the artifact's latest version, before the
  live-version-serving-suffix and the reapply-your-edits remedy tail.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_PUBLISH_HAVENT_VIEWED_LATEST_LEAD_VAR_0
-->
You haven't viewed the latest version of this artifact${TOOL_RESULT_ARTIFACT_PUBLISH_HAVENT_VIEWED_LATEST_LEAD_VAR_0.live===void 0?"":` (the content host is serving version ${TOOL_RESULT_ARTIFACT_PUBLISH_HAVENT_VIEWED_LATEST_LEAD_VAR_0.live})`}, so nothing was published. 
