<!--
name: 'Data: Settings sandbox network deniedResolvedAddresses description'
description: >-
  Schema description for the sandbox network.deniedResolvedAddresses setting in
  settings.json, listing IP/CIDR addresses an allowed hostname must not resolve
  to, and its interaction with deniedDomains, allowedDomains, parentProxy and
  mitmProxy
ccVersion: 2.1.284
-->
IP addresses / CIDR ranges (IPv4 or IPv6, unbracketed) that an allowed HOSTNAME must not resolve to, in addition to the built-in set (see README "Resolved-address check") and any IP literal listed in deniedDomains. A permitted name that resolves only into these is refused instead of dialed. A name may resolve to a denied address only if that IP literal (and port) is itself in allowedDomains. Not evaluated for connections routed through parentProxy (including one taken from HTTP_PROXY/HTTPS_PROXY) or mitmProxy (that hop resolves the name).
