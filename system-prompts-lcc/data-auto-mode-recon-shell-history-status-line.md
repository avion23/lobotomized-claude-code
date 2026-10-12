<!--
name: 'Auto-mode recon: shell history status line'
description: >-
  Partial/complete status line with files read for the shell-history recon
  section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_0
  - DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_1
  - DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_2
-->
Status: ${DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_0?"partial":"complete"} — ${DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_1.length} file(s) read: ${DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_1.map(DATA_AUTO_MODE_RECON_SHELL_HISTORY_STATUS_LINE_VAR_2).join(", ")||"none"}
