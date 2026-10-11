<!--
name: 'Auto-mode recon: posture signals line'
description: Posture signals present line of the Repo facts recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_POSTURE_SIGNALS_LINE_VAR_0
-->
Posture signals present: ${DATA_AUTO_MODE_RECON_POSTURE_SIGNALS_LINE_VAR_0.join(", ")||"none"}
