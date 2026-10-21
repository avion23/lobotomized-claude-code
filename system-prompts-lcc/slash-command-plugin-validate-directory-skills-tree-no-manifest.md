<!--
name: 'Plugin validate: skills tree without manifest'
description: 'Finding: no plugin.json, but a skills tree loads as a plugin.'
ccVersion: 2.1.305
-->
No .claude-plugin/plugin.json. This folder holds a skills tree (skills/<name>/SKILL.md), which Claude Code loads without a manifest, so the directory accepts it as a plugin; anything else in it (agents/, commands/, hooks/, …) is validated and loads with it.
