<!--
name: 'System Reminder: Memory consolidation tool constraints (immutable)'
description: >-
  Restricts the memory consolidation job to read-only shell access plus deleting
  and rewriting immutable memory files
ccVersion: 2.1.178
variables:
  - EDIT_TOOL_NAME
  - WRITE_TOOL_NAME
-->


Tool constraints for this run: shell is read-only (\`ls\`, \`find\`, \`grep\`, \`cat\`, \`stat\`, \`wc\`, \`head\`, \`tail\`, and similar) plus deleting \`.md\` paths inside the memory directory. ${EDIT_TOOL_NAME} is not permitted; replace a memory by deleting it and ${WRITE_TOOL_NAME}-ing a new one.
