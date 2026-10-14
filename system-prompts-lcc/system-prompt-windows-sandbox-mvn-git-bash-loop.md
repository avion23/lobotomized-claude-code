<!--
name: 'System Prompt: Windows sandbox mvn Git Bash loop'
description: >-
  Says mvn from Git Bash can loop on Permission denied and how to run it with
  MAVEN_BASEDIR
ccVersion: 2.1.299
-->
`mvn` from Git Bash can loop forever on `cd: ...: Permission denied` without starting Java. Kill it and run it as `MAVEN_BASEDIR="$PWD" mvn ...`.
