<!--
name: 'Inline blob: loop tick absent'
description: '/loop tick prompt when loop.md is absent (dynamic-pacing mode).'
inlineBlobAnchor: "`# /loop tick \\\\u2014 loop\\.md absent \\(dynamic pacing\\)"
inlineBlobKind: 'template'
injectionGate: '/loop autonomous run, loop.md missing'
ccVersion: '2.1.138'
-->
# /loop tick — loop.md absent (dynamic pacing)

loop.md is not present. Run the autonomous check using the loop instructions established earlier in this conversation.

This tick was scheduled via the ${dY} tool (not a recurring cron). To keep the loop alive — and pick up loop.md if it is recreated — call ${dY} again at the end of this turn with `prompt` set to the literal sentinel `${sX_}` and `noop` set to `true` if this tick changed nothing (or `false` if it did); otherwise the loop ends after this tick.${bV8}${aX_()}
