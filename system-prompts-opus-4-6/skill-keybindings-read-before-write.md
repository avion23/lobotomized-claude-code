<!--
name: 'Skill: Keybindings read before write'
description: >-
  Keybindings skill instruction to read ~/.claude/keybindings.json before
  merging changes.
ccVersion: 2.1.178
-->
Read `~/.claude/keybindings.json` first (it may not exist yet). Merge changes with existing bindings rather than replacing the file.
