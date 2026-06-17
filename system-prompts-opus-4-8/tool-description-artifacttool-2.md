<!--
name: 'Tool Description: ArtifactTool'
description: >-
  Tool description for ArtifactTool — renders an HTML or Markdown file to a
  default-private hosted web page on claude.ai
ccVersion: 2.1.178
-->
Render an HTML or Markdown file to an Artifact — a default-private web page hosted on claude.ai that the user can share. Use it when a visual (image, diagram, rich HTML/Markdown) communicates better than terminal text.

Write the content to a file first (Write/Edit), then call Artifact with its path. The file is wrapped in a `<!doctype html>…<head>…</head><body>` skeleton at publish time, so write the page content directly — no `<!DOCTYPE>`, `<html>`, `<head>`, or `<body>` tags of your own. Unless the user names a location, put the file in your scratchpad directory if one is listed in your system prompt.

Set a concise `<title>` — it names the artifact in the tab, gallery, and lists; files without one fall back to the basename, so pick a short, distinctive filename.

To update, call Artifact again with the same file path — it redeploys to the same URL; a different path mints a new URL. To update an artifact the user gives you a URL for (not published this session), pass the URL as `url`. To read an existing artifact, call WebFetch with its URL.

**Self-contained only**: a strict CSP blocks all external hosts — CDN scripts, external stylesheets, fonts, remote images, fetch/XHR/WebSockets — and relative paths won't resolve. Blocked resources don't error; the page just renders without them. Inline all CSS/JS and embed assets as `data:` URIs. System font stacks are fine.

**Responsive**: viewport is unknown (mobile or desktop). Wide content (tables, diagrams, code blocks) must scroll inside its own `overflow-x: auto` container; the page body must never scroll horizontally.

**Favicon** (required): pass one or two emoji as `favicon` (e.g. `"📊"`, `"⚡🔥"`) — emoji only, no SVG or markup. It becomes the browser-tab icon; keep it stable across redeploys.
