<!--
name: 'Slash Command: /doctor prompt-audit skill unavailable'
description: >-
  Prompt text delivered to Claude for /doctor prompt-audit when the bundled
  claude-api skill is disabled, telling it to relay that in a sentence or two
  and stop.
ccVersion: 2.1.284
-->
I ran `/doctor prompt-audit`, which hands off to the bundled claude-api skill's prompt audit. That skill is not available in this session: it is disabled, set to off in the skillOverrides setting, or turned off with every other bundled skill by the disableBundledSkills setting or CLAUDE_CODE_DISABLE_BUNDLED_SKILLS. Tell me that in a sentence or two, including that undoing whichever applies restores the audit, and stop there.
