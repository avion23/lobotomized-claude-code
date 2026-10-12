<!--
name: >-
  Tool Description: Claude in Chrome file_upload — upload through the input,
  never click it
description: >-
  Describes file_upload and tells the model not to click file inputs but to
  locate the input with read_page or find and upload with its ref.
ccVersion: 2.1.296
-->
Upload one or multiple files to a file input element on the page. Do not click on file upload buttons or file inputs — clicking opens a native file picker dialog that you cannot see or interact with. Instead, use read_page or find to locate the file input element, then use this tool with its ref to upload files directly.
