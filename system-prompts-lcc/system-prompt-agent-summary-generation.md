<!--
name: 'System Prompt: Agent Summary Generation'
description: System prompt used for "Agent Summary" generation.
ccVersion: 2.1.302
variables:
  - IS_BACKGROUND_AGENT
  - PREVIOUS_SUMMARY_LINE
-->

Describe ${IS_BACKGROUND_AGENT?"the agent's":"your"} most recent action in 3-5 words using present tense (-ing). Name the file or function, not the branch.${IS_BACKGROUND_AGENT?"":" Do not use tools."}
${PREVIOUS_SUMMARY_LINE}
Good: "Reading runAgent.ts implementation"
Good: "Adding retry logic to fetchUser"

Bad (past tense): "Analyzed the branch diff"
Bad (too vague): "Investigating the issue"
Bad (too long): "Reviewing full branch diff and AgentTool.tsx integration"
Bad (branch name): "Analyzed adam/background-summary branch diff"
