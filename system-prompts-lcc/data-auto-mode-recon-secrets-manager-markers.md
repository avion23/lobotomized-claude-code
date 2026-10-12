<!--
name: 'Auto-mode recon: secrets-manager markers'
description: Secrets-manager markers subsection of the config-scan recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_SECRETS_MANAGER_MARKERS_VAR_0
  - DATA_AUTO_MODE_RECON_SECRETS_MANAGER_MARKERS_VAR_1
-->

#### Secrets-manager markers
${DATA_AUTO_MODE_RECON_SECRETS_MANAGER_MARKERS_VAR_0.map((DATA_AUTO_MODE_RECON_SECRETS_MANAGER_MARKERS_VAR_1)=>`- ${DATA_AUTO_MODE_RECON_SECRETS_MANAGER_MARKERS_VAR_1}`).join(`
`)}
