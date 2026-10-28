<!--
name: 'Tool Result: Artifact publish stale version guard'
description: >-
  Artifact tool error when an earlier same-turn read returned only a summary of
  a newer version.
ccVersion: 2.1.312
-->
A read earlier in this same turn recorded this artifact's newer live version but returned only a summary of it, not its source, so nothing was published. 
