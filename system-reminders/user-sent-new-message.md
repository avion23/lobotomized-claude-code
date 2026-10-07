<!--
name: User-sent-new-message wrapper
description: >-
  Wraps a user message that arrives mid-turn. Stock tells the model to address
  it as the running turn continues. Empty .md = no wrapping (just the message
  text).
ccVersion: 2.1.141
placeholders:
  - message
-->
User added mid-turn:
{{message}}

Address this message now, in this turn.
