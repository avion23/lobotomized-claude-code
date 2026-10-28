<!--
name: Artifact root parameter
description: Describes root as the base directory for relative files sources
ccVersion: 2.1.310
variables:
  - TOOL_PARAMETER_ARTIFACT_ROOT_2_VAR_0
-->
The base directory that relative \`files\` sources resolve against, like a bundler root. ${TOOL_PARAMETER_ARTIFACT_ROOT_2_VAR_0.typesOn?"It never changes the published path of a `files` entry":"It never changes published paths"}. It is relative to the working directory, or absolute within it or within Claude's scratchpad directory.
