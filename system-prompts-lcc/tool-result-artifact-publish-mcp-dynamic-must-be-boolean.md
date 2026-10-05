<!--
name: 'Artifact publish: capabilities.mcp.dynamic must be boolean'
description: >-
  Error text for the dynamic_not_boolean case when capabilities.mcp.dynamic is
  set to something other than the JSON boolean true.
ccVersion: 2.1.284
-->
capabilities.mcp "dynamic" must be the JSON boolean true (or left out) — no other value is accepted, a string or a number included; with "dynamic": true the page may call connectors the declaration does not list, and "servers" may then be empty
