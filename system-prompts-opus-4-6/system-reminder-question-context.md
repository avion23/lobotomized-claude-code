<!--
name: 'System Reminder: Question context'
description: >-
  Provides potentially relevant context entries to use only when highly relevant
  to the current task
ccVersion: 2.1.178
variables:
  - QUESTION_CONTEXT
  - CONTEXT_ENTRY_LIMIT
  - CONTEXT_ENTRY_TITLE
  - CONTEXT_ENTRY_CONTENT
-->
<system-reminder>
Context you can use to answer the user's questions:
${QUESTION_CONTEXT.entries(CONTEXT_ENTRY_LIMIT).map(([CONTEXT_ENTRY_TITLE,CONTEXT_ENTRY_CONTENT])=>`# ${CONTEXT_ENTRY_TITLE}
${CONTEXT_ENTRY_CONTENT}`).join(`
`)}

This context may or may not be relevant; only use it if it bears on the task.
</system-reminder>
