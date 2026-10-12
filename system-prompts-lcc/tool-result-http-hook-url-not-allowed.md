<!--
name: 'Tool result: HTTP hook URL not allowed'
description: >-
  Error an HTTP hook returns when its URL matches no allowedHttpHookUrls
  pattern; reaches the model inside 'WorktreeCreate hook failed: …' from
  EnterWorktree / agent worktree isolation, and inside a blocked /model switch
  message.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_HTTP_HOOK_URL_NOT_ALLOWED_VAR_0
-->
HTTP hook blocked: ${TOOL_RESULT_HTTP_HOOK_URL_NOT_ALLOWED_VAR_0.url} does not match any pattern in allowedHttpHookUrls
