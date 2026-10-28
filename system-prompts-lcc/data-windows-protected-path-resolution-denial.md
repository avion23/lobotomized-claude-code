<!--
name: 'Data: Windows protected path resolution denial'
description: >-
  Explains why a Windows write is denied when a possible protected path cannot
  be resolved
ccVersion: 2.1.312
variables:
  - QUOTE_PATH_FN
  - WRITE_PATHS
  - UNRESOLVED_PATH
  - MAX_PATH_SPELLINGS
-->
Refusing to write ${QUOTE_PATH_FN(WRITE_PATHS[0])}: on Windows this path, or a link on the way to it, may also open ${QUOTE_PATH_FN(UNRESOLVED_PATH)}, and Claude Code could not work out where that leads on disk (a link or folder on the way could not be examined, the links do not resolve, or there were more than ${MAX_PATH_SPELLINGS} other spellings to look up). So the write may land in the jobs, daemon, shell-snapshots or session-env folder or in daemon.json of the Claude Code config directory. The file tools do not write those. If the file is on this computer, name it by the plain drive path of the file itself, such as C:\\x, with no link, no share, and no name that ends in a dot or a space. If it is on another computer, a person can edit it there.
