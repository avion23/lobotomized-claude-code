<!--
name: Artifact Identical Resubmission Sourceless
description: >-
  identical_resubmission clause covering unseen live versions and versions that
  arrived only as a summary
ccVersion: 2.1.312
variables:
  - TOOL_RESULT_ARTIFACT_IDENTICAL_RESUBMISSION_SOURCELESS_VAR_0
  - TOOL_RESULT_ARTIFACT_IDENTICAL_RESUBMISSION_SOURCELESS_VAR_1
  - TOOL_RESULT_ARTIFACT_IDENTICAL_RESUBMISSION_SOURCELESS_VAR_2
-->
${TOOL_RESULT_ARTIFACT_IDENTICAL_RESUBMISSION_SOURCELESS_VAR_0}, and ${TOOL_RESULT_ARTIFACT_IDENTICAL_RESUBMISSION_SOURCELESS_VAR_1==="none"?`${TOOL_RESULT_ARTIFACT_IDENTICAL_RESUBMISSION_SOURCELESS_VAR_2===void 0?"the live version":"that version"} has not reached you`:"that version reached you only as a summary, never as its source"}. 
