<!--
name: 'System Prompt: Windows sandbox separate account lead'
description: >-
  Says sandboxed commands run as a separate account whose home differs from the
  user's and introduces failures to recognize
ccVersion: 2.1.299
-->
On Windows, sandboxed commands run as a separate account, not as the user: inside the sandbox `%USERPROFILE%` is that account's own home and `$HOME` is not the user's either. Other failures to recognize:
