<!--
name: 'Windows sandbox: profile forget remedy'
description: >-
  How to take back the profile grant by running profile forget with every
  session closed.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_PROFILE_FORGET_REMEDY_VAR_0
  - TOOL_RESULT_BASH_SANDBOX_WINDOWS_PROFILE_FORGET_REMEDY_VAR_1
-->
To take it back, close every Claude Code session and run "${TOOL_RESULT_BASH_SANDBOX_WINDOWS_PROFILE_FORGET_REMEDY_VAR_0.execPath}" ${TOOL_RESULT_BASH_SANDBOX_WINDOWS_PROFILE_FORGET_REMEDY_VAR_1} profile forget in a terminal; sandboxed commands then read nothing in your user profile.
