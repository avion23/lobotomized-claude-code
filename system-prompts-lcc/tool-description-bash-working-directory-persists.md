<!--
name: 'Tool Description: Bash working directory persists'
description: >-
  Bash prompt bullet: working directory persists, prefer absolute paths over cd,
  shell state does not persist
ccVersion: 2.1.301
-->
- Your working directory persists between calls. In general you should prefer absolute paths, because using `cd` in a compound command could trigger a permission prompt for the user. Shell state, such as env vars and functions, does not persist - the shell has been initialized from the user's profile.
