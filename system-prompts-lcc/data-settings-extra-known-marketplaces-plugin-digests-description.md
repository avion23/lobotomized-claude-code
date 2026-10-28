<!--
name: 'Data: extraKnownMarketplaces.pluginDigests setting description'
description: >-
  Description of the `extraKnownMarketplaces.pluginDigests` setting in Claude
  Code's settings JSON schema. The model reads it through /update-config and
  settings validation errors; it is also shown to users in the settings help.
ccVersion: 2.1.311
-->
Managed settings only: the plugins of this marketplace that an organization delivers with its own tier, by plugin name, each with the digests of its releases. A plugin also enabled and listed in prependPlugins or appendPlugins by managed settings the session vouches for loads its hooks module only from a folder that proves one of them, and is then seated in that tier; any other copy does not load. A digest is sha256- and the base64 SHA-256 of, for every regular file in the folder in UTF-16 code unit order of its path, not normalized, "f PATH" NUL BYTE-LENGTH NUL BYTES, with / in paths; .git, .in_use, .orphaned_at, .claude-plugin-link and .links_materialized at the root are left out. The plugin keeps its manifest at .claude-plugin/plugin.json and names one module in hooks/hooks.json. A string of any other form, or a list that is empty or of any other shape, matches no folder. A symbolic link, or a surface module, proves nothing. A proved plugin ships bundled with no install step: the digest covers the whole folder, node_modules included. A checkout whose line endings were converted proves nothing.
