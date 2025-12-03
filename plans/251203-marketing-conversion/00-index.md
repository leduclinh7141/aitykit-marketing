# ClaudeKit Marketing Kit - Conversion Plan

**Document ID:** PLAN-251203-MARKETING
**Created:** 2025-12-03
**Status:** Draft

---

## Executive Summary

Convert **ClaudeKit Engineer** (software development focused) into **ClaudeKit Marketing** (marketing automation focused) based on features at [claudekit.cc/marketing](https://claudekit.cc/marketing).

**Scope:**
- 6 new marketing-focused AI agents (funnel-stage based)
- ~35 new slash commands for marketing workflows
- 8 new skill modules (SEO, social media, email, ads, analytics)
- Complete workflow redesign: Research → Insights → Creative → Plan → Create → Edit → Publish → Measure
- 12+ MCP integrations for ad platforms, analytics, social media

---

## Document Structure

| File | Description |
|------|-------------|
| [01-research-findings.md](./01-research-findings.md) | Current architecture analysis |
| [02-gap-analysis.md](./02-gap-analysis.md) | Gap analysis between current and target |
| [03-agent-specifications.md](./03-agent-specifications.md) | New agent definitions |
| [04-command-specifications.md](./04-command-specifications.md) | New command definitions |
| [05-skill-specifications.md](./05-skill-specifications.md) | New skill modules |
| [06-workflow-specifications.md](./06-workflow-specifications.md) | Workflow and config updates |
| [07-implementation-plan.md](./07-implementation-plan.md) | Phases, file inventory, validation |
| [08-appendix.md](./08-appendix.md) | Architecture diagrams and reference |

---

## Quick Stats

| Component | Current | Target | Change |
|-----------|---------|--------|--------|
| **Agents** | 15 engineering | 10 marketing | Replace 11, keep 4 |
| **Commands** | ~45 code-focused | ~35 marketing | Replace most |
| **Skills** | 12 dev skills | 8 marketing skills | Replace all |
| **Workflows** | Code → Test → Review | Research → Publish → Measure | Rewrite |

---

## Open Questions

1. Content Hub: R2 storage as skill or MCP server?
2. AI Artist: Extend `ai-multimodal` or new `brand-artist` skill?
3. MCP Servers: Which are available vs need building?
4. Shopify Skill: Keep for e-commerce marketing?

---

## Next Action

Await approval to proceed with implementation phases.
