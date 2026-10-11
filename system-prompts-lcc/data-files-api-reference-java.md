<!--
name: 'Data: Files API reference — Java'
description: >-
  claude-api skill reference file (Files API reference — Java) inlined as <doc>
  or extracted for the model to Read when the skill's Reading Guide points to
  it.
ccVersion: 2.1.296
-->
# Files API - Java

## Files API

> **Out of beta.** In current SDKs \`client.beta().files()\` has breaking shape changes from previous versions, matching the stable \`client.files()\` - migrate per the Files API row in \`shared/live-sources.md\`. Examples below predate this.

Under \`client.beta().files()\`. File references in messages need the beta message types (non-beta \`DocumentBlockParam.Source\` has no file-ID variant).

\`\`\`java
import com.anthropic.models.beta.files.FileUploadParams;
import com.anthropic.models.beta.files.FileMetadata;
import com.anthropic.models.beta.messages.BetaRequestDocumentBlock;
import com.anthropic.models.beta.messages.BetaFileDocumentSource;
import java.nio.file.Paths;

FileMetadata meta = client.beta().files().upload(
    FileUploadParams.builder()
        .file(Paths.get("/path/to/doc.pdf"))  // or .file(InputStream) or .file(byte[])
        .build());

// Reference in a beta message:
BetaRequestDocumentBlock doc = BetaRequestDocumentBlock.builder()
    .source(BetaFileDocumentSource.builder().fileId(meta.id()).build())
    .build();
\`\`\`

Other methods: \`.list()\`, \`.delete(String fileId)\`, \`.download(String fileId)\`, \`.retrieveMetadata(String fileId)\`.
