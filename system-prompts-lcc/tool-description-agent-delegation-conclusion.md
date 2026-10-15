<!--
name: 'Tool Description: Agent delegation conclusion'
description: >-
  Agent prompt summary: use subagents for parallelism and side quests, not for
  small lookups, and wait for delegated searches
ccVersion: 2.1.301
-->
If the amount of work to be done is small (for example, just making a few file reads or searches or tool calls), that is probably not enough to warrant using a subagent.

For a single-fact lookup where you already know the file, symbol, or value, search directly. And once you've delegated a search, wait for the result to return rather than also running it yourself.
