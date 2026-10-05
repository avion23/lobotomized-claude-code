<!--
name: 'Git bundle: Windows exe-only clause'
description: >-
  Windows-only suffix from wz(), embedded in jin()'s synthetic git-not-found
  stderr. Traced reachability: GTo() (write-tree, hardened:!1 so it can hit
  jin()/wz()) embeds this stderr into its `detail`; cRo()'s
  fallback-legacy-bundle path turns that into `{kind:'refused',sentence:...}`;
  Kqt() (git-bundle-upload fallback flow, tengu_ccr_bundle_upload telemetry)
  returns `{success:!1,error:`${s.error}
  ${g.sentence}`,failReason:'uncommitted_credentials'}` — confirmed model-facing
  via this fallback chain.
ccVersion: 2.1.284
-->
 (only git.exe counts; git.cmd and git.bat wrappers are skipped)
