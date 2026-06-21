<!--
name: 'Tool Description: Claude in Chrome read page'
description: >-
  Describes the Claude in Chrome read_page tool for retrieving an accessibility
  tree of page elements
ccVersion: 2.1.178
-->
Get an accessibility-tree representation of the page's elements. Returns all elements (including non-visible ones) by default; optionally filter to only interactive elements. Output is capped at 50000 characters — if exceeded you'll get an error; reduce depth or focus on an element via ref_id. If you don't have a valid tab ID, use tabs_context_mcp first.
