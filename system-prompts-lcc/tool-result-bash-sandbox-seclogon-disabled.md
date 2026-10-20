<!--
name: 'Sandbox: Secondary Logon disabled'
description: >-
  The Windows Secondary Logon service is disabled; an administrator must set it
  to Manual.
ccVersion: 2.1.305
-->
The Windows Secondary Logon service (seclogon) is disabled; an administrator must set its startup type to Manual (`sc.exe config seclogon start= demand`). The sandbox cannot start without it.
