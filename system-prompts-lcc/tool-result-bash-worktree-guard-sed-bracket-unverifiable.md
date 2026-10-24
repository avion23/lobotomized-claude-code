<!--
name: 'Tool Result: worktree guard sed bracket unverifiable'
description: Explains when the check cannot tell where sed ends a pattern and how to pass.
ccVersion: 2.1.308
-->
 (the check cannot tell where every sed ends a pattern or address here: a bracket is unclosed or holds the delimiter, a control character, "\[", "[.", "[=", a broken [:class:], "[" just before "]" or "^", or "-]" just after "]"; a y operand holds "["; or the delimiter is "[" or alphanumeric. To pass: use another delimiter; put "-" straight after "[" or "[^" unless "]" already stands there (then match "-" in a command of its own); or move the character, escaped, out of a non-negated bracket)
