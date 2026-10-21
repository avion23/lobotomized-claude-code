<!--
name: 'Data: /teleport — Session now in the cloud, Remote Control update failed'
description: >-
  /teleport result when the session moved to the cloud (with its URL) but Claude
  Code failed to finish updating Remote Control in this terminal, with the
  error.
ccVersion: 2.1.302
variables:
  - DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_0
  - DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_1
  - DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_2
  - DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_3
-->
Session now in the cloud: ${DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_0}
Claude Code didn’t finish updating Remote Control in this terminal after the move (${DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_1(DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_2)}).${DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_3===void 0?"":`
${DATA_TELEPORT_SESSION_NOW_IN_CLOUD_HEADLINE_VAR_3}`}
