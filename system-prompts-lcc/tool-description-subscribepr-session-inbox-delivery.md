<!--
name: 'Tool Description: SubscribePR session inbox delivery'
description: >-
  SubscribePR description paragraph for remote-control project threads: events
  go to the session inbox as notifications carrying a file_id to read with the
  named tool
ccVersion: 2.1.304
variables:
  - TOOL_DESCRIPTION_SUBSCRIBEPR_SESSION_INBOX_DELIVERY_VAR_0
-->
In a session the \`claude remote-control\` daemon started for a project thread, events are placed in this session's inbox instead of arriving as user messages: each one is an \`<event source="session-inbox" kind="message.received">\` notification carrying a file_id — read it with the ${TOOL_DESCRIPTION_SUBSCRIBEPR_SESSION_INBOX_DELIVERY_VAR_0} tool.
