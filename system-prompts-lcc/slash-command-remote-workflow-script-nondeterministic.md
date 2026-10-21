<!--
name: 'Slash Command: Remote Workflow Script Nondeterministic'
description: >-
  Result line when a remote-launched workflow script uses Date.now(),
  Math.random() or new Date(), which break resume.
ccVersion: 2.1.302
-->
workflow scripts must be deterministic: Date.now()/Math.random()/new Date() are unavailable (breaks resume). Stamp results after the workflow returns, or pass timestamps via args.
