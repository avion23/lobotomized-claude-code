<!--
name: 'Tool Result: Artifact edits with files or root refused'
description: Says edits change only file_path and cannot combine with files or root
ccVersion: 2.1.299
-->
`edits` changes only the file at `file_path`: not with `files` (publish the other files in a call without edits) and not with `root` (Edit a file that needs `root`, then publish it with `root` and no edits). Nothing was published.
