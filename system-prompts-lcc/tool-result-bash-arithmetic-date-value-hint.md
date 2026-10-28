<!--
name: 'Tool Result: Bash arithmetic date value hint'
description: Hint on passing a date value to arithmetic safely
ccVersion: 2.1.311
-->
 (if this value comes from date: some versions print %N and %q as a letter and others leave them unchanged, and arithmetic can read either as a variable. To pass: use date +%s, or do the sum in bc or awk)
