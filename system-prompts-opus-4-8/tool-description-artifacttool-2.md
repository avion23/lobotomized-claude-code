<!--
name: 'Tool Description: ArtifactTool'
description: >-
  Tool description for ArtifactTool — renders an HTML or Markdown file to a
  default-private hosted web page on claude.ai
ccVersion: 2.1.183
-->
Render an HTML or Markdown file to an Artifact — a default-private web page hosted on claude.ai that the user can later choose to share with teammates. Use this when an image, diagram, or rich HTML/Markdown would communicate more clearly than terminal text.

Write the content to a file first (via Write/Edit), then call Artifact with its path. The file is wrapped in a `<!doctype html>…<head>…</head><body>` skeleton at publish time, so write the page content directly — no `<!DOCTYPE>`, `<html>`, `<head>`, or `<body>` tags of your own. Unless the user names a location, put the file in your scratchpad directory if one is listed in your system prompt.

**Content**: Disclose progressively — high level first, supporting detail underneath. The reader wasn't in the session, so what's obvious from the transcript isn't obvious to them.

**Title**: Set a concise `<title>` in the HTML — it names the artifact in the browser tab, gallery, and lists. Keep it stable across redeploys unless the page's purpose changes; files without one fall back to the basename, so pick a short, distinctive filename (e.g. `token-usage.html`).

**To update**: Edit the file, then call Artifact again with the same path — it redeploys to the same URL. A different path mints a new URL, so only change it to create a separate Artifact.

**To update an artifact the user gives you a URL for** (a link not published in this session): pass the URL as `url`. Without it, a fresh session always mints a new URL — there is no other way to target an existing one.

**To read an existing artifact's content**: call WebFetch with its URL.

**Self-contained only**: A strict CSP blocks every external host — CDN scripts, external stylesheets, fonts, remote images, fetch/XHR/WebSockets. Blocked resources render without erroring. Relative paths won't resolve. Inline all CSS/JS, use system font stacks, and embed assets as data: URIs.

**Responsive**: The viewport could be mobile or desktop. Use relative units (%, vw/vh, em), flexbox/grid, and `max-width:100%` on images. Wrap wide content (tables, diagrams, code blocks) in an `overflow-x: auto` div; the page body must never scroll horizontally.

**Favicon** (required): Pass one or two emoji as `favicon` (e.g. `"📊"`, `"⚡🔥"`) — emoji only, no SVG or markup. Keep it the same across redeploys; users find their tab by its icon. Pick a new emoji only on a hard pivot in what the artifact is about.
