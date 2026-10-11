<!--
name: 'Tool Result: Built-in gh Search repos example'
description: >-
  Instead-of line in the built-in gh refusal for `gh search repos`: gh api -X
  GET search/repositories -f q='<terms>'
ccVersion: 2.1.296
-->
gh api -X GET search/repositories -f q='<terms>'
