<!--
name: 'Tool Result: CA certs all on deny list and no built-in roots'
description: >-
  Error when every CA certificate found is on the CLI deny list and the runtime
  has no built-in roots
ccVersion: 2.1.311
-->
No certificate authority to trust: every CA certificate found is on the CLI's deny list, and this runtime has no built-in root certificates. Add a certificate authority that is not on the deny list to the CA files (SSL_CERT_FILE, SSL_CERT_DIR).
