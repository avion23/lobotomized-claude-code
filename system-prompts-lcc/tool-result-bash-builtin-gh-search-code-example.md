<!--
name: 'Tool Result: Built-in gh Search code example'
description: >-
  Instead-of line in the built-in gh refusal for `gh search code`: gh api -X GET
  search/code -f q='<terms> repo:<owner>/<repo>'
ccVersion: 2.1.296
-->
gh api -X GET search/code -f q='<terms> repo:<owner>/<repo>'
