<!--
name: 'Data: sandbox.allowNestedUserNamespaces setting description (part 2 of 5)'
description: >-
  Description of the `sandbox.allowNestedUserNamespaces` setting in Claude
  Code's settings JSON schema. The model reads it through /update-config and
  settings validation errors; it is also shown to users in the settings help.
ccVersion: 2.1.305
-->
**Removes code-execution isolation** — in any folder a hostile command may write, it can then bypass filesystem.denyWrite, filesystem.denyRead, credentials.files entries and the paths the sandbox always write-protects (such as .claude/settings.json, git hooks and git config), 
