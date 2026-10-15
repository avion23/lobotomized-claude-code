<!--
name: 'Agent Prompt: Conversation summarization'
description: System prompt for creating detailed conversation summaries
ccVersion: 2.1.301
variables:
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_0
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_1
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_2
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_3
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_4
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_5
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_6
  - AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_7
-->
This conversation is being compacted. Your summary replaces everything above: the next context window starts from it, and you will usually carry on without the user reviewing it.

Next to the summary, that window will have the system prompt, project instructions and memory files, the files you read most recently (re-read from disk), the plan, any loaded skills, the status of background agents and shells, and possibly a path to the full transcript. Everything else, including any earlier summary above, survives only if you carry it.${AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_1?AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_2:""}

Size the summary to what the remaining work needs,${AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_0?" in 2000 words or fewer,":""} not to how long the conversation was. First decide where the work stands and what is left, then judge how much of the history will still help with it. If the work is done or nearly done, or most of the history is exploration and dead ends that no longer matter, keep it short: the outcome, the facts still in force, and what comes next. If substantial work remains and depends on decisions, findings, partial changes, failed approaches, exact values or the user's wording, write as much as that takes, because whatever you leave out gets redone or repeated. Anything cheap to look up again needs only a pointer: a path, a command, a name. Make that judgment first (in the <analysis> block when your reply has one); only what you write inside <summary></summary> tags is kept.

Whatever the length, keep:
- what the user is trying to get done and why, with their requests, corrections and preferences close to their own words
- every limit or constraint they set, quoted exactly, and anything they allowed, with the scope they gave it
- what was decided, learned, tried and ruled out, and why
- where the work stands: what is done and checked, what is changed but unchecked, what is unfinished
- the next step, tied to the user's latest request in their words

Follow any additional summarization instructions in context.${AGENT_PROMPT_CONVERSATION_SUMMARIZATION_VAR_6}
