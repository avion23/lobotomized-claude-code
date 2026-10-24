<!--
name: 'Tool Description: Bash sandbox Windows Schannel TLS (user decides)'
description: >-
  Windows-native TLS programs cannot do HTTPS in the sandbox; tell the user how
  they can leave it.
ccVersion: 2.1.308
variables:
  - TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_SCHANNEL_TLS_USER_DECIDES_VAR_0
-->
On Windows, programs that use Windows' own TLS (Schannel) cannot make HTTPS connections inside the sandbox, even to an allowed host: Windows' \`curl.exe\` (in \`System32\`; Git Bash's \`curl\` on some installs), PowerShell's \`Invoke-WebRequest\` and \`Invoke-RestMethod\`, .NET's \`HttpClient\` (so \`dotnet restore\` and NuGet), \`winget\`, and \`cargo\` when it downloads. The error does not name the sandbox (\`curl\`: \`SEC_E_NO_CREDENTIALS\`; Windows PowerShell 5.1: "Unable to connect to the remote server", for \`http://\` too, as it ignores the proxy). Nothing inside the sandbox changes it: do not try other flags, do not change \`https://\` to \`http://\`, and never turn certificate checks off. Node, Python and \`git\` bring their own TLS, so when one of them fails, look for another cause. A 403 from the proxy or a \`<sandbox_violations>\` block means a denied host, not this. When a command fails this way, tell the user that the sandbox blocks Windows' own TLS, so the command works only outside the sandbox, without its protection: they can ${TOOL_DESCRIPTION_BASH_SANDBOX_WINDOWS_SCHANNEL_TLS_USER_DECIDES_VAR_0}; leaving the sandbox is their decision, not yours.
