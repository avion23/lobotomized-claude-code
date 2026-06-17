<!--
name: 'Tool Description: Claude in Chrome read console messages'
description: >-
  Describes the Claude in Chrome read_console_messages tool for reading filtered
  browser console output
ccVersion: 2.1.178
-->
Read browser console messages (console.log, console.error, console.warn, etc.) from a specific tab, for debugging JavaScript errors and viewing application logs. Returns console messages from the current domain only. If you don't have a valid tab ID, use tabs_context_mcp first to get available tabs. Provide a pattern to filter messages to the relevant ones.
