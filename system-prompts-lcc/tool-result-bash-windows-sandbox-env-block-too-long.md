<!--
name: 'Tool Result: Windows sandbox environment block too long'
description: >-
  Says the settings env variables and the command exceed 30,000 characters in
  the Windows sandbox
ccVersion: 2.1.299
-->
The environment variables that your settings files or /env set leave no room for this command in the Windows sandbox: the variables and the command together come to more than 30,000 characters. Shorten the env block in your settings, or move long values into files.
