<!--
name: 'Auto-mode recon: default allow labels'
description: >-
  Default allow labels subsection of the shipped default auto-mode rule labels
  recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_0
  - DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_1
  - DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_2
-->

#### Default allow labels
${DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_0(DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_1.allow).map((DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_2)=>`- ${DATA_AUTO_MODE_RECON_DEFAULT_ALLOW_LABELS_VAR_2}`).join(`
`)}
