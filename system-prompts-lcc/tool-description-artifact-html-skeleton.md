<!--
name: 'Tool Description: Artifact HTML Skeleton'
description: >-
  Artifact authoring instruction that publish wraps the file in a
  doctype/head/body skeleton, so the model must not emit those tags.
ccVersion: 2.1.301
variables:
  - TOOL_DESCRIPTION_ARTIFACT_HTML_SKELETON_VAR_0
  - TOOL_DESCRIPTION_ARTIFACT_HTML_SKELETON_VAR_1
-->
The file is wrapped in a \`<!doctype html>…<head>…</head><body>\` skeleton at publish time, so write the page content directly — no \`<!DOCTYPE>\`, \`<html>\`, \`<head>\`, or \`<body>\` tags of your own. Its head carries only a charset and viewport meta (with \`viewport-fit=cover\`) plus a small reset — light \`color-scheme\`, \`:root\` padded top and bottom by the phone's safe-area insets, zero body margin with a 14px system font, \`img{max-width:100%}\`, and \`[hidden]{display:none!important}\` (toggle visibility with \`el.hidden\`, not \`style.display\`) — so put your own \`<title>\` and \`<style>\` at the top of the file. Keep the \`:root\` padding. Put \`<meta name="claude:viewport-fit-sides" content="cover">\` at the top of the file beside your \`<title>\`: it promises that the side gutter uses the two \`max()\` paddings given under Responsive, ${TOOL_DESCRIPTION_ARTIFACT_HTML_SKELETON_VAR_0} With it the page also runs under a system bar at the phone's side, where backgrounds reach that edge while the gutter keeps text and controls clear. Anything fixed to a screen edge stays at \`0\` and adds that edge's \`env(safe-area-inset-*, 0px)\` to its own padding (one that spans the width takes the side gutter too), a floating or absolutely placed control adds the nearby edges' insets to its offsets, and a sticky page header uses \`top: env(safe-area-inset-top, 0px)\`, not \`0\`, with the band above it painted by a fixed \`body::before\` (\`${TOOL_DESCRIPTION_ARTIFACT_HTML_SKELETON_VAR_1}\`) in its background, or in the page's where it starts lower.
