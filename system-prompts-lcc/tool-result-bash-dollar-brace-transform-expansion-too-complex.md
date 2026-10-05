<!--
name: 'Bash: ${…@P} transform expansion too complex'
description: >-
  Shell-parse failure for a ${...@P} parameter-transform expansion (runs what
  the variable holds); routed through the same unreadable/wo() pipeline as the
  ambiguous-brace case.
ccVersion: 2.1.284
-->
a ${ …@P } expansion, which runs what the variable holds and this reading cannot follow
