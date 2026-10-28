<!--
name: 'Tool Result: Project read local_file read-only'
description: >-
  Explains that local_file is read-only, long-line workarounds, and how to save
  changes through a new file
ccVersion: 2.1.311
variables:
  - TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_0
  - TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_1
  - TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_2
  - TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_3
  - TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_4
-->
local_file is for reading only${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_0?`. One of its lines is too long for ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_1} to page through, because ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_1}'s offset and limit count lines. ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_1} with no offset or limit gives only the first part of the file. ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_1} with an offset and limit gives whole lines, or an error if those lines do not fit. The file is too large for project_read to return inline. ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_2} shows a line or a match of over 500 characters as [Omitted long matching line]. With output_mode \`content\`, \`-o\` true and a pattern such as \`.{0,200}term.{0,200}\`, ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_2} shows each match of term with up to 200 characters on each side. In ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_3}, \`grep -ob 'term' /path/of/local_file | head\` gives the byte offset of each match of term, counted from 0. \`tail -c +START /path/of/local_file | head -c 20000\` gives 20000 bytes from byte START, counted from 1: START is an offset plus 1, or any number from 1 to size_bytes.`:`: read the parts you need with ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_1}'s offset and limit, or search it with ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_4}.`} Edits to ${TOOL_RESULT_PROJECT_READ_LOCAL_FILE_READ_ONLY_VAR_0?"local_file":"it"} never reach the project, and project_write rejects it as local_path. To change the document or make a file from it, run \`cat /path/of/local_file > new-name\` in the working directory, where new-name is a name that no file there has, and work on that file. To save a change, call project_write with the document's path and that file as local_path. If the document is an upload such as a PDF, that saves a new text document and leaves the upload as it is.
