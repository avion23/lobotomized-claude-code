<!--
name: 'Tool Result: Git partial-clone invocation changed env or args'
description: >-
  Error saying programs.buildInvocation changed the environment or the arguments
  it was handed
ccVersion: 2.1.299
-->
programs.buildInvocation must return the environment it was handed, less at most PWD and OLDPWD, and the arguments it was handed, with nothing before them but -C and the directory it was handed; it changed the environment or the arguments
