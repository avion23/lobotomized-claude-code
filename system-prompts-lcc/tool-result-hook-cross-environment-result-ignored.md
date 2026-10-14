<!--
name: Hook cross-environment result ignored
description: >-
  A hook changed a tool result across environments, so the result was read
  unchanged.
ccVersion: 2.1.300
-->
A hook changed a tool's result. That is allowed only for calls that run in the same environment as the hook, and this one does not, so Claude read the result unchanged.
