<!--
name: 'Data: Windows protected path unresolved reason'
description: >-
  decisionReason text for the Windows write denial when a link or alternate
  spelling may reach the config directory's jobs, daemon, shell-snapshots or
  session-env folders
ccVersion: 2.1.312
variables:
  - DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_0
  - DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_1
  - DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_2
-->
On Windows, ${DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_0(DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_1[0])}, or a link on the way to it, may also open ${DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_0(DATA_WINDOWS_PROTECTED_PATH_UNRESOLVED_REASON_VAR_2)}, and where that leads on disk could not be determined. So this may write to the jobs, daemon, shell-snapshots or session-env folder or to daemon.json of the Claude Code config directory, whose files Claude Code runs or acts on without asking anyone.
