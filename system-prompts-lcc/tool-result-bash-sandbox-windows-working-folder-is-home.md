<!--
name: 'Tool Result: Windows sandbox working folder is home'
description: >-
  Says the Windows sandbox does not start when the working folder is the home or
  config folder and suggests a project folder
ccVersion: 2.1.299
-->
Claude Code's working folder is your home folder, a folder that contains it, or Claude Code's config folder. The Windows sandbox doesn't start there, because sandboxed commands from other sessions could then reach your settings and credentials. Start a new session in a project folder, or move this one there (`/cd <folder>` in a terminal)
