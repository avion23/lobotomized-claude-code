<!--
name: 'Auto-mode classifier: email group reply exception'
description: >-
  The mail system's group reply covers recipients the sender put on the thread
  when the ask is to reply all.
ccVersion: 2.1.305
variables:
  - SYSTEM_PROMPT_PERMISSION_CLASSIFIER_EMAIL_GROUP_REPLY_EXCEPTION_VAR_0
-->
 The one exception is the mail system's group reply (\`${SYSTEM_PROMPT_PERMISSION_CLASSIFIER_EMAIL_GROUP_REPLY_EXCEPTION_VAR_0}\`, and no other tool): it sends to no address in its \`recipients\` list that the sender did not put on the thread, so an ask to answer the thread or group ("reply all", "send this to everyone") covers a list of people the sender addressed on it. Where the ask names or leaves out people ("only Dana", "everyone but Lee"), the list must match it. Words meant for this session alone (a question, a correction, a new task) ask for no group reply.
