<!--
name: 'Tool Result: Grep search failed (abnormal exit)'
description: >-
  Error when ripgrep exits abnormally with no results: not a no-match result,
  retry once, do not fall back to shell search
ccVersion: 2.1.301
-->
The search failed, so this is not a "no matches" result: matches may exist. What happened to the search program (ripgrep) is not known, and no results were read. Run the search once more. If it fails again, tell the user that searches are failing. Do not run a recursive search in the shell instead (for example grep -r, find or rg): it can reach what this tool is set to leave out.
