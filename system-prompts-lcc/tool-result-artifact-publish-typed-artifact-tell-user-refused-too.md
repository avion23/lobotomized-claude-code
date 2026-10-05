<!--
name: 'Artifact publish: type-created artifact refusal -- tell the user'
description: >-
  Guidance clause telling Claude that if the Artifact being updated turns out to
  be type-created, the operation will also be refused, and to tell the user
  rather than retry.
ccVersion: 2.1.284
-->
If the Artifact being updated was created from an Artifact type, that will be refused too, because nothing can be published to it from this session; in that case tell the user so.
