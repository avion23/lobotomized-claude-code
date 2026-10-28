<!--
name: Artifact type no root folder
description: Error that no folder holding the file can be a root and how to fix it
ccVersion: 2.1.310
-->
No folder that holds it can be a `root`: a `root` must lie in one of the session's working directories or your scratchpad directory. Copy it into one of them, at the path this Artifact's page reads it from under a folder there, then send the call again with `root` set to that folder.
