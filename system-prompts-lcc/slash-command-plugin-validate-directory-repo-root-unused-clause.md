<!--
name: 'Plugin validate: repo-root files unused clause'
description: 'Clause: no repository-root README or license was used.'
ccVersion: 2.1.305
variables:
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNUSED_CLAUSE_VAR_0
  - SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNUSED_CLAUSE_VAR_1
-->
so no README or license at a repository root was used${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNUSED_CLAUSE_VAR_0===void 0?"":` and the name the directory would list this folder under is not known. The directory's rules for that name (${SLASH_COMMAND_PLUGIN_VALIDATE_DIRECTORY_REPO_ROOT_UNUSED_CLAUSE_VAR_1}) were not checked`}
