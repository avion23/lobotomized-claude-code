<!--
name: List connectors needs reconnect call
description: >-
  Tool prompt clause that enabledInChat false with needs_reconnect means the
  user must sign in again, calling a tool so the app can offer it
ccVersion: 2.1.310
variables:
  - TOOL_DESCRIPTION_LIST_CONNECTORS_NEEDS_RECONNECT_CALL_TOOL_VAR_0
-->
 enabledInChat: false with installState: "needs_reconnect" means the connector needs the user to sign in to it again; if the task needs it, call ${TOOL_DESCRIPTION_LIST_CONNECTORS_NEEDS_RECONNECT_CALL_TOOL_VAR_0} with its directoryUuid so the app can offer them a way to do that, and do not tell them to enable it for this chat.
