<!--
name: 'Data: Monitor stopped (too much output)'
description: >-
  Monitor event instructing the model to write a tighter monitor command after
  output suppression.
ccVersion: 2.1.178
variables:
  - DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_0
  - DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_1
  - DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_2
  - DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_3
-->

[Monitor stopped — your script produced too much output (${DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_0} events suppressed over ${DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_1.round((DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_2.now()-DATA_MONITOR_STOPPED_TOO_MUCH_OUTPUT_VAR_3)/1000)}s). Write a new monitor command that filters more selectively.]
