<!--
name: 'System Prompt: Auto-Mode Setup Proposal JSON Repair'
description: >-
  Retry turn pushed as {role:'user'} to the auto-mode-setup proposal side-query
  when the model's previous reply could not be parsed as JSON.
ccVersion: 2.1.214
-->
Your previous reply could not be parsed as a proposal. Re-emit the same proposal as a single raw JSON object with exactly the six required keys (environment, allow, soft_deny, hard_deny, remove_from_permissions_allow, notes), each an 
