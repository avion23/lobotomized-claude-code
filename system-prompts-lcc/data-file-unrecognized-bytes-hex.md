<!--
name: 'Data: file content — unrecognized bytes (hex: …)'
description: Read image-type mismatch diagnostic describing the detected nonimage bytes.
ccVersion: 2.1.296
variables:
  - DATA_FILE_UNRECOGNIZED_BYTES_HEX_VAR_0
-->
unrecognized bytes (hex: ${DATA_FILE_UNRECOGNIZED_BYTES_HEX_VAR_0.subarray(0,8).toString("hex").replace(/(..)/g,"$1 ").trim()})
