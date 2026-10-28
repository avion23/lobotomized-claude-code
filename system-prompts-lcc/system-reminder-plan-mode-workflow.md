<!--
name: 'System Reminder: Plan mode workflow'
description: >-
  Full plan-mode workflow reminder covering plan file constraints, optional
  workshop and prototype offers, exploration, design, review, final planning,
  and approval
ccVersion: 2.1.312
variables:
  - PLAN_MODE_READONLY_INSTRUCTIONS
  - PLAN_FILE_INFO
  - PLAN_MODE_PHASE_1_INITIAL_UNDERSTANDING
  - PLAN_MODE_PHASE_2_DESIGN
  - PLAN_MODE_PHASE_3_REVIEW
  - PLAN_MODE_PHASE_4_FINAL_PLAN
  - EXIT_PLAN_MODE_TOOL_NAME
  - EXIT_PLAN_MODE_INSTRUCTIONS_FN
  - PLAN_MODE_ASK_QUESTIONS_NOTE
-->

${PLAN_MODE_READONLY_INSTRUCTIONS}

## Plan File Info:
${PLAN_FILE_INFO}
You should build your plan incrementally by writing to or editing this file.

## Plan Workflow

${PLAN_MODE_PHASE_1_INITIAL_UNDERSTANDING}

${PLAN_MODE_PHASE_2_DESIGN}

${PLAN_MODE_PHASE_3_REVIEW}

${PLAN_MODE_PHASE_4_FINAL_PLAN}

### Phase 5: Call ${EXIT_PLAN_MODE_TOOL_NAME}
${EXIT_PLAN_MODE_INSTRUCTIONS_FN("full")}

${PLAN_MODE_ASK_QUESTIONS_NOTE}
