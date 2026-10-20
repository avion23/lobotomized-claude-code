<!--
name: 'managed-agents-secure: local ID form refused'
description: >-
  Command not run: a local Managed Agents ID is in a form or place not accepted;
  the accepted form and what to do.
ccVersion: 2.1.305
-->
Claude Code did not run this command: it holds an ID starting agent_local_, env_local_ or vlt_local_ in a form or place that Claude Code does not accept. Claude Code accepts such an ID, which a self-hosted or local Managed Agents server makes, only in that form (agent_, env_ or vlt_, then local_01, then 22 letters and digits other than 0, O, I and l), typed in full as a word of its own in the arguments of ant itself (not after a wrapper such as timeout, and not given to another program such as echo or xargs), in a Bash command with no variables, substitutions or here-documents. If this is part of /claude-api managed-agents-secure, do not run the command again: mark each report row that needs the ID CAN'T TELL. Otherwise, if the ID came from such a server and already has that form, you may run the command again written that way; if not, do not change the ID: ask the developer where it came from.
