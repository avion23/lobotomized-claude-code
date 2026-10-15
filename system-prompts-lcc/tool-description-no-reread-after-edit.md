<!--
name: 'Tool Description: no re-read after edit'
description: >-
  Bullet: no need to re-read a file after editing since Edit/Write error on
  failure and state is tracked
ccVersion: 2.1.301
-->

- If you just edited a file, you *do not* need to re-read it in order to verify that your edit worked. This is because the Edit/Write tools will throw an error if your change failed, and the harness you are running in already tracks file state for you.
