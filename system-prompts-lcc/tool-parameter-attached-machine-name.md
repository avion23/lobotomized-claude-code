<!--
name: 'Tool Parameter: Attached machine name field'
description: >-
  Shared input_schema description for the optional attached-machine-name field
  (_host) added to every tool call schema when device routing is available,
  explaining it must name a listed attached machine and defaults to this
  session's own environment
ccVersion: 2.1.284
-->
Optional. Name of an attached machine to run this tool call on; omit it to run in this session's own environment (the default). Use only a name this session listed as attached; the result says where it ran. Choose per call by which machine the command or file path concerns; the attached-machines note says what lives where and which are reachable now.
