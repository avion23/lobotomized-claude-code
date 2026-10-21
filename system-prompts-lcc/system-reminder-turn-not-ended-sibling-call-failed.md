<!--
name: 'System Reminder: turn not ended because a sibling call failed'
description: >-
  Meta message telling the model its end-turn call did not take effect because
  another call in the same message failed
ccVersion: 2.1.301
-->
The turn did not end: a tool call in your last message asked to end it, but another call in that message failed. Deal with the failure, then finish the turn. The calls that succeeded took effect, so do not repeat them.
