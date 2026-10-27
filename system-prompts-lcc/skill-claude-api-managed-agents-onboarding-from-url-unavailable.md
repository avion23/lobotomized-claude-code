<!--
name: Claude API Managed Agents onboarding from URL unavailable
description: >-
  Section appended to the Claude API skill when its reference files could not be
  written to disk, telling Claude to say that onboarding an agent from a URL is
  unavailable, that running /claude-api again retries saving the files, and to
  stop without fetching the page or writing files
ccVersion: 2.1.310
-->
## Onboarding From a URL Unavailable

Setting up an agent from a page (`managed-agents-onboard <url>`, or a request in plain words to copy a setup from a cookbook, post or docs page) follows `shared/managed-agents-onboarding-from-url.md`, which isn't available this session. If the request is for that, tell the user it isn't possible right now because the skill's files couldn't be saved and that running `/claude-api` again will retry saving them, then stop without fetching the page or writing any files.
