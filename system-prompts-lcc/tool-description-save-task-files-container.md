<!--
name: 'Tool Description: Save task files into container'
description: Describes saving task files into the chat's container
ccVersion: 2.1.311
variables:
  - TOOL_DESCRIPTION_SAVE_TASK_FILES_CONTAINER_VAR_0
-->
Save files that a task produced into this chat's container, where this session's shell commands and file tools work. ${TOOL_DESCRIPTION_SAVE_TASK_FILES_CONTAINER_VAR_0} Each file is saved in this chat's task-files folder in the container under that name, with a number added if the name is taken; nothing is overwritten. A saved file stays while the chat's container keeps its disk, so a later turn may find it gone. The person is asked to approve every call. The answer says where each file was saved, or why it was not.
