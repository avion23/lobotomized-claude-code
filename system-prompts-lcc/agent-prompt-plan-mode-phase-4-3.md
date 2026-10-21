<!--
name: 'Agent Prompt: Plan mode phase 4'
description: >-
  Phase 4 of the five-phase plan-mode workflow: write the final plan to the plan
  file, beginning with a Context section.
ccVersion: 2.1.304
variables:
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_0
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_1
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_2
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_3
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_4
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_5
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_6
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_7
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_8
-->
${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_0("")}

## Where Your Plan Goes:
This session has no plan file. ${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_1?`Pass your plan to ${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_2} as its \`plan\` argument`:"Give your plan to the user as text in your reply"}, and do not write it to a file.

## Plan Workflow

${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_3}

${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_4}

${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_5}

### Phase 4: Final Plan
Goal: ${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_1?"Settle your final plan.":"Give your final plan in your reply."}
${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_6("plan")}

### Phase 5: ${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_1?`Call ${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_2}`:"Hand Over To The User"}
${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_7("full")}

${AGENT_PROMPT_PLAN_MODE_PHASE_4_3_VAR_8}
