<!--
name: 'Tool Result: Memory write refused for non-main agent'
description: >-
  Tells a subagent, teammate, fork, or backgrounded query it cannot change the
  user's account memory itself, and that it should say what should be saved so
  the main agent can save it
ccVersion: 2.1.284
-->
Only the session's main agent can change the user's account memory; a subagent, teammate, fork or backgrounded query cannot. If something should be saved, say so in your reply so the main agent can save it.
