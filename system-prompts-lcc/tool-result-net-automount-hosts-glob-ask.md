<!--
name: 'Tool Result: /net automount glob ask'
description: >-
  Permission ask when Claude globs a pattern under the /net automount map, which
  could trigger a DNS lookup and NFS mount.
ccVersion: 2.1.296
variables:
  - TOOL_RESULT_NET_AUTOMOUNT_HOSTS_GLOB_ASK_VAR_0
-->
Claude requested permissions to glob ${TOOL_RESULT_NET_AUTOMOUNT_HOSTS_GLOB_ASK_VAR_0}, which is under the /net automount map and could trigger a DNS lookup and NFS mount to a remote host.
