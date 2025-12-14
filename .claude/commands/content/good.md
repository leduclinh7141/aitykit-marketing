---
description: Write good creative & smart copy [GOOD]
argument-hint: [user-request]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

---

Write good creative & smart copy for this user request:
<user_request>$ARGUMENTS</user_request>

## Workflow

- If the user provides screenshots, use `ai-multimodal` skill to analyze and describe the context in detail.
- If the user provides videos, use `ai-multimodal` (`video-analysis`) skill to analyze video content.
- Use multiple `researcher` agents in parallel to search for relevant information, then report back to main agent.
- Use `/scout:ext` (preferred) or `/scout` (fallback) slash command to search the codebase for files needed to complete the task
- Use `planner` agent to plan the copy, make sure it can satisfy the user request.
- Use `copywriter` agent to write the copy based on the plan, then report back to main agent.