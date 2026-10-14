<!--
name: 'Agent Prompt: Plan mode Phase 4 final plan'
description: 'Plan mode phase 4: write the final plan to the plan file'
ccVersion: 2.1.299
variables:
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_VAR_0
  - AGENT_PROMPT_PLAN_MODE_PHASE_4_VAR_1
-->
### Phase 4: Final Plan
Write your final plan to the plan file (the only file you can edit${AGENT_PROMPT_PLAN_MODE_PHASE_4_VAR_0?", besides the session workshop document":""}).
- Whoever executes the plan sees only this file, possibly a different model or a cleared context, so it has to stand on its own. Check it against what the user actually asked, not your restatement of it.
${AGENT_PROMPT_PLAN_MODE_PHASE_4_VAR_1("plan file")}
