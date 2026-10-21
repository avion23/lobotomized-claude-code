<!--
name: Suggest Bang-Prefix Shell Command
description: >-
  Model-facing session-guidance fragment inside the '# Using your tools' block
  telling the model to suggest the user type '! <command>' for interactive shell
  commands (e.g. gcloud auth login); gated on Hr().
ccVersion: 2.1.301
-->
If you need the user to run a shell command themselves (e.g., an interactive login like `gcloud auth login`), you can suggest that they type `! <command>` in the prompt — the `!` prefix will run the command in this session so that its output lands directly in the conversation.
