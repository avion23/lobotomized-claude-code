<!--
name: 'Tool Parameter: plugin_errors entry path field'
description: >-
  Schema description for the optional 'path' field on a plugin_errors entry in
  the SDK system/init message, present only when a directory or zip plugin
  source failed to load at all, giving the resolved path used to pair the error
  to its mount
ccVersion: 2.1.284
-->
Present only when a --plugin-dir, SDK `plugins` or synced directory entry did not load at all: the path of that entry, resolved against the cwd (for a directory, the value its `plugins[]` row would have carried; for a .zip, the archive; a --plugin-url entry carries none). `plugin` is then the positional `inline[N]` / `synced[N]` tag, so a host that mounts several directories pairs the error to its own by this path.
