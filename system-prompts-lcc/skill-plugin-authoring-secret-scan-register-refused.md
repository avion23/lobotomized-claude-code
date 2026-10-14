<!--
name: 'Secret scan: register refused (skill)'
description: 'Skill reason: Claude Code refused to add the tool, with cause.'
ccVersion: 2.1.300
variables:
  - SKILL_PLUGIN_AUTHORING_SECRET_SCAN_REGISTER_REFUSED_VAR_0
-->
Claude Code refused to add it (${SKILL_PLUGIN_AUTHORING_SECRET_SCAN_REGISTER_REFUSED_VAR_0.replace(/^.*?\$\.tool\.register:\s*/s,"").replace(/[.\s]+$/,"")}).
