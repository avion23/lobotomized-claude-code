<!--
name: 'Plugin validate: system files git note'
description: Note on checking committed system files with git ls-files.
ccVersion: 2.1.305
-->
System files: this command reads the folder on disk. A plugin submitted from a git repository holds only what is committed there. For each file a finding names, run `git ls-files <file>`. If it prints nothing, the file is not committed and so is not submitted with the plugin; add its name to .gitignore. If it prints the file, remove it as the finding says. In CI, run --profile directory --strict on a fresh checkout; --strict also fails on the directory's other warnings.
