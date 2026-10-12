<!--
name: 'Auto-mode recon: sensitive paths'
description: >-
  Sensitive-looking paths (filename scan) subsection of the config-scan recon
  section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_0
  - DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_1
  - DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_2
-->

#### Sensitive-looking paths (filename scan)
${DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_0.map((DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_1)=>`- ${DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_2(DATA_AUTO_MODE_RECON_SENSITIVE_PATHS_VAR_1)}`).join(`
`)}
