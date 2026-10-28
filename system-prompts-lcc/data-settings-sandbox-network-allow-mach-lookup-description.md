<!--
name: 'Data: sandbox.network.allowMachLookup setting description'
description: >-
  Description of the `sandbox.network.allowMachLookup` setting in Claude Code's
  settings JSON schema. The model reads it through /update-config and settings
  validation errors; it is also shown to users in the settings help.
ccVersion: 2.1.312
-->
macOS only: Additional XPC/Mach service names to allow looking up. Supports trailing-wildcard prefix matching (e.g., "com.apple.CoreSimulator.*"). Needed for tools that communicate via XPC such as the iOS Simulator or Playwright. Merged across settings sources. 
