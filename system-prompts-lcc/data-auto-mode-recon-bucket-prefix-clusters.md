<!--
name: 'Auto-mode recon: bucket prefix clusters'
description: Bucket name prefix clusters subsection of the config-scan recon section.
ccVersion: 2.1.296
variables:
  - DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_0
  - DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_1
  - DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_2
-->

#### Bucket name prefix clusters (distinct names per first-dash prefix)
${DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_0.clusters.map(([DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_1,DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_2])=>`- ${DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_1}-* (${DATA_AUTO_MODE_RECON_BUCKET_PREFIX_CLUSTERS_VAR_2} distinct names)`).join(`
`)}
