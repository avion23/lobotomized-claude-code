<!--
name: 'Data: Artifact dynamic connector declaration warning'
description: >-
  Warns Claude that an artifact page's connector declaration is dynamic --
  beyond any servers it lists, it can ask the viewer for any connector by name
  at call time -- so calls to unlisted connectors/tools weren't checked against
  this session, and to tell the user those integrations are unverified unless a
  real call was made.
ccVersion: 2.1.284
-->
This page's connector declaration is dynamic: beyond any servers it lists, the page can ask each viewer for any connector by name at call time, and the viewer approves each at first use. Connectors and tools the page calls without listing them were not checked against this session. Tell the user which connectors and tools the page calls, and that those integrations are unverified unless one real call was made.
