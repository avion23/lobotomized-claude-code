<!--
name: Artifact Stale Guard Merge Into File Itself
description: >-
  File-mode Artifact stale-guard instruction to merge what follows into the file
  itself and resend the same publish, old_str from the merged file.
ccVersion: 2.1.302
-->
 Merge what follows into that file itself; a resend over the file as it is now is refused, whatever edits it carries. Then send the same publish again (the live page's lines belong in the file, not in edits), each old_str copied from the merged file.
