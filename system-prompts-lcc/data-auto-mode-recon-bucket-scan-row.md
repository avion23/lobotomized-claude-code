<!--
name: 'Data: Auto-Mode Recon Bucket Scan Row'
description: >-
  One line of the auto-mode recon report bucket-name list: the bucket name, its
  occurrence count and how many files mention it.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_BUCKET_SCAN_ROW_VAR_0
  - DATA_AUTO_MODE_RECON_BUCKET_SCAN_ROW_VAR_1
-->
- ${DATA_AUTO_MODE_RECON_BUCKET_SCAN_ROW_VAR_0} (${DATA_AUTO_MODE_RECON_BUCKET_SCAN_ROW_VAR_1.occurrences}×, ${DATA_AUTO_MODE_RECON_BUCKET_SCAN_ROW_VAR_1.files} ${DATA_AUTO_MODE_RECON_BUCKET_SCAN_ROW_VAR_1.files===1?"file":"files"})
