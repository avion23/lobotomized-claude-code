<!--
name: Windows sandbox loopback mode changed
description: >-
  The command did not run because the sandbox was set up again with the other
  local-connections setting; tell the user to restart.
ccVersion: 2.1.305
-->
The command did not run: the sandbox on this machine was set up again with the other setting for local connections (sandbox.network.allowLocalBinding) since this session started, and a session keeps the one it started with. Every sandboxed command is refused like this one until Claude Code is restarted: tell the user to restart Claude Code.
