<!--
name: >-
  System Reminder: ambient context — The following MCP servers have
  disconnected. Their instructi
description: >-
  Normalized attachment reminder: The following MCP servers have disconnected.
  Their instructions above no longer apply:

  ${.join(`

  `)}. Inserted into normalized model context as a meta reminder.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_AMBIENT_FOLLOWING_MCP_SERVERS_HAVE_DISCONNECTED_THEIR_VAR_0
-->
The following MCP servers have disconnected. Their instructions above no longer apply:
${SYSTEM_REMINDER_AMBIENT_FOLLOWING_MCP_SERVERS_HAVE_DISCONNECTED_THEIR_VAR_0.join(`
`)}
