<!--
name: 'System Reminder: Attached repositories trust declined refusal'
description: >-
  Tells Claude the session's attached repositories were not marked trusted (the
  person declined the trust question), so calls to the target are refused, and
  to ask the person to answer the trust question and say what stays blocked
  until they do.
ccVersion: 2.1.284
variables:
  - SYSTEM_REMINDER_ATTACHED_REPOSITORIES_DECLINED_TRUST_REFUSAL_VAR_0
-->
This session's attached repositories were not marked trusted, so its calls to ${SYSTEM_REMINDER_ATTACHED_REPOSITORIES_DECLINED_TRUST_REFUSAL_VAR_0} are not accepted — nothing was done for this one. Sending it again will not change that: ask the person to answer the trust question, and tell them what stays blocked until they do.
