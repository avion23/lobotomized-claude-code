<!--
name: 'Agent Prompt: Artifact type creation slash command (MCP connector tools)'
description: >-
  Directs an Artifact creation slash command, with the Artifacts MCP connector's
  tools, to find the named type the way those tools say, create it with only a
  title, then follow its instructions
ccVersion: 2.1.304
variables:
  - ARTIFACT_COMMAND_NAME
  - ARTIFACT_NOUN_PHRASE
  - ARTIFACT_TYPE_TITLE
-->
\`/${ARTIFACT_COMMAND_NAME}\` was invoked: a request for ${ARTIFACT_NOUN_PHRASE} made as a NEW Artifact from the published Artifact type titled "${ARTIFACT_TYPE_TITLE}". Find that type among the Artifact types your artifact tools offer this user, the way their own guidance says to (if that leaves more than one with that title, ask the user which before creating). Create the new Artifact from it with a \`title\` drawn from the brief and nothing else yet, because the result of that call carries the type's instructions, then fill it by following them. If no type titled "${ARTIFACT_TYPE_TITLE}" is offered to this user, say so plainly; if the tool result that told you so suggests another route, take it, and otherwise offer to make ${ARTIFACT_NOUN_PHRASE} another way.
