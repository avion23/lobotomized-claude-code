<!--
name: 'Data: Streaming reference — PHP'
description: >-
  claude-api skill reference file (Streaming reference — PHP) inlined as <doc>
  or extracted for the model to Read when the skill's Reading Guide points to
  it.
ccVersion: 2.1.311
-->
# Streaming - PHP

> **Requires SDK v0.5.0+.** v0.4.0 and earlier used a single \`$params\` array; calling with named parameters throws \`Unknown named parameter $model\`. Upgrade: \`composer require "anthropic-ai/sdk"\`

\`\`\`php
use Anthropic\\Messages\\RawContentBlockDeltaEvent;
use Anthropic\\Messages\\TextDelta;

$stream = $client->messages->createStream(
    model: '{{OPUS_ID}}',
    maxTokens: 64000,
    messages: [
        ['role' => 'user', 'content' => 'Write a haiku'],
    ],
);

foreach ($stream as $event) {
    if ($event instanceof RawContentBlockDeltaEvent && $event->delta instanceof TextDelta) {
        echo $event->delta->text;
    }
}
\`\`\`

---

