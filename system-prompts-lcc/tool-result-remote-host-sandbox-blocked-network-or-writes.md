<!--
name: 'Tool Result: Remote host sandbox blocked network or writes'
description: >-
  Tells Claude a command ran inside the target machine's Claude Code sandbox,
  which can block network connections and file writes outside the working
  directories, and to tell the user what was blocked instead of guessing at
  another cause if that's why the command failed.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_REMOTE_HOST_SANDBOX_BLOCKED_NETWORK_OR_WRITES_VAR_0
  - TOOL_RESULT_REMOTE_HOST_SANDBOX_BLOCKED_NETWORK_OR_WRITES_VAR_1
-->
This command ran on ${TOOL_RESULT_REMOTE_HOST_SANDBOX_BLOCKED_NETWORK_OR_WRITES_VAR_0} inside Claude Code's sandbox, which is switched on there. The sandbox can block network connections and file writes outside the working directories.${TOOL_RESULT_REMOTE_HOST_SANDBOX_BLOCKED_NETWORK_OR_WRITES_VAR_1?" The sandbox_violations lines in the output name what it blocked.":""} If that is why the command failed, running it again unchanged will fail the same way — tell the user what was blocked instead of guessing at another cause.
