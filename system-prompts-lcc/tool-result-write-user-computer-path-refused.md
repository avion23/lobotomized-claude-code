<!--
name: 'Write refused: user-computer path'
description: >-
  Refuses a file path that looks like it is on the user's computer and explains
  how to deliver files.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_0
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_1
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_2
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_3
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_4
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_5
  - TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_6
-->
${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_0} ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_1[0]} starts like a path on the user's computer and was refused; nothing was written. Neither ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_0} nor ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_2} runs there: on this session's machine that path names an unrelated file, which never reaches the user. If this session has ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_3}, make or change the file there with it. Otherwise save the finished file under ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_4()}, from where ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_5} copies it over; to change a file of theirs, first copy it here with ${TOOL_RESULT_WRITE_USER_COMPUTER_PATH_REFUSED_VAR_6}. With none of these tools, work here and tell the user that nothing was saved on their computer.
