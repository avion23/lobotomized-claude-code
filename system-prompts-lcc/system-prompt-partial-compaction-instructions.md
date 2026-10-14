<!--
name: 'System Prompt: Partial compaction instructions'
description: >-
  Instructions on how to compact when the user decided to compact only a portion
  of the conversation, with a structured summary format and analysis process
ccVersion: 2.1.273
variables:
  - SUMMARY_ANALYSIS_INSTRUCTIONS
  - USER_MESSAGE_ATTRIBUTION_GUARD
-->
Summarize this portion of the conversation. The summary goes at the start of a continuing session and newer messages (which you do not see) follow it, so a reader of the summary plus those messages must be able to continue the work. Record only what the transcript shows; keep uncertainty where the record is incomplete.

Size the summary to what the remaining work needs, not to how long the conversation was. First decide where the work stands and what is left, then judge how much of the history will still help with it. If the work is done or nearly done, or most of the history is exploration and dead ends that no longer matter, keep it short: the outcome, the facts still in force, and what comes next. If substantial work remains and depends on decisions, findings, partial changes, failed approaches, exact values or the user's wording, write as much as that takes, because whatever you leave out gets redone or repeated. Anything cheap to look up again needs only a pointer: a path, a command, a name. The newer messages show the latest state, so carry what they will rely on: the user's requests, constraints and decisions, the work done and its results, and the context needed to make sense of what follows. Make that judgment in the <analysis> block; only what you write inside <summary></summary> tags is kept.

${SUMMARY_ANALYSIS_INSTRUCTIONS}

Output <analysis> then <summary>. The summary has these numbered sections:
1. Primary Request and Intent: the user's explicit requests and intents.
2. Key Technical Concepts: technologies, frameworks, and concepts discussed.
3. Files and Code Sections: files examined, modified, or created; why each matters; code snippets.
4. Errors and fixes: each error and how it was fixed.
5. Problem Solving: problems solved and ongoing troubleshooting.
6. All user messages: every user message that is not a tool result; keep instructions whose exact wording matters verbatim.${USER_MESSAGE_ATTRIBUTION_GUARD}
7. Pending Tasks: outstanding tasks, including attempted but unconfirmed work.
8. Work Completed: what this portion accomplished and confirmed.
9. Context for Continuing Work: decisions and state needed to continue in subsequent messages.
