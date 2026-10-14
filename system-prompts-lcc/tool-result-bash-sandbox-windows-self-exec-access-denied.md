<!--
name: 'Tool Result: Windows sandbox self-exec access denied'
description: >-
  Says Windows refused to start the sandbox account with access denied and tells
  the model to retry once and then tell the user
ccVersion: 2.1.299
-->
Windows refused to start Claude Code as the sandbox account (access denied, 0x80070005), so the command most likely did not run. The Secondary Logon service is not the cause. Claude Code tries to set the permission on its program file again before the next command, so try the command once more. If it fails the same way, stop and tell the user.
