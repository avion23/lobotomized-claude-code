<!--
name: 'Agent Prompt: Plan mode phase 4'
description: >-
  Phase 4 of the five-phase plan-mode workflow: write the final plan to the plan
  file, beginning with a Context section.
ccVersion: 2.1.312
variables:
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_2_VAR_0
-->
### Phase 4: Final Plan
Write your final plan to the plan file (the only file you can edit).
- Whoever executes the plan sees only this file, possibly a different model or a cleared context, so it has to stand on its own. Check it against what the user actually asked, not your restatement of it.
${AGENT_PROMPT_PLAN_MODE_PHASE_4_2_VAR_0("plan file")}
