---
description: Analyze and fix content or campaign issues [AUTO DETECT COMPLEXITY]
argument-hint: [issues]
---

If there is a markdown implementation plan already, use `/campaign:plan` to execute it.

Else:
- Analyze the issues and ask for more details if needed.
- Decide to use `/fix:fast` or `/fix:hard` SlashCommands based on the complexity.
- Execute SlashCommand: `/fix:fast <detailed-instructions-prompt>` or `/fix:hard <detailed-instructions-prompt>`
- Note: `detailed-instructions-prompt` is **an enhanced prompt** that describes the issue in detail based on the provided issue description.
