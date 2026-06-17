<!--
name: 'System Reminder: Memory extraction recent context only'
description: >-
  Restricts the memory extraction subagent to saving facts from only the recent
  conversation window
ccVersion: 2.1.178
variables:
  - RECENT_MESSAGE_COUNT
-->
Use only content from the last ~${RECENT_MESSAGE_COUNT} messages to update your persistent memories. Take that content as given — don't investigate or verify it further.
