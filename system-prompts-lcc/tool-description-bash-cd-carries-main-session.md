<!--
name: 'Tool Description: Bash cd carries in main session'
description: Explains when cd carries to the next call in the main session
ccVersion: 2.1.311
-->
`cd` carries to the next call only in the main session, if the command succeeds and ends inside the working directories. Outside them the shell returns to the start folder; otherwise it stays where it was.
