<!--
name: No certificate authority to trust
description: >-
  Error that CLAUDE_CODE_CERT_STORE=system or --use-system-ca leaves no trusted
  roots and NODE_EXTRA_CA_CERTS alone does not count
ccVersion: 2.1.310
variables:
  - TOOL_RESULT_CA_CERTS_NO_AUTHORITY_TO_TRUST_VAR_0
-->
No certificate authority to trust: CLAUDE_CODE_CERT_STORE=system (or NODE_OPTIONS --use-system-ca or --use-openssl-ca) leaves out the runtime's bundled roots, and ${TOOL_RESULT_CA_CERTS_NO_AUTHORITY_TO_TRUST_VAR_0}. NODE_EXTRA_CA_CERTS only adds to the store; it does not count on its own.
