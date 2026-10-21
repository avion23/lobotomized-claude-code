<!--
name: 'Tool Result: git partial clone fetchesFrom args invalid'
description: >-
  materializeWorkTree contract error describing the allowed argument shape with
  fetchesFrom
ccVersion: 2.1.301
variables:
  - TOOL_RESULT_GIT_PARTIAL_CLONE_FETCHES_FROM_ARGS_INVALID_VAR_0
-->
materializeWorkTree: with fetchesFrom, the arguments must be -c pairs if any, then fetch or ls-remote, then options, then --end-of-options, then that remote's name. Each option must carry its value after '=' (--depth=1), begin with --no-, or be one of ${[...TOOL_RESULT_GIT_PARTIAL_CLONE_FETCHES_FROM_ARGS_INVALID_VAR_0].join(", ")}. A fetch needs --no-recurse-submodules. No option may begin with --rec.
