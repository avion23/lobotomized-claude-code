<!--
name: 'Write denied: jobs folder'
description: Denial for writing into the Claude Code jobs folder.
ccVersion: 2.1.300
-->
This path is in, or leads into, the jobs folder of the Claude Code config directory ($CLAUDE_CONFIG_DIR or ~/.claude); a Windows short name such as CLAUDE~1 counts as the folder in its place. Claude Code restarts background sessions from the files there, so they cannot be written directly. Scratch files of a background session go in $CLAUDE_JOB_DIR/tmp. A person can stop, restart or remove a session in `claude agents`, or with `claude stop <id>`, `claude respawn <id>` or `claude rm <id>`.
