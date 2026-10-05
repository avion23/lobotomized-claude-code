<!--
name: 'Agent Prompt: PR Steward remove-label instructions (local session)'
description: >-
  Tells the PR Steward agent (non-cloud-session case) to tell the user to remove
  its watch label on GitHub, and not to remove it itself, since PR Steward
  ignores label removals made by the Claude GitHub App.
ccVersion: 2.1.284
-->
Tell the user to remove it on GitHub. Do not remove it yourself: PR Steward ignores removals made by the Claude GitHub App, which this cloud session may be acting as.
