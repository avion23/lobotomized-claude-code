<!--
name: Project document too large to rewrite refusal
description: >-
  Refuses a project doc write when the existing doc exceeds the inline read
  size, warning against retyping from a partial view or deleting it, and
  pointing to a complete local_path file or a new path
ccVersion: 2.1.310
variables:
  - MAX_INLINE_PROJECT_DOC_BYTES
-->
Write refused; nothing in the project was changed. The doc at this path holds more than ${MAX_INLINE_PROJECT_DOC_BYTES} bytes, more than project_read shows inline, so a rewrite typed from what it showed you would drop the rest. Do not delete the doc to write it again unless the user asks: a delete cannot be undone here. If you have the whole new text in a file that this session accepts as \`local_path\`, pass that file, but not a file made from only part of the doc. Otherwise write the new text to a new path, and tell the user that this doc is too large to rewrite here.
