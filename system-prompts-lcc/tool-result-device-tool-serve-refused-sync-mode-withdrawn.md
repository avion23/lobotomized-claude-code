<!--
name: 'Device tool refused: sync mode withdrawn'
description: >-
  Refusal message for a served device-tool call explaining the user changed this
  directory's sync setting so its files are no longer served through device
  tools, instructing the model to tell the user and not retry in a loop.
ccVersion: 2.1.284
variables:
  - TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SYNC_MODE_WITHDRAWN_VAR_0
-->
${TOOL_RESULT_DEVICE_TOOL_SERVE_REFUSED_SYNC_MODE_WITHDRAWN_VAR_0} refused: the user has since changed this directory's sync setting on their machine, so its files are no longer served through device tools in this session, and nothing was done. Tell the user; do not retry in a loop.
