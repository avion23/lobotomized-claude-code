<!--
name: Device identify probe tool description
description: >-
  Tool description for the bridge's own identify probe tool, explaining it takes
  no input and returns this machine's platform, arch, version and dial-name so
  refusing it would only hide the machine from the bridge.
ccVersion: 2.1.284
-->
The bridge service's own identify probe, sent with no session. It takes no input, runs nothing and reads nothing here, and answers the name this machine dialed the bridge under plus platform, architecture, Claude Code version and the time. Refusing it would hide the machine from the bridge, not keep anything from a sender.
