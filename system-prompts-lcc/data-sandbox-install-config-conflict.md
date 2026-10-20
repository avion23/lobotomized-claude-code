<!--
name: 'Sandbox install: config conflict'
description: >-
  A filter set with a different configuration is installed; how to remove it and
  reinstall.
ccVersion: 2.1.305
-->
A sandbox network-filter set is already installed with a different configuration: under a different sandbox account name, or with the other setting for local connections (sandbox.network.allowLocalBinding) while its state could not be read. Run /sandbox install again; if it is refused again, remove the existing set by running npx @anthropic-ai/sandbox-runtime windows-uninstall from a trusted directory, then run /sandbox install.
