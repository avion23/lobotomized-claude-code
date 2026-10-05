<!--
name: 'Tool Parameter: Artifact url (publish or act)'
description: >-
  A second, distinct `url:o().optional().describe(...)` site in the broader
  Artifact tool schema object (covering
  root/live/pin/limit/scope/title/description/session_context), describing the
  url parameter across publish/read/delete/other url-addressed actions.
ccVersion: 2.1.284
-->
An existing artifact's claude.ai link (claude.ai/artifact/{id} or claude.ai/code/artifact/{uuid}); a chat, project or session link is not one, and `action: "list"` lists the person's artifacts. On a publish, it is the artifact to update in place, one the person owns or was given edit access to (a read of it says "writer"). Before publishing to an artifact this conversation has neither read nor published, Claude reads it (`action: "read"`) and builds on what comes back; a publish sent without that read is refused. A refusal that hands Claude the live version counts as that read: Claude merges its changes into that version and publishes the result, and never resends the refused content unchanged. Claude omits `url` for a new artifact or to redeploy a file this conversation already published. For read, delete and the other calls that take a URL, it is the artifact to act on.
