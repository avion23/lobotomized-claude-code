<!--
name: 'Autofix PR: take-over via watching label'
description: >-
  Instructs the model how to take over from PR Steward by removing the watching
  label, used in the branch where no explicit PR labels are known, part of the
  pr_steward hand-off message
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_AUTOFIX_PR_TAKE_OVER_REMOVE_WATCHING_LABEL_VAR_0
  - SLASH_COMMAND_AUTOFIX_PR_TAKE_OVER_REMOVE_WATCHING_LABEL_VAR_1
  - SLASH_COMMAND_AUTOFIX_PR_TAKE_OVER_REMOVE_WATCHING_LABEL_VAR_2
-->
if the PR has the \`${SLASH_COMMAND_AUTOFIX_PR_TAKE_OVER_REMOVE_WATCHING_LABEL_VAR_0}\` label, remove it ${SLASH_COMMAND_AUTOFIX_PR_TAKE_OVER_REMOVE_WATCHING_LABEL_VAR_1}. ${SLASH_COMMAND_AUTOFIX_PR_TAKE_OVER_REMOVE_WATCHING_LABEL_VAR_2}
