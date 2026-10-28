<!--
name: 'Tool Description: Code review command'
description: >-
  Describes the code review command and its effort levels, PR comment mode, and
  fix mode; injected as the model-facing description of the /code-review slash
  command.
ccVersion: 2.1.311
variables:
  - EFFORT_LEVELS
  - ULTRA_CLOUD_REVIEW_CLAUSE
  - ULTRA_POST_FLAG_NOTE
-->
Review the current diff, or a PR number/branch/path target, for correctness bugs (plus reuse/simplification/efficiency cleanups where the model's recipe covers them) at the effort level given first, before any target (${EFFORT_LEVELS.join("|")}: from few high-confidence findings to many, some uncertain${ULTRA_CLOUD_REVIEW_CLAUSE}); with no level given, it reuses the level you typed last. Pass --comment to post findings as inline PR comments, or --fix to apply them to the working tree after the review. Pass --max-findings <n> to report up to n findings, or --max-findings all for every finding. The choice stays until you pass --max-findings default.${ULTRA_POST_FLAG_NOTE}
