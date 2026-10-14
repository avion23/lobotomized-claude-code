<!--
name: 'Artifact publish: multi-file edit then publish'
description: >-
  Tool-description text for larger changes: edit files then publish in the same
  response.
ccVersion: 2.1.300
variables:
  - TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_0
  - TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_1
-->
 For a change to several files at once, or a rewrite of most of a page, Claude makes the change with ${TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_0}, not a shell command, and publishes the artifact again with the same file path in the same response: the ${TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_0} call(s) first, then the publish, with no ${TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_1} and without waiting for the ${TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_0} result. The calls run in the order sent, so the publish carries the edited file. If one of those ${TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_0} calls does not apply, the publish sent in the same response is refused and the artifact stays as it was, so Claude corrects the ${TOOL_DESCRIPTION_ARTIFACT_PUBLISH_MULTI_FILE_EDIT_THEN_PUBLISH_VAR_0} and publishes again. Either way, Claude reads the file first only when its text is not in this conversation or the change cannot be placed exactly from that text.
