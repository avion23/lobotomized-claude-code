<!--
name: 'Plugin validate: MCP config symlink'
description: 'Finding: MCP config is a symlink or not a regular file.'
ccVersion: 2.1.305
-->
MCP config is a symlink, goes through one, or is not a regular file and was not read. The loader reads it anyway, so none of its servers were checked.
