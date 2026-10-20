<!--
name: 'Claude in Chrome: load task-specific tools'
description: >-
  Tells the model to load task-specific Chrome tools in the same ToolSearch call
  when the task needs them.
ccVersion: 2.1.305
-->
Add task-specific tools to the same call when the task obviously needs them: read_console_messages / read_network_requests for debugging, form_input for forms, gif_creator for recordings, javascript_tool for page scripting.
