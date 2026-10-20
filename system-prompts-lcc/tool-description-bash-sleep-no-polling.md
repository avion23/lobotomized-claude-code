<!--
name: 'Tool Description: Bash (sleep — no polling background tasks)'
description: 'Bash tool instruction: do not poll background tasks, wait for notification'
ccVersion: 2.1.304
variables:
  - ARE_BACKGROUND_SHELLS_KEPT_ELSEWHERE
-->
If waiting for a background task you started with \`run_in_background\`, you will be notified ${ARE_BACKGROUND_SHELLS_KEPT_ELSEWHERE?"if it completes while you are still working":"when it completes"} — do not poll.
