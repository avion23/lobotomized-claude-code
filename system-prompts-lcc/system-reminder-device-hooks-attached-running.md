<!--
name: Device hooks from attached machine running
description: >-
  Additional context telling the model hooks from an attached machine are
  running.
ccVersion: 2.1.296
variables:
  - SYSTEM_REMINDER_DEVICE_HOOKS_ATTACHED_RUNNING_VAR_0
  - SYSTEM_REMINDER_DEVICE_HOOKS_ATTACHED_RUNNING_VAR_1
-->
Hooks from a machine the user attached are running.${SYSTEM_REMINDER_DEVICE_HOOKS_ATTACHED_RUNNING_VAR_0>=SYSTEM_REMINDER_DEVICE_HOOKS_ATTACHED_RUNNING_VAR_1?" Later changes are not announced.":""}
