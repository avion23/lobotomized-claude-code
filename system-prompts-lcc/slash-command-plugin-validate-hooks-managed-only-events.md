<!--
name: 'Slash Command: Plugin validate hooks managed-only events'
description: >-
  Validation note that hooks on certain events run only for plugins an
  organization lists in managed settings
ccVersion: 2.1.299
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MANAGED_ONLY_EVENTS_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MANAGED_ONLY_EVENTS_VAR_1
-->
${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MANAGED_ONLY_EVENTS_VAR_0} hooks on ${SLASH_COMMAND_PLUGIN_VALIDATE_HOOKS_MANAGED_ONLY_EVENTS_VAR_1.join(", ")} do not run in a plugin a person installs where an organization manages Claude Code: there, these events pass over the plugins you install, and only a plugin the organization lists in managed settings runs them
