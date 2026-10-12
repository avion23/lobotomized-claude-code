<!--
name: 'Auto-mode recon: transcripts scanned line'
description: >-
  Transcripts-scanned and Bash-commands-seen summary line of the recent-usage
  recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_0
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_1
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_2
-->
Transcripts scanned: ${DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_0.length-DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_1}${DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_1?` (${DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_1} skipped as oversized)`:""}; Bash commands seen: ${DATA_AUTO_MODE_RECON_TRANSCRIPTS_SCANNED_LINE_VAR_2.length}
