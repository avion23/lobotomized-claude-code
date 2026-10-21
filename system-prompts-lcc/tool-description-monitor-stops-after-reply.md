<!--
name: 'Tool Description: Monitor stops after reply'
description: >-
  Monitor description note for sessions where a monitor is only reliable while
  Claude works: it may stop soon after the reply, so wait with a foreground
  command or tell the user what to check
ccVersion: 2.1.304
variables:
  - TOOL_DESCRIPTION_MONITOR_STOPS_AFTER_REPLY_VAR_0
-->
In this session a monitor can be counted on only while you are working. After your reply it may stop at any time, often within a minute, and you are told so with the user's next message. To wait for one thing before you answer, run a foreground ${TOOL_DESCRIPTION_MONITOR_STOPS_AFTER_REPLY_VAR_0} command that exits when it happens; for anything longer, tell the user what to check and when.
