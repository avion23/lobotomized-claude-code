<!--
name: 'Auto-mode recon: default soft-deny labels'
description: >-
  Default soft-deny labels subsection of the shipped default auto-mode rule
  labels recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_0
  - DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_1
  - DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_2
-->

#### Default soft-deny labels
${DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_0(DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_1.soft_deny).map((DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_2)=>`- ${DATA_AUTO_MODE_RECON_DEFAULT_SOFT_DENY_LABELS_VAR_2}`).join(`
`)}
