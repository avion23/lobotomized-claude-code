<!--
name: 'Auto-mode recon: package registry hosts'
description: Package registry hosts subsection of the config-scan recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_PACKAGE_REGISTRY_HOSTS_VAR_0
  - DATA_AUTO_MODE_RECON_PACKAGE_REGISTRY_HOSTS_VAR_1
-->
#### Package registry hosts
${DATA_AUTO_MODE_RECON_PACKAGE_REGISTRY_HOSTS_VAR_0.map((DATA_AUTO_MODE_RECON_PACKAGE_REGISTRY_HOSTS_VAR_1)=>`- ${DATA_AUTO_MODE_RECON_PACKAGE_REGISTRY_HOSTS_VAR_1}`).join(`
`)}
