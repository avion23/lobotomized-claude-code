<!--
name: deniedModels Ambiguous Alias Ignored
description: >-
  Explains that a deniedModels entry was ignored because it names a different
  model depending on the release/settings, and suggests naming the model
  explicitly, e.g. claude-opus-5-5.
ccVersion: 2.1.284
variables:
  - DATA_SETTINGS_DENIED_MODELS_AMBIGUOUS_NAME_IGNORED_VAR_0
  - DATA_SETTINGS_DENIED_MODELS_AMBIGUOUS_NAME_IGNORED_VAR_1
-->
"${DATA_SETTINGS_DENIED_MODELS_AMBIGUOUS_NAME_IGNORED_VAR_0(DATA_SETTINGS_DENIED_MODELS_AMBIGUOUS_NAME_IGNORED_VAR_1)}" was ignored: it names a different model depending on the release and settings. Name the model instead, for example "claude-opus-5-5".
