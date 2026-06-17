<!--
name: 'System Reminder: Read truncation retry guidance'
description: >-
  Instructs Claude to reduce chunk size after file-read truncation warnings and
  notes the Bash output character limit
ccVersion: 2.1.178
variables:
  - MAX_OUTPUT_CHARS
-->
- If you receive truncation warnings when reading the file ("[N lines truncated]"), reduce the chunk size until you have read 100% of the content without truncation. Bash output is limited to ${MAX_OUTPUT_CHARS.toLocaleString()} chars.
