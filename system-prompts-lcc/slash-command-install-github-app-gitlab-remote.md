<!--
name: 'Slash Command: /install-github-app — GitLab remote'
description: >-
  Tells the model the GitHub App cannot be installed because the repository's
  git remote is on GitLab, and where to read about GitLab CI/CD.
ccVersion: 2.1.296
variables:
  - SLASH_COMMAND_INSTALL_GITHUB_APP_GITLAB_REMOTE_VAR_0
-->
The Claude GitHub App only works with GitHub repositories, and this repository's git remote is on GitLab. To run Claude Code from GitLab CI/CD instead, see ${SLASH_COMMAND_INSTALL_GITHUB_APP_GITLAB_REMOTE_VAR_0}. To install the app for a GitHub repository, run /install-github-app from a checkout of that repository.
