<!--
name: 'Data: Message Batches API reference — C#'
description: >-
  claude-api skill reference file (Message Batches API reference — C#) inlined
  as <doc> or extracted for the model to Read when the skill's Reading Guide
  points to it.
ccVersion: 2.1.296
-->
# Message Batches - C#

## Message Batches API

\`\`\`csharp
var batch = await client.Messages.Batches.Create(new() {
    Requests = [
        new() { CustomID = "req-1", Params = new() { Model = "{{OPUS_ID}}", MaxTokens = 1024, Messages = [...] } },
    ],
});
// Poll client.Messages.Batches.Retrieve(batch.ID) until ProcessingStatus == "ended",
// then iterate client.Messages.Batches.Results(batch.ID).
\`\`\`

