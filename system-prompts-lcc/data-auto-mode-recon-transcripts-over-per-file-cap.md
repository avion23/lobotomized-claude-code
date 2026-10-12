<!--
name: 'Auto-mode recon: transcripts over per-file cap'
description: >-
  Note that transcripts exceeded the per-file cap and only their most recent
  part was scanned.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_0
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_1
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_2
  - DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_3
-->

_${DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_0} ${DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_1(DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_0,"transcript")} exceeded the ${DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_2.round(DATA_AUTO_MODE_RECON_TRANSCRIPTS_OVER_PER_FILE_CAP_VAR_3.perFileCap/1048576)} MiB per-file cap — only the most recent part of each was scanned._
