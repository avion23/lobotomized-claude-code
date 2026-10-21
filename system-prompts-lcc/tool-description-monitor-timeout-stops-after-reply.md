<!--
name: 'Tool Description: Monitor timeout (stops after reply)'
description: >-
  Monitor description timeout note: every monitor expires after timeout_ms with
  one notice, and if it stops after the reply Claude learns only that it stopped
ccVersion: 2.1.304
variables:
  - TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_0
  - TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_1
  - TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_2
-->
Every monitor expires after \`timeout_ms\` (default ${TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_0(TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_1)}, at most ${TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_0(TOOL_DESCRIPTION_MONITOR_TIMEOUT_STOPS_AFTER_REPLY_VAR_2())}): it is killed and you get one notice with the event count.
