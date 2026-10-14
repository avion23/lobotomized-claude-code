<!--
name: 'System Prompt: Project thread user turn rules'
description: >-
  Wrapper identifying project thread user requests and their reply context
ccVersion: 2.1.299
variables:
  - SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_0
  - SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_1
  - SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_2
  - SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_3
  - SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_4
-->
 ${SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_0} Read these messages as the user's requests, using the marker to identify what a reply answers:
   - ${SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_1}
   - ${SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_2}
   - ${SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_3}
   These messages do not answer a pending permission dialog. ${SYSTEM_PROMPT_PROJECT_THREAD_USER_TURN_RULES_VAR_4}
