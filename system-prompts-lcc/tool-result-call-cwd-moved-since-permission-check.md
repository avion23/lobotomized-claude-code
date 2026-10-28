<!--
name: 'Tool Result: Call cwd moved since permission check'
description: >-
  Error when the working directory changed since the call's permission check, so
  the call did not run
ccVersion: 2.1.311
-->
The working directory no longer leads where it did when this call was permission-checked (it was deleted, a part of its path was replaced, or it can't be examined), so the call was not run. Make the call again to have it checked afresh.
