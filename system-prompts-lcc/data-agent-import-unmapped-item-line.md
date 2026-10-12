<!--
name: '/import headless: unmapped item line'
description: >-
  Line listing a foreign config item with no automatic mapping and the reason,
  in the headless /import scan summary.
ccVersion: 2.1.296
variables:
  - DATA_AGENT_IMPORT_UNMAPPED_ITEM_LINE_VAR_0
  - DATA_AGENT_IMPORT_UNMAPPED_ITEM_LINE_VAR_1
-->
- ${DATA_AGENT_IMPORT_UNMAPPED_ITEM_LINE_VAR_0(DATA_AGENT_IMPORT_UNMAPPED_ITEM_LINE_VAR_1.label)} — ${DATA_AGENT_IMPORT_UNMAPPED_ITEM_LINE_VAR_1.reason}
