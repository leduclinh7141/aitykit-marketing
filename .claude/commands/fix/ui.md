---
description: Analyze and fix UI/design issues
argument-hint: [issue]
---

Use `ui-ux-designer` subagent to read and analyze `./docs/design-guidelines.md` then fix the following issues:
<issue>$ARGUMENTS</issue>

## Workflow
If the user provides screenshots or videos, use `ai-multimodal` skill to describe the issue in detail.

1. Use `ui-ux-designer` subagent to implement the fix step by step.
2. Use screenshot capture tools along with `ai-multimodal` skill to take screenshots of the implemented fix and analyze those outputs to verify the result matches the design guideline.
   - If the issues are not addressed, repeat the process until all issues are addressed.
3. Use `chrome-devtools` skill to analyze the implemented fix and make sure it matches the design guideline.
4. Project Management & Documentation:
   **If user approves the changes:** Use `project-manager` and `docs-manager` subagents in parallel to update the project progress and documentation:
     * Use `project-manager` subagent to update the project progress and task status.
     * Use `docs-manager` subagent to update the docs in `./docs` directory if needed.
     * **IMPORTANT:** Sacrifice grammar for the sake of concision when writing outputs.
   **If user rejects the changes:** Ask user to explain the issues and repeat the process.
5. Final Report:
   * Report back to user with a summary of the changes
   * Guide user to get started and suggest the next steps.
   * **IMPORTANT:** Sacrifice grammar for the sake of concision when writing reports.
   * **IMPORTANT:** In reports, list any unresolved questions at the end, if any.

**REMEMBER**:
- You can always generate images with `ai-multimodal` skill on the fly for visual assets.
- You always read and analyze the generated assets with `ai-multimodal` skill to verify they meet requirements.
- For image editing (removing background, adjusting, cropping), use `ImageMagick` skill or similar tools as needed.
- **IMPORTANT:** Analyze the skills catalog and activate the skills that are needed for the task during the process.
