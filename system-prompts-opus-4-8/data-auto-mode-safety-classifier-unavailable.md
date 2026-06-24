<!--
name: 'Data: Auto mode safety classifier unavailable'
description: >-
  tool_result text telling the model the safety classifier is down and to retry
  later or do read-only work.
ccVersion: 2.1.187
variables:
  - DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_0
  - DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_1
  - DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_2
  - DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_3
  - DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_4
  - DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_5
-->
${DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_0} is temporarily unavailable${DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_1(DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_2,DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_3)}${DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_4}${DATA_AUTO_MODE_SAFETY_CLASSIFIER_UNAVAILABLE_VAR_5} right now. Retry shortly; if it keeps failing, work on other tasks meanwhile. Read-only operations (reading files, searching code) don't require the classifier and still work.
