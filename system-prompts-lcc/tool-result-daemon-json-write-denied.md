<!--
name: 'Write denied: daemon.json'
description: Denial for writing the daemon.json file.
ccVersion: 2.1.300
-->
This path is daemon.json in the Claude Code config directory ($CLAUDE_CONFIG_DIR or ~/.claude), or a link, temp file or short name that stands in for it; above it, a Windows short name such as CLAUDE~1 counts as the folder in its place. The service that runs background sessions starts the workers listed there, so it cannot be written directly. A person can change it in an editor.
