<!--
name: 'Sandbox install: config conflict'
description: >-
  A filter set with a different configuration is installed; how to remove it and
  reinstall.
ccVersion: 2.1.308
-->
A sandbox network-filter set is already installed with a different configuration: under a different sandbox account name, or with the other setting for local connections (sandbox.network.allowLocalBinding) while its state could not be read. Run /sandbox install again; if it is refused again, close every Claude Code session and run claude sandbox uninstall in a terminal, then run /sandbox install.
