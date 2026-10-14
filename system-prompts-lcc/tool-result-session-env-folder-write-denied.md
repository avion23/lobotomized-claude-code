<!--
name: 'Write denied: session-env folder'
description: Denial for writing into the session-env folder.
ccVersion: 2.1.300
-->
This path is in, or leads into, the session-env folder of the Claude Code config directory ($CLAUDE_CONFIG_DIR or ~/.claude); a Windows short name such as SESSIO~1 or CLAUDE~1 counts as the folder in its place. Claude Code runs the scripts that hooks leave there ahead of Bash commands, so they cannot be written directly. To set variables for later Bash commands, a person can add a SessionStart hook that appends export lines to the file named in $CLAUDE_ENV_FILE.
