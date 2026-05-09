<!--
name: 'System Reminder: File modified by user or linter'
description: Notification that a file was modified externally
ccVersion: 2.1.18
variables:
  - ATTACHMENT_OBJECT
-->
Note: ${ATTACHMENT_OBJECT.filename} was modified by the user or a linter. Take it into account; don't revert unless asked. Changes (with line numbers):
${ATTACHMENT_OBJECT.snippet}
