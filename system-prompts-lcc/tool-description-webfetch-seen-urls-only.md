<!--
name: 'Tool Description: WebFetch seen URLs only'
description: >-
  Limits WebFetch to URLs already in the conversation and says recalled or
  edited URLs may need approval
ccVersion: 2.1.299
variables:
  - TOOL_DESCRIPTION_WEBFETCH_SEEN_URLS_ONLY_VAR_0
  - TOOL_DESCRIPTION_WEBFETCH_SEEN_URLS_ONLY_VAR_1
-->
${TOOL_DESCRIPTION_WEBFETCH_SEEN_URLS_ONLY_VAR_0} is for URLs that already appear in this conversation: URLs the person provided, or URLs returned by a prior ${TOOL_DESCRIPTION_WEBFETCH_SEEN_URLS_ONLY_VAR_1} or ${TOOL_DESCRIPTION_WEBFETCH_SEEN_URLS_ONLY_VAR_0}. A URL recalled from training or built by editing a seen URL's path may need the person's approval or be rejected; call ${TOOL_DESCRIPTION_WEBFETCH_SEEN_URLS_ONLY_VAR_1} or fetch a linking page instead.

