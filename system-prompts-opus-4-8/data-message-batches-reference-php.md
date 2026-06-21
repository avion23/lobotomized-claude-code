<!--
name: 'Data: Message Batches reference — PHP'
description: Message Batches API reference for PHP SDK
ccVersion: 2.1.185
-->
# Message Batches — PHP

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

