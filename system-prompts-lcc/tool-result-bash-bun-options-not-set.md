<!--
name: 'Bash: BUN_OPTIONS could not be set'
description: >-
  Shell prefix that refuses to run the command when BUN_OPTIONS cannot be
  exported, explaining why on stderr.
ccVersion: 2.1.305
variables:
  - TOOL_RESULT_BASH_BUN_OPTIONS_NOT_SET_VAR_0
-->
{ \\builtin test -n "\${${TOOL_RESULT_BASH_BUN_OPTIONS_NOT_SET_VAR_0}-}" && \\builtin export BUN_OPTIONS="$${TOOL_RESULT_BASH_BUN_OPTIONS_NOT_SET_VAR_0}" && \\builtin unset -v ${TOOL_RESULT_BASH_BUN_OPTIONS_NOT_SET_VAR_0} || { \\builtin printf '%s\\n' 'Claude Code did not run this command: it could not set BUN_OPTIONS, which turns off automatic package installs in Bun. A read-only BUN_OPTIONS, or a CLAUDE_CODE_SHELL_PREFIX that drops the environment, can cause this.' >&2; \\builtin exit 126; }; }
