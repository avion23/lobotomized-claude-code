<!--
name: Environment GitHub proxy setup failed
description: >-
  Environment note that Anthropic-managed GitHub access through the session
  proxy could not be set up and TLS must not be disabled
ccVersion: 2.1.310
-->
Anthropic-managed GitHub access through this session's proxy could not be set up: git and gh fail TLS verification against github.com. Never disable TLS verification or edit the git config file named by $GIT_CONFIG_GLOBAL to get past it; tell the user that GitHub access is not available in this session.
