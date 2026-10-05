<!--
name: 'Tool Parameter: Artifact write_db Batch Writes'
description: >-
  Artifact tool input-schema description of write_db db_op 'batch' writes:
  all-or-nothing set/update/delete entries.
ccVersion: 2.1.284
variables:
  - TOOL_PARAMETER_ARTIFACT_WRITE_DB_BATCH_WRITES_VAR_0
  - TOOL_PARAMETER_ARTIFACT_WRITE_DB_BATCH_WRITES_VAR_1
-->
write_db with db_op 'batch' only: the writes to apply together, 1-${TOOL_PARAMETER_ARTIFACT_WRITE_DB_BATCH_WRITES_VAR_0} entries of {op: 'set'|'update'|'delete', collection, doc_id, and for set/update exactly one of data (inline object) or file_path (a local JSON file)${TOOL_PARAMETER_ARTIFACT_WRITE_DB_BATCH_WRITES_VAR_1?", plus if_version — that document's last-read `version`, required for every entry whose document already exists (omit it only when creating); if any pinned document has changed since, or an existing document's entry carries no pin, the whole batch writes nothing and the result names the first such entry":""}}. Each document is addressed at most once and the whole batch body is at most 1 MiB; the batch commits all-or-nothing where the server supports it, else ${TOOL_PARAMETER_ARTIFACT_WRITE_DB_BATCH_WRITES_VAR_1?"(a batch with no pinned entry) ":""}in order one at a time (the result says which).
