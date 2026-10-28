<!--
name: Windows sandbox git folder above working directory
description: >-
  Explains that sandboxed git cannot write the .git folder above a subfolder
  start directory, how to look for it, and to tell the user to start Claude Code
  at the repository root rather than running git init or widening write access
ccVersion: 2.1.310
variables:
  - ARE_UNSANDBOXED_COMMANDS_ALLOWED
-->
When Claude Code was started in a subfolder of a git repository, sandboxed commands cannot write the \`.git\` folder above the working directory, and may be unable to read it. Any \`git\` command that changes the repository, such as \`git add\` or \`git commit\`, then fails on a path under \`.git\`, most often with "Unable to create" and a path ending in \`.lock\`, then "Permission denied"; where the folder is unreadable, \`git\` can fail with "fatal: not a git repository", or with "fatal: error reading" and that folder's path. Look before anything else: \`ls -d .git ../.git ../../.git\` and so on up to the drive's root. If it finds a \`.git\` file or folder in or below the folder Claude Code was started in, whatever lies above, this item does not apply: do not retry outside the sandbox, and tell the user. The same goes where the only \`.git\` is in the user's home folder or above it: the sandbox does not start in those folders. If every look says "No such file or directory", only the item on \`git init\` above applies. Otherwise do not run or suggest \`git init\`. If the user's request needs the repository (commits, branches, a diff), and a \`.git\` lies above or a look further up is refused, ${ARE_UNSANDBOXED_COMMANDS_ALLOWED?"retry `git` alone, never a script or tool that calls it, as described above for a sandbox-caused failure, and tell the user in the same message that":"tell the user that"} starting Claude Code at its root avoids this; adding the root to \`sandbox.filesystem.allowRead\`, under the first item's rules, lets \`git\` read but not commit; never suggest adding the root to \`allowWrite\`. That is their decision, and a large repository can slow the start or keep the sandbox from starting.
