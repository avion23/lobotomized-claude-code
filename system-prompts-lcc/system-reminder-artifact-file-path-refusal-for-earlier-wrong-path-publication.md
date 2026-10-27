<!--
name: Artifact file_path refusal for earlier wrong-path publication
description: >-
  Refuses an Artifact publish whose file_path would be served at a path that
  differs from an earlier publication of the same file under a deeper folder,
  offering files entries to serve it correctly or replace the old path
ccVersion: 2.1.310
variables:
  - JSON_STRINGIFY_FN
  - SOURCE_FILE_ABSOLUTE_PATH
  - FORMAT_ASCII_SAFE_JSON_STRING_FN
  - SERVED_PATH
  - PUBLISH_PATH_CONTEXT
  - IS_LIKELY_INTENDED_PATH_ALREADY_PUBLISHED
  - LIKELY_INTENDED_SERVED_PATH
  - IS_ONLY_FILE_UNDER_INTENDED_TOP_LEVEL_FOLDER
  - INTENDED_TOP_LEVEL_FOLDER
  - PUBLISHED_FILES_SCOPE_DESCRIPTION
  - RESEND_WITH_FILES_ENTRY_INSTRUCTION
  - FILES_ENTRY_SOURCE_PATH
  - INTENDED_PATH_UNTRUSTED_DATA_NOTE
-->
file_path: nothing was published. ${JSON_STRINGIFY_FN(SOURCE_FILE_ABSOLUTE_PATH)} would be served at ${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)}, its path relative to ${PUBLISH_PATH_CONTEXT.relativeTo.words} (${JSON_STRINGIFY_FN(PUBLISH_PATH_CONTEXT.relativeTo.dir)}), while ${IS_LIKELY_INTENDED_PATH_ALREADY_PUBLISHED?`${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH)}, which ends in ${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)}, is ${IS_ONLY_FILE_UNDER_INTENDED_TOP_LEVEL_FOLDER?`the only file under ${FORMAT_ASCII_SAFE_JSON_STRING_FN(INTENDED_TOP_LEVEL_FOLDER)}`:`already one of ${PUBLISHED_FILES_SCOPE_DESCRIPTION}`}: either it was`:`${PUBLISHED_FILES_SCOPE_DESCRIPTION} are all under ${FORMAT_ASCII_SAFE_JSON_STRING_FN(INTENDED_TOP_LEVEL_FOLDER)}: either they were`} published at a wrong path earlier, or ${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)} is not the path this Artifact's page reads. ${PUBLISH_PATH_CONTEXT.root!==void 0?"Keeping `root` as it is, s":"S"}${RESEND_WITH_FILES_ENTRY_INSTRUCTION.slice(1)} {${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)}: ${FILES_ENTRY_SOURCE_PATH}} to serve it at ${FORMAT_ASCII_SAFE_JSON_STRING_FN(SERVED_PATH)}${IS_ONLY_FILE_UNDER_INTENDED_TOP_LEVEL_FOLDER?"":` (then publish the Artifact's other files again without the leading ${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH.slice(0,-SERVED_PATH.length))})`}, or {${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH)}: ${FILES_ENTRY_SOURCE_PATH}} to ${IS_LIKELY_INTENDED_PATH_ALREADY_PUBLISHED?"replace":"serve it at"} ${FORMAT_ASCII_SAFE_JSON_STRING_FN(LIKELY_INTENDED_SERVED_PATH)}. A path stated in \`files\` is used as it is.${INTENDED_PATH_UNTRUSTED_DATA_NOTE}
