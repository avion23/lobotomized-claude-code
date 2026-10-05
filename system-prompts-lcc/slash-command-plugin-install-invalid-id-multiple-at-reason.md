<!--
name: 'Slash Command: Plugin install invalid id multiple @ reason'
description: >-
  Install error explaining an invalid plugin id whose plugin or marketplace name
  contains an extra "@", and that whoever named it can rename it.
ccVersion: 2.1.284
-->
Each part of a plugin id (plugin@marketplace) may use only the letters a-z and A-Z, digits, ".", "_" and "-", and must start with a letter or digit. Here the id holds more than one "@", so the plugin's name or the marketplace's name holds one; whoever named it can rename it.
