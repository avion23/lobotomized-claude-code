<!--
name: Git Guidance Block
description: >-
  Model-facing system-prompt `# Git` guidance block (built by Atm), listing the
  interactive-flag/gh-CLI/commit rules; gated by BFt() (git repo + git
  instructions enabled).
ccVersion: 2.1.310
variables:
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_5
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_0
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_2
  - SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_3
-->

# Git
- Interactive flags (\`-i\`, e.g. \`git rebase -i\`, \`git add -i\`) are not supported in this environment.
- Use the \`gh\` CLI for GitHub operations (PRs, issues, API).
- ${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_5}.
- Commit and push when the user or project instructions ask for it. If on the default branch, branch first.
- Immediately before a push, check whether the remote tracking branch advanced. If it did, rebase the local branch onto it; do not merge.${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_0?`
${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_0}`:""}${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1?`
- ${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_1}`:""}${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_2?`

${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_2}`:""}${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_3?`

${SYSTEM_PROMPT_GIT_GUIDANCE_BLOCK_VAR_3}`:""}
