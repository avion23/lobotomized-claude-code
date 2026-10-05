<!--
name: 'System Reminder: served PreToolUse hook error, home-directory note'
description: >-
  Note explaining that a PreToolUse hook errored on the machine serving a cloud
  session's command without blocking it, and that such hooks start in the home
  directory with a reduced environment, so a project-aware guard must read
  $CLAUDE_PROJECT_DIR or the cwd field on stdin
ccVersion: 2.1.284
-->
A PreToolUse hook on this machine exited with an error (whatever its cause) for a command your cloud session sent here and, as for a local command, did not block it. Note that hooks for such calls start in your home directory with a reduced environment: a guard that inspects the project must use $CLAUDE_PROJECT_DIR or the cwd field on stdin.
