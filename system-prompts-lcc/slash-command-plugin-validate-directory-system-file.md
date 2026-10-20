<!--
name: 'Plugin validate: system file found'
description: 'Finding: a macOS/Windows system file is in the plugin.'
ccVersion: 2.1.305
-->
This is a macOS or Windows system file (.DS_Store, Thumbs.db, desktop.ini, or anything under __MACOSX), not part of your plugin. The directory cannot scan or list a plugin that contains one. Remove it from the repository (git rm --cached the file, commit and push, and add the name to .gitignore), then validate again.
