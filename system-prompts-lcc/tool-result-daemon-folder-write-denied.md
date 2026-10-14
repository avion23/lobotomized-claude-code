<!--
name: 'Write denied: daemon folder'
description: Denial for writing into the Claude Code daemon folder.
ccVersion: 2.1.300
-->
This path is in, or leads into, the daemon folder of the Claude Code config directory ($CLAUDE_CONFIG_DIR or ~/.claude); a Windows short name such as CLAUDE~1 counts as the folder in its place. The service that runs background sessions acts on the files there, so they cannot be written directly. A person can check the service with `claude daemon status`.
