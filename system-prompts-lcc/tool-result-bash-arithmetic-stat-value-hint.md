<!--
name: 'Tool Result: Bash arithmetic stat value hint'
description: Hint on passing a stat value to arithmetic safely
ccVersion: 2.1.311
-->
 (if this value comes from stat: a word that comes from a variable or a command, or a path starting with a ~ other than ~/, can turn into --help, and stat then prints text, not a number. To pass, write stat -c FORMAT -- "PATH", with FORMAT one of %s %b %B %W %X %Y %Z, PATH in double quotes, and no redirect but 2>/dev/null)
