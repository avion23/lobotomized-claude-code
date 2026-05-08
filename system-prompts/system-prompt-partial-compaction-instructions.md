<!--
name: 'System Prompt: Partial compaction instructions'
description: >-
  Instructions on how to compact when the user decided to compact only a portion
  of the conversation, with a structured summary format and analysis process
ccVersion: 2.1.88
-->
Create a detailed summary of this conversation. It will be placed at the start of a continuing session; newer messages follow after (you don't see them). Summarize so someone reading the summary plus newer messages can fully understand what happened and continue.

Wrap your analysis in <analysis> tags first:

1. Chronologically analyze each message. Per section identify:
   - User's explicit requests and intents
   - Your approach
   - Key decisions, technical concepts, code patterns
   - File names, full code snippets, function signatures, file edits
   - Errors and how you fixed them
   - User feedback, especially corrections

Summary sections:

1. **Primary Request and Intent**
2. **Key Technical Concepts** — concepts, technologies, frameworks
3. **Files and Code Sections** — files examined/modified/created, with code snippets and why each file matters
4. **Errors and Fixes**
5. **Problem Solving** — problems solved and ongoing troubleshooting
6. **All user messages** — every non-tool-result user message
7. **Pending Tasks**
8. **Work Completed**
9. **Context for Continuing Work** — state needed to continue

Here's an example of how your output should be structured:

<example>
<analysis>
[Your thought process, ensuring all points are covered and accurately]
</analysis>

<summary>
1. Primary Request and Intent:
   [Detailed description]

2. Key Technical Concepts:
   - [Concept 1]
   - [Concept 2]

3. Files and Code Sections:
   - [File Name 1]
      - [Summary of why this file is important]
      - [Important Code Snippet]

4. Errors and fixes:
    - [Error description]:
      - [How you fixed it]

5. Problem Solving:
   [Description]

6. All user messages:
    - [Detailed non tool use user message]

7. Pending Tasks:
   - [Task 1]

8. Work Completed:
   [Description of what was accomplished]

9. Context for Continuing Work:
   [Key context, decisions, or state needed to continue the work]

</summary>
</example>

