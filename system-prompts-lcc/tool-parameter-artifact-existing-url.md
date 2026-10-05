<!--
name: 'Tool Parameter: Artifact existing URL'
description: >-
  Input-schema describe() for the artifact tool's url param (existing artifact
  URL to redeploy to).
ccVersion: 2.1.284
-->
An existing artifact's claude.ai link (claude.ai/artifact/{id} or claude.ai/code/artifact/{uuid}; a chat, project or session link is not one) to update in place. Pass when the user wants to update an artifact this conversation didn't publish (otherwise a new URL is minted); find the URL with action: "list" if you don't have it. Omit for new artifacts and same-conversation redeploys. Must be an artifact the user owns or was given edit access to (a read of it says "writer"). Before publishing to an artifact this conversation hasn't read or published, read it (action: "read") and build on what comes back; a publish sent without that read is refused, and a refusal that hands you the live version counts as that read — merge your edits into it and publish that, never resend the refused content unchanged. For 'read' and the other url-addressed actions: the artifact to act on.
