<!--
name: 'Tool Result: CA certs no usable authority and no built-in roots'
description: >-
  Error when no usable CA certificate was found and the runtime has no built-in
  roots, naming SSL_CERT_FILE, SSL_CERT_DIR and CLAUDE_CODE_CERT_STORE
ccVersion: 2.1.311
-->
No certificate authority to trust: no usable CA certificate was found (none could be read, every one had expired, or the claude-code-server host handed none), and this runtime has no built-in root certificates. Check the CA files this process reads (SSL_CERT_FILE, SSL_CERT_DIR) and CLAUDE_CODE_CERT_STORE; NODE_EXTRA_CA_CERTS only adds to those and does not count on its own.
