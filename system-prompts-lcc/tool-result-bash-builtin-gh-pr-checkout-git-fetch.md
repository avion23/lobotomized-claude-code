<!--
name: 'Tool Result: Built-in gh PR checkout git fetch'
description: >-
  Instead-of line in the built-in gh refusal for `gh pr checkout`: git fetch
  origin refs/pull/<number>/head && git checkout FETCH_HEAD
ccVersion: 2.1.296
-->
git fetch origin refs/pull/<number>/head && git checkout FETCH_HEAD
