<!--
name: 'Data: Message Batches API reference — PHP'
description: >-
  claude-api skill reference file (Message Batches API reference — PHP) inlined
  as <doc> or extracted for the model to Read when the skill's Reading Guide
  points to it.
ccVersion: 2.1.296
-->
# Message Batches - PHP

## Message Batches API

\`\`\`php
$batch = $client->messages->batches->create(requests: [
    ['customId' => 'req-1', 'params' => ['model' => '{{OPUS_ID}}', 'maxTokens' => 1024, 'messages' => [...]]],
    ['customId' => 'req-2', 'params' => [...]],
]);
// Poll $client->messages->batches->retrieve($batch->id) until processingStatus === 'ended',
// then iterate $client->messages->batches->results($batch->id).
\`\`\`

---

