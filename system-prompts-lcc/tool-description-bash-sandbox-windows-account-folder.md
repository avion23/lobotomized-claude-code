<!--
name: 'Tool Description: Bash sandbox Windows account temp folder'
description: >-
  Explains the sandbox account folder is unreadable to the user and file tools;
  where to put temp files.
ccVersion: 2.1.308
variables:
  - TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_ACCOUNT_FOLDER_VAR_0
  - TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_ACCOUNT_FOLDER_VAR_1
  - TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_ACCOUNT_FOLDER_VAR_2
-->
the sandbox account's own folder: neither the user nor the ${TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_ACCOUNT_FOLDER_VAR_0}, ${TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_ACCOUNT_FOLDER_VAR_1} and ${TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_ACCOUNT_FOLDER_VAR_2} tools can open what a command writes there. Put a temporary file that the user or those tools must open in your scratchpad directory if you have one; otherwise put it in the working directory and delete it when done.
