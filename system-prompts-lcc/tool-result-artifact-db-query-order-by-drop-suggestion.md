<!--
name: Suggest dropping order_by (Artifact DB)
description: >-
  Else-branch suggestion when the ordered query's limit already meets the server
  cap.
ccVersion: 2.1.284
-->
Drop `query.order_by` and page with `query.cursor` to read them all, or narrow with `query.where`.
