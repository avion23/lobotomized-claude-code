<!--
name: 'Git bundle: Windows git.exe directory clause'
description: >-
  Windows-only suffix from Hlt(), directly interpolated as `${Hlt()}` inside the
  git-bundle-upload 'git was not found on PATH' error strings.
ccVersion: 2.1.284
-->
 On Windows, that directory must hold git.exe itself, since git.cmd and git.bat wrappers are skipped.
