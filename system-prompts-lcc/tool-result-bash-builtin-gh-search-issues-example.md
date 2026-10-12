<!--
name: 'Tool Result: Built-in gh Search issues example'
description: >-
  Instead-of line in the built-in gh refusal for `gh search issues`: gh api -X
  GET search/issues -f q='<terms> is:issue'
ccVersion: 2.1.296
-->
gh api -X GET search/issues -f q='<terms> is:issue'
