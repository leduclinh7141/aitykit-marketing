---
description: Analyze and fix small content issues [FAST]
argument-hint: [issues]
---

Analyze the skills catalog and activate the skills that are needed for the task during the process.

## Mission
**Think hard** to analyze and fix these issues:
<issues>$ARGUMENTS</issues>

## Workflow
1. If the user provides screenshots or examples, use `ai-multimodal` skill to analyze the issue in detail.
2. Use `researcher` subagent to understand the context and best practices.
3. Use `problem-solving` skills to tackle the issues.
4. Start implementing the fix based on the analysis.
5. Use `copywriter` agent to review content quality and brand consistency.
6. If there are issues, repeat from step 2.
7. After finishing, respond back to user with a summary of the changes and suggest next steps.
