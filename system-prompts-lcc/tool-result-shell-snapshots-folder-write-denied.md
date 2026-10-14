<!--
name: 'Write denied: shell-snapshots folder'
description: Denial for writing into the shell-snapshots folder.
ccVersion: 2.1.300
-->
This path is in, or leads into, the shell-snapshots folder of the Claude Code config directory ($CLAUDE_CONFIG_DIR or ~/.claude); a Windows short name such as SHELL-~1 or CLAUDE~1 counts as the folder in its place. Each Bash command first runs a snapshot, kept there, of the shell setup (aliases, functions, options), so the files cannot be written directly. Claude Code takes a new snapshot each time it starts, so a person can change their shell startup file, such as ~/.bashrc or ~/.zshrc, and restart Claude Code.
