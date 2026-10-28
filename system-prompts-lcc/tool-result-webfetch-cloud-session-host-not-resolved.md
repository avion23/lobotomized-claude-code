<!--
name: 'Tool Result: WebFetch host not resolved in cloud session'
description: >-
  WebFetch error in a cloud session when a host fails DNS resolution, likely
  outside the allowed network domains; tells Claude to stop trying more sites
  and tell the user to allow the host
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_WEBFETCH_CLOUD_SESSION_HOST_NOT_RESOLVED_VAR_0
  - TOOL_RESULT_WEBFETCH_CLOUD_SESSION_HOST_NOT_RESOLVED_VAR_1
  - TOOL_RESULT_WEBFETCH_CLOUD_SESSION_HOST_NOT_RESOLVED_VAR_2
-->
${TOOL_RESULT_WEBFETCH_CLOUD_SESSION_HOST_NOT_RESOLVED_VAR_0.message}. In this cloud session a host fails to resolve like this when it is outside the session's allowed network domains, or does not exist. If another host has failed the same way, stop trying more sites: carry on without them, and say in your answer that ${new TOOL_RESULT_WEBFETCH_CLOUD_SESSION_HOST_NOT_RESOLVED_VAR_1(TOOL_RESULT_WEBFETCH_CLOUD_SESSION_HOST_NOT_RESOLVED_VAR_2).hostname} has to be allowed in the session's network settings. Fetch it again only once the user says it is allowed.
