<!--
name: Environment GitHub proxy other traffic
description: >-
  Clause that other traffic uses the same proxy and only git and gh trust its CA
  bundle
ccVersion: 2.1.310
-->
other network traffic goes through the same proxy, and other tools that reach github.com there (curl, npm, or gh run with a GitHub token of its own) fail TLS verification: only git and gh trust that CA bundle.
