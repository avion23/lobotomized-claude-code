<!--
name: CLAUDE_CONFIG_DIR relative path note
description: >-
  Suffix explaining that an empty or relative CLAUDE_CONFIG_DIR widened the
  protected-folder check.
ccVersion: 2.1.300
variables:
  - TOOL_RESULT_CONFIG_DIR_RELATIVE_PATH_NOTE_VAR_0
-->
${TOOL_RESULT_CONFIG_DIR_RELATIVE_PATH_NOTE_VAR_0.message} CLAUDE_CONFIG_DIR is empty or relative here, so the config directory is worked out from each of three folders: the current one, the one where Claude Code was started and the home folder. That may be the only reason this path counts. Unset CLAUDE_CONFIG_DIR or set it to an absolute path to avoid that.
