<!--
name: 'Sandbox install: profile readable summary'
description: Summary of what the profile grant made readable and excluded.
ccVersion: 2.1.305
variables:
  - DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_0
  - DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_1
  - DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_2
  - DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_3
  - DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_4
  - DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_5
-->
 Sandboxed commands can now read your user profile (${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_0}) except credential stores: ${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_1} folders made readable, ${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_2} excluded${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_3.length>0?`, ${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_3.length} left unreadable because their permissions could not be changed`:""}. That includes package-manager configuration that can hold feed tokens (.npmrc, pip.ini, NuGet.Config, Maven settings.xml, gradle.properties, .gitconfig). ${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_4} ${DATA_SANDBOX_INSTALL_PROFILE_READABLE_SUMMARY_VAR_5()}
