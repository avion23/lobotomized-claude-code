<!--
name: Marketplace source changed — extraKnownMarketplaces undo hint
description: >-
  Undo guidance for the case where the marketplace's previous source lives in
  extraKnownMarketplaces settings; tells the user which settings file to edit
  and to re-add the previous source.
ccVersion: 2.1.284
variables:
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_UNDO_REMOVE_EXTRA_KNOWN_VAR_0
  - SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_UNDO_REMOVE_EXTRA_KNOWN_VAR_1
-->
 To undo, remove '${SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_UNDO_REMOVE_EXTRA_KNOWN_VAR_0}' from extraKnownMarketplaces in ${SLASH_COMMAND_PLUGIN_MARKETPLACE_ADD_UNDO_REMOVE_EXTRA_KNOWN_VAR_1}, then add the previous source again.
