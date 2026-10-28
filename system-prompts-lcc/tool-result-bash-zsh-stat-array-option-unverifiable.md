<!--
name: 'Tool Result: Bash zsh stat array option unverifiable'
description: >-
  Ask reason when stat -A or -H lets zsh's stat builtin store into a tracked
  variable
ccVersion: 2.1.311
-->
'stat' with -A or -H — zsh's stat builtin stores its result in the variable that option names, so a tracked value cannot be statically verified
