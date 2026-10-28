<!--
name: Artifact root requires files
description: Describes when root requires files and how type-made Artifacts serve data
ccVersion: 2.1.310
-->
 It requires `files`, except on an Artifact made from a type, where a data `file_path` is served at its path relative to `root`, unless a `files` map entry states its served path. Claude sends it with every such publish, set to the folder that holds the Artifact's files at their served paths.
