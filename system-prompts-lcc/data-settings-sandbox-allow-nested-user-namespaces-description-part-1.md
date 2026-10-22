<!--
name: 'Data: sandbox.allowNestedUserNamespaces setting description (part 1 of 5)'
description: >-
  Description of the `sandbox.allowNestedUserNamespaces` setting in Claude
  Code's settings JSON schema. The model reads it through /update-config and
  settings validation errors; it is also shown to users in the settings help.
ccVersion: 2.1.308
-->
Linux/WSL only: Let sandboxed commands create user namespaces of their own, which the sandbox refuses by default. Needed by tools that sandbox themselves that way, such as Chromium's and Electron's sandbox, a nested bubblewrap, and `unshare`. 
