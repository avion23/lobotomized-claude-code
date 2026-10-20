<!--
name: 'Tool Parameter: Monitor timeout_ms (stops after reply)'
description: >-
  Monitor timeout_ms description with default and cap, noting the monitor may
  also stop soon after the reply
ccVersion: 2.1.304
variables:
  - TOOL_PARAMETER_MONITOR_TIMEOUT_MS_STOPS_AFTER_REPLY_VAR_0
  - TOOL_PARAMETER_MONITOR_TIMEOUT_MS_STOPS_AFTER_REPLY_VAR_1
-->
Kill the monitor after this deadline. Default ${TOOL_PARAMETER_MONITOR_TIMEOUT_MS_STOPS_AFTER_REPLY_VAR_0}ms. Deadlines above ${TOOL_PARAMETER_MONITOR_TIMEOUT_MS_STOPS_AFTER_REPLY_VAR_1}ms are capped to ${TOOL_PARAMETER_MONITOR_TIMEOUT_MS_STOPS_AFTER_REPLY_VAR_1}ms. It may also stop soon after your reply.
