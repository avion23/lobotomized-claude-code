<!--
name: 'Tool Result: Settings deny glob trailing separator'
description: >-
  Settings validation issue for a deny glob ending in a separator, with the
  corrected spelling
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_0
  - TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_1
-->
Deny glob "${TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_0}" ends in a separator, so as a pattern it can match no path. Write "${TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_0.replace(TOOL_RESULT_SETTINGS_DENY_GLOB_TRAILING_SEPARATOR_VAR_1,"")}", which is also read as the path of that name where it exists, or add a "**" segment to match at any depth.
