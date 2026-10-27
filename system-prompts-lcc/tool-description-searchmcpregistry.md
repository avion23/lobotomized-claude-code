<!--
name: 'Tool Description: SearchMcpRegistry'
description: >-
  Describes the SearchMcpRegistry tool for discovering MCP connectors by
  keyword, including named-product and intent-based examples and install-state
  guidance
ccVersion: 2.1.310
-->
Search the MCP connector registry by keyword. Call this when connecting to an MCP server might help complete the task — whether or not the user named a specific product.

Returns a ranked list with directoryUuid, name, description, sample tool names, installState (org-level), and enabledInChat (this session). Results include the org's custom connectors (ones the org configured that are not in the public directory) when they match the keywords. enabledInChat: false with installState: "connected" means the connector's tools are not loaded in this session, so you cannot call them; the field does not say why. There may be no connector setting for this chat alone. If the request needs the connector, tell the user it is not available here and that they can check it, and its tool permissions, in their claude.ai connector settings.
