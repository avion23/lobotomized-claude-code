<!--
name: 'Data: Artifact runtime capability declarations'
description: >-
  Defines Artifact runtime capability declaration, carry-forward, clearing,
  replacement, and contract pinning semantics; injected into the Artifact
  capabilities skill.
ccVersion: 2.1.284
-->
# Artifact runtime capabilities

A published Artifact page can declare **runtime capabilities** — abilities the claude.ai viewer grants the page at open time — by passing `capabilities: {name: config}` to the Artifact tool. The control plane is the authority on valid names and config shapes. A **non-empty object** is a full-set declaration: anything stored but not restated is revoked. Carrying a declaration forward (omitting `capabilities` on redeploy) preserves the artifact's stored contract pin.

**A page that republishes itself** through the `artifact` capability sends its whole document in exactly the shape the Artifact tool publishes, so a later publish from the tool recognizes and replaces the skeleton instead of nesting it: `<!doctype html><html><head><meta charset=utf8><meta name=viewport content="width=device-width,initial-scale=1,viewport-fit=cover"><style>` the same small reset the tool's description names `</style></head><body>` — no whitespace between those tags and nothing else in the head — then the page content exactly as it was written for the tool (its `<title>` and `<style>` first, inside the body, regenerated from the page's state), then `</body></html>`.
