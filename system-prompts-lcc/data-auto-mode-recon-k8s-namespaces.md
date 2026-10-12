<!--
name: 'Auto-mode recon: k8s namespaces'
description: k8s namespaces (-n flags) subsection of the recent-usage recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_0
  - DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_1
  - DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_2
-->

#### k8s namespaces (-n flags)
${DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_0.map(([DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_1,DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_2])=>`- ${DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_1} (${DATA_AUTO_MODE_RECON_K8S_NAMESPACES_VAR_2}×)`).join(`
`)}
