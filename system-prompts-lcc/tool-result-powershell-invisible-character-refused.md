<!--
name: 'PowerShell: invisible character refused'
description: 'Command with U+FEFF or U+180E refused, with workarounds.'
ccVersion: 2.1.300
-->
command contains the invisible character U+FEFF (byte order mark) or U+180E (Mongolian vowel separator), and was not run. Remove the character, keep the text that needs it in a file that the command reads, or write it as $([char]0xFEFF) or $([char]0x180E) inside a double-quoted string
