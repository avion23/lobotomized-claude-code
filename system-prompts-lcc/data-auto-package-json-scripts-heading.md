<!--
name: Auto-mode package script list
description: >-
  Auto-mode package script list. Emitted by the concrete model-context route
  documented below.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_0
  - DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_1
  - DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_2
-->

#### package.json scripts
${DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_0.map((DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_1)=>`- ${DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_2(DATA_AUTO_PACKAGE_JSON_SCRIPTS_HEADING_VAR_1)}`).join(`
`)}
