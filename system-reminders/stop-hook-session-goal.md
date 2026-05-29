<!--
name: Stop-hook session-goal reminder
description: >-
  Fires when /goal sets a session-scoped stop hook. Carries the "do not pause to
  ask" framing. Empty .md = silent goal activation (just the condition value
  used internally).
ccVersion: 2.1.141
placeholders:
  - condition
-->
Goal active: "{{condition}}". Acknowledge, then work toward it. Stop hook blocks turn-end until the condition genuinely holds — it checks real state, so make the condition actually true rather than making output merely look complete; never suppress or flush out failing-test names or error strings to satisfy the check. If the condition is wrong, impossible, or blocked, say so to the user instead of routing around it. Auto-clears on success.
