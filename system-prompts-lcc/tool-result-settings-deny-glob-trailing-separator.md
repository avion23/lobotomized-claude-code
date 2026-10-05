<!--
name: 'Settings deny-glob ends in separator, matches no path'
description: >-
  Zod schema addIssue message emitted when a settings.json permissions deny glob
  ends in a path separator (matches no path); part of the settings schema sent
  whole to the model by /update-config and surfaced in settings validation
  errors.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_0
  - TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_1
-->
Deny glob "${TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_0}" ends in a separator, so the pattern can match no path. Write "${TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_0.replace(TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_1,"")}", or add a "**" segment to match at any depth.
