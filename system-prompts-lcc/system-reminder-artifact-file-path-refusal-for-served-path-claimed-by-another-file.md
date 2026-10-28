<!--
name: Artifact file_path refusal for served path claimed by another file
description: >-
  Refuses an Artifact publish whose file_path would be served at a different
  path than the one another file in the same call already claims, giving the two
  corrected files entries to choose from
ccVersion: 2.1.310
variables:
  - JSON_STRINGIFY_FN
  - SOURCE_FILE_ABSOLUTE_PATH
  - FORMAT_ASCII_SAFE_JSON_STRING_FN
  - SERVED_PATH
  - PUBLISH_PATH_CONTEXT
  - LIKELY_INTENDED_SERVED_PATH
  - FILES_ENTRY_SOURCE_PATH
-->
file_path: nothing was published. ${JSON_STRINGIFY_FN(SOURCE_FILE_ABSOLUTE_PATH)} would be served at ${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)}, its path relative to ${PUBLISH_PATH_CONTEXT.relativeTo.words} (${JSON_STRINGIFY_FN(PUBLISH_PATH_CONTEXT.relativeTo.dir)}), while this call sends another file to ${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH)}. If this file is the one meant for ${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH)}, send the call again${PUBLISH_PATH_CONTEXT.root!==void 0?", keeping `root` as it is,":""} with {${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH)}: ${FILES_ENTRY_SOURCE_PATH}} in \`files\` in place of the other file's entry. If ${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)} is the path you mean, send the call again${PUBLISH_PATH_CONTEXT.root!==void 0?", keeping `root` as it is,":""} with {${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)}: ${FILES_ENTRY_SOURCE_PATH}} added to \`files\`.
