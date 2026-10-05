<!--
name: 'Artifact publish: HTML files missing doctype'
description: >-
  Warning appended to the Artifact publish tool result's warnings array when
  published HTML supporting files lack <!doctype html>.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_0
  - TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_1
-->
files: ${TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_0} ${TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_1?"has":"have"} no <!doctype html> — supporting HTML pages are served exactly as written (only the page itself is wrapped in the skeleton), so if ${TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_1?"it is a page":"they are pages"} people open, start ${TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_1?"it":"each"} with a doctype, charset and viewport meta and its base styles and publish again (a fragment the page fetches and inserts can stay as written); as published ${TOOL_RESULT_ARTIFACT_PUBLISH_HTML_NO_DOCTYPE_WARNING_VAR_1?"it renders":"they render"} in quirks mode.
