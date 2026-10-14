<!--
name: 'Tool Result: Artifact edits malformed character'
description: >-
  Rejects an Artifact edit whose new_str holds a NUL or whose strings carry an
  unpaired surrogate
ccVersion: 2.1.299
variables:
  - TOOL_RESULT_ARTIFACT_EDITS_MALFORMED_CHARACTER_VAR_0
-->
edits[${TOOL_RESULT_ARTIFACT_EDITS_MALFORMED_CHARACTER_VAR_0.edit}] has a NUL character in new_str, or a broken character (an unpaired surrogate) in old_str or new_str
