<!--
name: 'Tool Description: Artifact publish edits small change hint'
description: >-
  Third-person hint that small changes can go as edits on the publish call
  instead of editing the file first
ccVersion: 2.1.299
-->
 For a small change to a page published from a file in this conversation, Claude can send the change as `edits` on the publish call itself (old_str/new_str pairs copied exactly from the file as it now stands) instead of editing the file first; a rewrite of most of the page still goes through the file.
