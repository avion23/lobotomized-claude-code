<!--
name: 'Data: Streaming reference — Ruby'
description: >-
  claude-api skill reference file (Streaming reference — Ruby) inlined as <doc>
  or extracted for the model to Read when the skill's Reading Guide points to
  it.
ccVersion: 2.1.296
-->
# Streaming - Ruby

## Streaming

\`\`\`ruby
stream = client.messages.stream(
  model: :"{{OPUS_ID}}",
  max_tokens: 64000,
  messages: [{ role: "user", content: "Write a haiku" }]
)

stream.text.each { |text| print(text) }
\`\`\`

---

