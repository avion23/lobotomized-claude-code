<!--
name: 'Agent Prompt: /review-pr slash command'
description: >-
  System prompt for reviewing a GitHub pull request — gather the PR diff via gh,
  scope to the PR diff only
ccVersion: 2.1.186
variables:
  - AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_0
  - AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_1
  - AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_2
-->
Review target: GitHub pull request \`${AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_0}\`.

Gather the diff (not a local \`git diff\`): \`gh pr view ${AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_0} --json title,body,author,baseRefName,headRefName,state,additions,deletions,changedFiles,labels\` for context, then \`gh pr diff ${AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_0}\` for the unified diff. The PR's diff is the only review scope — local working-tree changes are out of scope. When an angle needs surrounding code, Read it from this checkout if the branch matches, otherwise fetch via \`gh\`.

${AGENT_PROMPT_REVIEW_PR_SLASH_COMMAND_VAR_2}

## Present the review

After the final phase, don't reply with the raw JSON findings array. Give a 2-3 sentence overview of what the PR does, then the surviving findings most-severe first as \`file:line — summary (failure scenario)\`.
