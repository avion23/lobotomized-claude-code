<!--
name: 'Auto-mode recon: container image registries'
description: Container image registries subsection of the config-scan recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_CONTAINER_IMAGE_REGISTRIES_VAR_0
  - DATA_AUTO_MODE_RECON_CONTAINER_IMAGE_REGISTRIES_VAR_1
-->

#### Container image registries
${DATA_AUTO_MODE_RECON_CONTAINER_IMAGE_REGISTRIES_VAR_0.map((DATA_AUTO_MODE_RECON_CONTAINER_IMAGE_REGISTRIES_VAR_1)=>`- ${DATA_AUTO_MODE_RECON_CONTAINER_IMAGE_REGISTRIES_VAR_1}`).join(`
`)}
