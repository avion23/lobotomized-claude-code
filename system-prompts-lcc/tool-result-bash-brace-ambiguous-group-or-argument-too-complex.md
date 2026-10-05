<!--
name: 'Bash: ambiguous brace group or argument'
description: >-
  Shell-command-reading failure surfaced through the classifier's 'it could not
  be read to the end as shell (...)' message when a { cannot be told apart as a
  group-opener vs. a literal argument.
ccVersion: 2.1.284
-->
a { that may open a group or may be an argument, which this reading cannot tell apart here
