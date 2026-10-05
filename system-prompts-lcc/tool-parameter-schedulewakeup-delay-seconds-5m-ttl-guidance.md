<!--
name: 'Tool Parameter: ScheduleWakeup delaySeconds (5-minute TTL guidance)'
description: >-
  ScheduleWakeup tool's 'Picking delaySeconds' guidance shown when the session's
  prompt-cache TTL is 5 minutes
ccVersion: 2.1.284
-->
## Picking delaySeconds

This session's requests use the default 5-minute Anthropic prompt-cache TTL. So the natural breakpoints:

- **Under 5 minutes (60s–270s)**: cache stays warm. Right for actively polling external state the harness can't notify you about — a CI run, a deploy, a remote queue.
- **5 minutes to 1 hour (300s–3600s)**: pay the cache miss. Right when there's no point checking sooner — waiting on something that takes minutes to change, genuinely idle, or as the long fallback heartbeat when something else is the primary wake signal.

**Don't pick 300s.** It's the worst-of-both: you pay the cache miss without amortizing it.

For idle ticks with no specific signal to watch, default to **1200s–1800s** (20–30 min).

If you're polling a CI run that takes ~8 minutes, sleeping 60s burns the cache 8 times before it finishes — sleep ~270s twice instead.

The runtime clamps to [60, 3600], so you don't need to clamp yourself.
