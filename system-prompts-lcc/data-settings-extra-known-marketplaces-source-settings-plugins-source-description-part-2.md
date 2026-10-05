<!--
name: >-
  Data: extraKnownMarketplaces.source.(settings).plugins.source setting
  description (part 2 of 4)
description: >-
  Description of the `extraKnownMarketplaces.source.(settings).plugins.source`
  setting in Claude Code's settings JSON schema. The model reads it through
  /update-config and settings validation errors; it is also shown to users in
  the settings help.
ccVersion: 2.1.284
-->
paths have no marketplace repository to resolve against. Under allowManagedPermissionRulesOnly, a settings marketplace keeps its plugins' allowed-tools only when every npm entry here pins a `registry` on a bare package name; unpinned, the package resolves through the member's own npm config, and a non-bare spelling (an `npm:` alias, a `name@range`, a URL or git spec) packs as an 
