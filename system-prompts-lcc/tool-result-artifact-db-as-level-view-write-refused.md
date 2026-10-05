<!--
name: 'Tool Result: Artifact db as_level ''view'' write refused'
description: >-
  write_db tool result explaining that nothing can be written when acting at
  as_level 'view', including the caller's own data/users subtree, and how to
  write as another level
ccVersion: 2.1.284
-->
nothing can be written at as_level 'view', your own data/users subtree included, so nothing was sent. Omit as_level to write as yourself, or pass 'interact' or 'admin' to check what that level can write.
