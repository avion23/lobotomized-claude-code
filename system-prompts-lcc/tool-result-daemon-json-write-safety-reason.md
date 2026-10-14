<!--
name: daemon.json write safety reason
description: Safety-check reason for writes to daemon.json.
ccVersion: 2.1.300
-->
This writes to the Claude Code daemon.json, or to a file that stands in for it. The service that runs background sessions starts the workers listed there without asking anyone.
