# Marketing System Cleanup Plan

**Date:** 2025-12-14
**Objective:** Remove non-marketing elements from AityKit Marketing system

## Executive Summary

This marketing automation framework was extended from an engineering kit, leaving many coding-focused components. This cleanup ensures consistency across all features by removing:
- Engineering-focused workflows, commands, agents, and skills
- Developer documentation not relevant to marketing
- Technical integrations unrelated to marketing operations

---

## 🗑️ Items to Remove

### 1. Workflows (`.claude/workflows/`)

| File | Reason | Action |
|------|--------|--------|
| `development-rules.md` | Software development rules (YAGNI, KISS, DRY, file naming, pre-commit hooks) | **REMOVE** |

**Keep:**
- `primary-workflow.md` - Marketing campaign lifecycle
- `sales-workflow.md` - Sales process
- `crm-workflow.md` - CRM automation
- `marketing-rules.md` - Marketing rules
- `orchestration-protocol.md` - Agent orchestration
- `documentation-management.md` - Documentation management

---

### 2. Commands (`.claude/commands/`)

#### Development/Engineering Commands

| Path | Reason | Action |
|------|--------|--------|
| `/ask.md` | Technical/architectural questions for software engineering | **REMOVE** |
| `/brainstorm.md` | Software engineering brainstorming (YAGNI, KISS, DRY) | **UPDATE FOR MARKETING** |
| `/scout.md` | Codebase scouting for development | **REMOVE** |
| `/scout/ext.md` | External agentic tools for codebase exploration | **REMOVE** |
| `/watzup.md` | Review recent code changes | **REMOVE** |
| `/use-mcp.md` | Technical MCP protocol usage | **KEEP** |
| `/plan.md` | Generic planning (replace with campaign planning) | **REMOVE** |
| `/plan/fast.md` | Fast code planning | **REMOVE** |
| `/plan/hard.md` | Hard code planning | **REMOVE** |
| `/plan/two.md` | Two-approach code planning | **REMOVE** |

#### Git Commands

| Path | Reason | Action |
|------|--------|--------|
| `/git/cm.md` | Git commit | **REMOVE** |
| `/git/cp.md` | Git commit & push | **REMOVE** |
| `/git/pr.md` | Create pull request | **REMOVE** |

#### Technical Integration Commands

| Path | Reason | Action |
|------|--------|--------|
| `/integrate/polar.md` | Payment gateway integration (engineering) | **REMOVE** |
| `/integrate/sepay.md` | Payment gateway integration (engineering) | **REMOVE** |

#### Design/UI Commands (Engineering-Focused)

| Path | Reason | Action |
|------|--------|--------|
| `/design/fast.md` | Quick UI design (coding) | **REMOVE** |
| `/design/good.md` | Immersive UI design (coding) | **REMOVE** |
| `/design/screenshot.md` | Design from screenshot (coding) | **REMOVE** |
| `/design/video.md` | Design from video (coding) | **REMOVE** |
| `/design/describe.md` | Describe design (coding) | **REMOVE** |

#### Fix/Debug Commands

| Path | Reason | Action |
|------|--------|--------|
| `/fix.md` | Generic fix command (engineering) | **REMOVE** |
| `/fix/ui.md` | UI bug fixes (engineering) | **REMOVE** |
| `/fix/fast.md` | Fast fixes (engineering) | **REMOVE** |
| `/fix/hard.md` | Complex fixes (engineering) | **REMOVE** |

#### Documentation Commands (Code-Focused)

| Path | Reason | Action |
|------|--------|--------|
| `/docs/init.md` | Initialize codebase documentation | **REMOVE** |
| `/docs/summarize.md` | Summarize codebase | **REMOVE** |
| `/docs/update.md` | Update codebase documentation | **REMOVE** |

**Keep:** All marketing commands (campaign, content, seo, social, analytics, crm, leads, sales, sequence, ops, report, checklist, research, competitor, brand, audit)

---

### 3. Agents (`.claude/agents/`)

| File | Reason | Action |
|------|--------|--------|
| `ui-ux-designer.md` | Engineering-focused (Three.js, WebGL, coding, HTML/CSS/JS implementation) | **REMOVE** |
| `mcp-manager.md` | Technical MCP protocol integration | **KEEP** |
| `solopreneur.md` | Reviewer persona (should be in reviewers/ only) | **KEEP** |
| `startup-founder.md` | Reviewer persona (should be in reviewers/ only) | **KEEP** |
| `marketing-manager.md` | Check for duplication with other agents | **EVALUATE** |

**Note:** Reviewer personas (manager-maria, solo-steve, startup-sam) are already in `.claude/agents/reviewers/` (staged for commit).

**Keep:** All marketing agents (attraction-specialist, lead-qualifier, email-wizard, sales-enabler, continuity-specialist, upsell-maximizer, researcher, brainstormer, planner, project-manager, copywriter, docs-manager, brand-voice-guardian, conversion-optimizer, seo-specialist)

---

### 4. Skills (`.claude/skills/`)

#### Engineering/Development Skills

| Skill | Reason | Action |
|-------|--------|--------|
| `aesthetic/` | UI/UX design aesthetics for coding | **REMOVE** |
| `ai-multimodal/` | Gemini API for images/videos/audio (technical implementation) | **REMOVE** |
| `chrome-devtools/` | Browser automation with Puppeteer | **REMOVE** |
| `docs-seeker/` | Technical documentation search (context7.com) | **REMOVE** |
| `document-skills/` | DOCX, PDF, PPTX, XLSX manipulation (coding) | **KEEP** |
| `frontend-design/` | Frontend code design | **REMOVE** |
| `media-processing/` | FFmpeg/ImageMagick (engineering) | **REMOVE** |
| `mcp-management/` | MCP protocol management | **REMOVE** |
| `payment-integration/` | Polar/SePay payment gateways (engineering) | **REMOVE** |
| `planning/` | Code planning (codebase understanding, solution design) | **REMOVE** |
| `problem-solving/` | Engineering problem-solving patterns | **REMOVE** |
| `research/` | Generic research (redundant with researcher agent) | **REMOVE** |
| `sequential-thinking/` | Engineering thinking patterns | **REMOVE** |
| `shopify/` | Shopify app development (coding) | **EVALUATE** - Could be useful for Shopify marketing |
| `skill-creator/` | Meta skill for creating skills | **REMOVE** |
| `template-skill/` | Template skill | **REMOVE** |

#### Supporting Files

| File | Action |
|------|--------|
| `agent_skills_spec.md` | **REMOVE** - Engineering spec |
| `INSTALLATION.md` | **REMOVE** - Skills installation guide |
| `README.md` | **REMOVE** - Skills overview for engineering |
| `THIRD_PARTY_NOTICES.md` | **KEEP** - Legal compliance |
| `.env.example` | **REMOVE** - Engineering config |
| `payment-integration.tar.gz` | **REMOVE** - Archive file |

**Keep:** Marketing skills (marketing-fundamentals, seo-mastery, social-media, email-marketing, paid-advertising, content-strategy, analytics-attribution, brand-building)

**Note on Shopify:** Evaluate if marketers need Shopify integration. If yes, keep. If no, remove.

---

### 5. Documentation (docs/)

#### Engineering Documentation to Remove

| File | Reason | Action |
|------|--------|--------|
| `code-standards.md` | Software coding standards | **REMOVE** |
| `codebase-summary.md` | Codebase overview for engineering | **REMOVE** |
| `system-architecture.md` | Technical architecture | **REMOVE** |
| `mcp-servers-recommendation.md` | MCP server setup (technical) | **REMOVE** |

#### Marketing Documentation to Keep/Create

| File | Status | Action |
|------|--------|--------|
| `project-overview-pdr.md` | Existing | **REVIEW** - Ensure marketing-focused |
| `project-roadmap.md` | Existing | **REVIEW** - Ensure marketing-focused |
| `brand-guidelines.md` | Missing | **CREATE** |
| `content-style-guide.md` | Missing | **CREATE** |
| `campaign-playbooks.md` | Missing | **CREATE** |
| `channel-strategies.md` | Missing | **CREATE** |
| `analytics-setup.md` | Missing | **CREATE** |
| `agent-organization-update.md` | Existing | **KEEP** |
| `reviewer-agents-update.md` | Existing | **KEEP** |
| `usage-guide.md` | Existing | **KEEP** |

---

### 6. Other Files

#### Hooks (`.claude/hooks/`)

| File | Status | Action |
|------|--------|--------|
| `telegram-hook-setup.md` | Integration | **KEEP** - Useful for notifications |
| `discord-hook-setup.md` | Integration | **KEEP** - Useful for notifications |
| `README.md` | Documentation | **KEEP** |

#### Training Commands (`.claude/commands/training/`)

**All training commands** - **KEEP** - These are marketing-focused training modules.

---

## ✅ Cleanup Execution Steps

1. **Remove workflows**
   ```bash
   rm .claude/workflows/development-rules.md
   ```

2. **Remove commands**
   ```bash
   rm .claude/commands/ask.md
   rm .claude/commands/brainstorm.md
   rm .claude/commands/scout.md
   rm -rf .claude/commands/scout/
   rm .claude/commands/watzup.md
   rm .claude/commands/use-mcp.md
   rm .claude/commands/plan.md
   rm -rf .claude/commands/plan/
   rm -rf .claude/commands/git/
   rm -rf .claude/commands/integrate/
   rm -rf .claude/commands/design/
   rm .claude/commands/fix.md
   rm -rf .claude/commands/fix/
   rm -rf .claude/commands/docs/
   ```

3. **Remove agents**
   ```bash
   rm .claude/agents/ui-ux-designer.md
   rm .claude/agents/mcp-manager.md
   rm .claude/agents/solopreneur.md
   rm .claude/agents/startup-founder.md
   ```

4. **Remove skills**
   ```bash
   rm -rf .claude/skills/aesthetic/
   rm -rf .claude/skills/ai-multimodal/
   rm -rf .claude/skills/chrome-devtools/
   rm -rf .claude/skills/docs-seeker/
   rm -rf .claude/skills/document-skills/
   rm -rf .claude/skills/frontend-design/
   rm -rf .claude/skills/media-processing/
   rm -rf .claude/skills/mcp-management/
   rm -rf .claude/skills/payment-integration/
   rm -rf .claude/skills/planning/
   rm -rf .claude/skills/problem-solving/
   rm -rf .claude/skills/research/
   rm -rf .claude/skills/sequential-thinking/
   rm -rf .claude/skills/shopify/  # IF not needed
   rm -rf .claude/skills/skill-creator/
   rm -rf .claude/skills/template-skill/
   rm .claude/skills/agent_skills_spec.md
   rm .claude/skills/INSTALLATION.md
   rm .claude/skills/README.md
   rm .claude/skills/.env.example
   rm .claude/skills/payment-integration.tar.gz
   ```

5. **Remove engineering documentation**
   ```bash
   rm docs/code-standards.md
   rm docs/codebase-summary.md
   rm docs/system-architecture.md
   rm docs/mcp-servers-recommendation.md
   ```

6. **Update CLAUDE.md**
   - Remove references to removed agents (ui-ux-designer, mcp-manager)
   - Update skills catalog to only show marketing skills
   - Update documentation structure

7. **Update README.md**
   - Remove engineering-focused sections
   - Update documentation links
   - Focus on marketing workflows

---

## 📊 Impact Summary

### Before Cleanup
- **Workflows:** 7 (1 engineering-focused)
- **Commands:** ~100 (30+ engineering-focused)
- **Agents:** 20 (4 engineering-focused)
- **Skills:** 25+ (16 engineering-focused)
- **Docs:** 9 (4 engineering-focused)

### After Cleanup
- **Workflows:** 6 (100% marketing)
- **Commands:** ~70 (100% marketing)
- **Agents:** 16 (100% marketing)
- **Skills:** 8 (100% marketing)
- **Docs:** 11 (100% marketing)

### Reduction
- **~30% fewer files**
- **100% marketing focus**
- **Clearer system purpose**
- **Easier onboarding**
- **Better consistency**

---

## 🔍 Evaluation Needed

1. **Shopify Skill:** Do marketers need Shopify app development capabilities?
   - If YES (for Shopify marketing automation): Keep
   - If NO (marketers don't code Shopify apps): Remove

2. **Marketing Manager Agent:** Check if it duplicates responsibilities of other agents
   - Review agent definition
   - Compare with planner, project-manager agents
   - Decide: Keep, Merge, or Remove

---

## ✨ Next Steps After Cleanup

1. Create missing marketing documentation:
   - `docs/brand-guidelines.md`
   - `docs/content-style-guide.md`
   - `docs/campaign-playbooks.md`
   - `docs/channel-strategies.md`
   - `docs/analytics-setup.md`

2. Update `CLAUDE.md` with cleaned-up system

3. Update `README.md` to reflect marketing focus

4. Test all remaining commands to ensure they work

5. Update training modules if needed

6. Commit changes with clear message

---

**End of Cleanup Plan**
