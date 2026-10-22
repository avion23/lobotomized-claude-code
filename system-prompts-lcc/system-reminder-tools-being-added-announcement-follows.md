<!--
name: 'System Reminder: tools being added'
description: >-
  Names tools being added to the conversation and says the following
  announcement explains how to call them.
ccVersion: 2.1.308
variables:
  - SYSTEM_REMINDER_TOOLS_BEING_ADDED_ANNOUNCEMENT_FOLLOWS_VAR_0
-->
Being added to this conversation: ${SYSTEM_REMINDER_TOOLS_BEING_ADDED_ANNOUNCEMENT_FOLLOWS_VAR_0.join(", ")}. The announcement after this result says how to call ${SYSTEM_REMINDER_TOOLS_BEING_ADDED_ANNOUNCEMENT_FOLLOWS_VAR_0.length===1?"it":"them"}.
