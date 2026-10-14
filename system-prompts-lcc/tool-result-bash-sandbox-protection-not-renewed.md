<!--
name: 'Tool Result: Bash sandbox protection not renewed'
description: >-
  Says the sandbox could not confirm Claude Code's files are protected, so the
  command did not run, and gives the retry and override steps
ccVersion: 2.1.299
-->
The sandbox could not check that Claude Code's own files are still protected, so this command was not run. Try it once more. If it fails the same way, stop and tell the user: restarting Claude Code may clear it. If it does not, CLAUDE_CODE_SANDBOX_LEAVE_DENIES_TO_SRT_WIN=1 in the environment that Claude Code is started from (a settings file cannot set it) turns this check off, but the sandbox may then fail to start on a large profile.
