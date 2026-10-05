<!--
name: 'Tool Parameter: Artifact DB as_level'
description: >-
  `as_level` on read_db/write_db: act at interact/admin instead of the caller's
  own access, never raising it.
ccVersion: 2.1.284
-->
read_db and write_db only: act at this access level instead of your own, to check what the page's access rules let such a user do — 'view' is someone the artifact is shared with who can only view it, 'interact' any signed-in viewer who can use the page, 'admin' someone who can edit it. It narrows, never raises, your access and keeps your identity (`me` is still you); at 'view' nothing can be written, your own data/users subtree included. At a lowered level a write the rules refuse reads as not found and a refused read as empty. Omit it to act as yourself.
