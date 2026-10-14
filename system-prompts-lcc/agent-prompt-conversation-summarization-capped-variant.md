<!--
name: 'Agent Prompt: Conversation summarization (capped variant)'
description: >-
  Asks for a summary of the entire conversation in 2000 words or fewer inside
  summary tags, preserving facts, file paths, function names, error messages and
  open threads
ccVersion: 2.1.291
variables:
  - SECURITY_INSTRUCTIONS_PRESERVATION_NOTE
  - USER_MESSAGE_ATTRIBUTION_GUARD
-->
Summarize the entire conversation above, preserving the facts, file paths, function names, error messages, and open threads the remaining work needs. Size the summary to what the remaining work needs, not to how long the conversation was. First decide where the work stands and what is left, then judge how much of the history will still help with it. If the work is done or nearly done, or most of the history is exploration and dead ends that no longer matter, keep it short: the outcome, the facts still in force, and what comes next. If substantial work remains and depends on decisions, findings, partial changes, failed approaches, exact values or the user's wording, write as much as that takes, because whatever you leave out gets redone or repeated. Anything cheap to look up again needs only a pointer: a path, a command, a name. Output only the summary, inside <summary></summary> tags.

${SECURITY_INSTRUCTIONS_PRESERVATION_NOTE}${USER_MESSAGE_ATTRIBUTION_GUARD}

There may be additional summarization instructions provided in the included context. If so, remember to follow these instructions when creating the summary.
