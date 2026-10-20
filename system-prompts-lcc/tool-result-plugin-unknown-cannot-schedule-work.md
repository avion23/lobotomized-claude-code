<!--
name: 'Tool Result: Unknown plugin cannot schedule work'
description: >-
  Refusal when a plugin not known in this session started the subagent, so it
  cannot schedule work that would outlive a Stop
ccVersion: 2.1.304
-->
A plugin started or resumed this subagent, or the one that spawned it, and that plugin is not known in this session. It cannot schedule work: nothing would hold that work after a Stop.
