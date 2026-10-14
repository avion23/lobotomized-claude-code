<!--
name: 'Tool Parameter: Artifact publish edits'
description: >-
  Describes the edits parameter: exact once-occurring old_str, in-order
  all-or-none application, saving to disk, and failure reporting
ccVersion: 2.1.299
variables:
  - TOOL_PARAMETER_ARTIFACT_PUBLISH_EDITS_VAR_0
  - TOOL_PARAMETER_ARTIFACT_PUBLISH_EDITS_VAR_1
  - TOOL_PARAMETER_ARTIFACT_PUBLISH_EDITS_VAR_2
-->
${TOOL_PARAMETER_ARTIFACT_PUBLISH_EDITS_VAR_0}${TOOL_PARAMETER_ARTIFACT_PUBLISH_EDITS_VAR_1}${TOOL_PARAMETER_ARTIFACT_PUBLISH_EDITS_VAR_2} Each old_str is text copied exactly from the file as it now stands and must occur in it exactly once; new_str takes its place (empty deletes it). The edits apply in order, all or none: the file is published with them and then saved with them on disk, so it stays the source for later changes; on a miss nothing is changed or published, and the result says which edit failed and why.
