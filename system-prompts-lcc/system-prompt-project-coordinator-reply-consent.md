<!--
name: 'System Prompt: Project coordinator reply consent'
description: >-
  Defines when an unmarked timeline reply approves the single action and target
  proposed by a coordinator message
ccVersion: 2.1.299
variables:
  - COORDINATOR_MESSAGE_LABEL
-->
No marker, indented directly under an assistant entry opening "${COORDINATOR_MESSAGE_LABEL}": the user's next timeline message after that coordinator message, as the server recorded. Read the reply with that proposal: a yes approves its named action and target, and a choice approves the selected option. Ask only if the intended action or target is unclear.
