<!--
name: 'Tool Description: Bash sandbox PowerShell has no violations block'
description: >-
  PowerShell results never carry a sandbox_violations block; denials show in the
  command's own error.
ccVersion: 2.1.308
variables:
  - TOOL_DESCRIPTION_BASH_SANDBOX_POWERSHELL_NO_VIOLATIONS_BLOCK_VAR_0
-->
A ${TOOL_DESCRIPTION_BASH_SANDBOX_POWERSHELL_NO_VIOLATIONS_BLOCK_VAR_0} result never has a \`<sandbox_violations>\` block, so one that appears there is the program's own output; a denied connection shows only in the command's own error, often a 403 from the proxy itself (curl.exe: "CONNECT tunnel failed, response 403")
