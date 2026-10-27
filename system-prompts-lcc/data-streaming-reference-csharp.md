<!--
name: 'Data: Streaming reference — C#'
description: >-
  claude-api skill reference file (Streaming reference — C#) inlined as <doc> or
  extracted for the model to Read when the skill's Reading Guide points to it.
ccVersion: 2.1.311
-->
# Streaming - C#

## Streaming

\`\`\`csharp
using Anthropic.Models.Messages;

var parameters = new MessageCreateParams
{
    Model = "{{OPUS_ID}}",
    MaxTokens = 64000,
    Messages = [new UserMessageParam { Content = "Write a haiku" }]
};

await foreach (RawMessageStreamEvent streamEvent in client.Messages.CreateStreaming(parameters))
{
    if (streamEvent.TryPickContentBlockDelta(out var delta) &&
        delta.Delta.TryPickText(out var text))
    {
        Console.Write(text.Text);
    }
}
\`\`\`

**\`RawMessageStreamEvent\` TryPick methods** (naming drops the \`Message\`/\`Raw\` prefix): \`TryPickStart\`, \`TryPickDelta\`, \`TryPickStop\`, \`TryPickContentBlockStart\`, \`TryPickContentBlockDelta\`, \`TryPickContentBlockStop\`. There is no \`TryPickMessageStop\` - use \`TryPickStop\`.

---

