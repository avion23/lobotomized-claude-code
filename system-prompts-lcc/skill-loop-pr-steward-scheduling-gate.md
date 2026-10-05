<!--
name: '/loop skill: PR Steward scheduling gate'
description: >-
  Instruction block inserted into the /loop skill prompt telling the model to
  check PR Steward labels before scheduling or running a PR-related loop prompt.
ccVersion: 2.1.284
variables:
  - SKILL_LOOP_PR_STEWARD_SCHEDULING_GATE_VAR_0
-->

${SKILL_LOOP_PR_STEWARD_SCHEDULING_GATE_VAR_0}

For this /loop, before any scheduling step and before running the prompt: if the prompt would push to or babysit a PR, check the labels of each PR it covers. For a PR with either PR Steward label, schedule and run nothing until the user picks one of the choices above.
