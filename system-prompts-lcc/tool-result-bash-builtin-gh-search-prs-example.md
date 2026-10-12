<!--
name: 'Tool Result: Built-in gh Search PRs example'
description: >-
  Instead-of line in the built-in gh refusal for `gh search prs`: gh api -X GET
  search/issues -f q='<terms> is:pr'
ccVersion: 2.1.296
-->
gh api -X GET search/issues -f q='<terms> is:pr'
