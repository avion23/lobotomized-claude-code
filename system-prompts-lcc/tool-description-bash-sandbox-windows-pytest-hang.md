<!--
name: 'Tool Description: Bash sandbox Windows pytest hang'
description: >-
  Warns pytest without a cache folder can hang in the Windows sandbox; kill and
  rerun with -p no:cacheprovider.
ccVersion: 2.1.308
-->
A recent `pytest` in a project with no `.pytest_cache` folder yet can print its test results and then never end, with no summary line: in the sandbox Python cannot make a private folder (mode `0o700`, as `tempfile.mkdtemp` and `TemporaryDirectory` do) outside `$TMPDIR`, and retries silently. Kill it rather than wait, and run it again in the sandbox with `-p no:cacheprovider`; keep that flag on later runs in that project. Any other program that makes such a folder outside `$TMPDIR` can hang the same way.
