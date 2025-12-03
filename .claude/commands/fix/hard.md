---
description: Use subagents to plan and fix complex campaign issues
argument-hint: [issues]
---

**Ultrathink** to plan & start fixing these issues follow the Orchestration Protocol in your `CLAUDE.md` file:
<issues>$ARGUMENTS</issues>

## Workflow:

If the user provides screenshots or examples, use `ai-multimodal` skill to analyze the issue in detail.

Use `sequential-thinking` skill to break complex problems into sequential thought steps.
Use `problem-solving` skills to tackle the issues.
Analyze the skills catalog and activate other skills that are needed for the task during the process.

1. Use `researcher` subagent to understand the root cause and gather best practices.
2. Use `planner` subagent to create an action plan based on the research.
3. Then use general agent (main agent) to implement the plan step by step.
4. Use `copywriter` subagent to review content quality and brand consistency.
5. If there are issues, repeat from step 1.
6. After finishing, delegate to `project-manager` to update project status.
7. Project Management & Documentation:
   **If user approves the changes:** Use `project-manager` and `docs-manager` subagents in parallel to update the project progress and documentation.
   **If user rejects the changes:** Ask user to explain the issues and repeat the process.
8. Final Report:
   * Report back to user with a summary of the changes
   * Guide user on next steps
   - **IMPORTANT:** Sacrifice grammar for the sake of concision when writing reports.
   - **IMPORTANT:** In reports, list any unresolved questions at the end, if any.

**REMEMBER**:
- You can always generate images with `ai-multimodal` skills on the fly for visual assets.
- You always read and analyze the generated assets with `ai-multimodal` skills to verify they meet requirements.
