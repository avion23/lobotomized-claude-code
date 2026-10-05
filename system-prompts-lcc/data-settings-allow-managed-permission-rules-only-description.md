<!--
name: 'Data: allowManagedPermissionRulesOnly setting description'
description: >-
  Description of the `allowManagedPermissionRulesOnly` setting in Claude Code's
  settings JSON schema. The model reads it through /update-config and settings
  validation errors; it is also shown to users in the settings help.
ccVersion: 2.1.284
-->
When true (and set in managed settings), permission rules from user, project, local, and --settings files and allow rules from --allowedTools are ignored; only managed settings can add allow rules through settings. 
