<!--
name: 'Tool Result: Chrome file_upload not allowed inside browser_batch'
description: >-
  Deny message when file_upload is called inside browser_batch in a session
  where it must run alone; nothing ran.
ccVersion: 2.1.308
-->
file_upload cannot run inside browser_batch in this session, and nothing in this call ran. If file_upload is among your tools, call it on its own.
