<!--
name: 'Data: install-tools.mjs'
description: >-
  claude-test helper (skills/run/scripts/install-tools.mjs) spawned by the
  browser helper to install the browser tooling; its JSON result (ok, log,
  remedy) feeds the claude_test_browser_installed answer the model reads.
ccVersion: 2.1.310
-->


import('./lib/tools.mjs').then((tools) => {
  const result = tools.installTools();
  process.stdout.write(JSON.stringify({ ok: !!result.ok, log: String(result.log || '').slice(-20000), remedy: result.remedy || null }));
}).catch((e) => { process.stdout.write(JSON.stringify({ ok: false, log: String((e && e.message) || e) })); });
