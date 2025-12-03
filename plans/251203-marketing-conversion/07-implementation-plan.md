# Part 7: Implementation Plan

## 7.1 Implementation Phases

### Phase 1: Foundation (Priority: HIGH)

| Task | File | Action |
|------|------|--------|
| Update CLAUDE.md | `CLAUDE.md` | MODIFY |
| Update metadata.json | `.claude/metadata.json` | MODIFY |
| Create primary-workflow.md | `.claude/workflows/primary-workflow.md` | REPLACE |
| Create marketing-rules.md | `.claude/workflows/marketing-rules.md` | CREATE |
| Update orchestration-protocol.md | `.claude/workflows/orchestration-protocol.md` | MODIFY |
| Update .mcp.json.example | `.claude/.mcp.json.example` | MODIFY |
| Update README.md | `README.md` | MODIFY |

**Files:** 7

---

### Phase 2: Agents (Priority: HIGH)

| Task | File | Action |
|------|------|--------|
| Create attraction-specialist | `.claude/agents/attraction-specialist.md` | CREATE |
| Create lead-qualifier | `.claude/agents/lead-qualifier.md` | CREATE |
| Create email-wizard | `.claude/agents/email-wizard.md` | CREATE |
| Create sales-enabler | `.claude/agents/sales-enabler.md` | CREATE |
| Create continuity-specialist | `.claude/agents/continuity-specialist.md` | CREATE |
| Create upsell-maximizer | `.claude/agents/upsell-maximizer.md` | CREATE |
| Adapt researcher.md | `.claude/agents/researcher.md` | MODIFY |
| Adapt brainstormer.md | `.claude/agents/brainstormer.md` | MODIFY |
| Adapt planner.md | `.claude/agents/planner.md` | MODIFY |
| Adapt project-manager.md | `.claude/agents/project-manager.md` | MODIFY |

**Files:** 10

---

### Phase 3: Commands (Priority: HIGH)

| Task | Files | Action |
|------|-------|--------|
| Create /campaign/* | 4 files | CREATE |
| Create /seo/* | 4 files | CREATE |
| Create /leads/* | 3 files | CREATE |
| Create /analytics/* | 3 files | CREATE |
| Create /brand/* | 3 files | CREATE |
| Create /social/* | 3 files | CREATE |
| Create /research/* | 3 files | CREATE |
| Enhance /content/* | 5 files | CREATE |

**Files:** 28

---

### Phase 4: Skills (Priority: MEDIUM)

| Task | Files | Action |
|------|-------|--------|
| Create marketing-fundamentals | 5 files | CREATE |
| Create seo-mastery | 6 files | CREATE |
| Create social-media | 5 files | CREATE |
| Create email-marketing | 5 files | CREATE |
| Create paid-advertising | 5 files | CREATE |
| Create content-strategy | 5 files | CREATE |
| Create analytics-attribution | 5 files | CREATE |
| Create brand-building | 5 files | CREATE |

**Files:** 41

---

### Phase 5: Cleanup (Priority: LOW)

| Task | Files | Action |
|------|-------|--------|
| Remove engineering agents | 8 files | DELETE |
| Remove engineering commands | ~15 dirs/files | DELETE |
| Remove engineering skills | 9 directories | DELETE |

**Files:** ~32 (deletions)

---

## 7.2 File Inventory

### Files to CREATE

```
.claude/agents/
├── attraction-specialist.md
├── lead-qualifier.md
├── email-wizard.md
├── sales-enabler.md
├── continuity-specialist.md
└── upsell-maximizer.md

.claude/commands/
├── campaign/
│   ├── plan.md
│   ├── brief.md
│   ├── calendar.md
│   └── analyze.md
├── seo/
│   ├── audit.md
│   ├── keywords.md
│   ├── competitor.md
│   └── optimize.md
├── leads/
│   ├── qualify.md
│   ├── score.md
│   └── nurture.md
├── analytics/
│   ├── report.md
│   ├── funnel.md
│   └── roi.md
├── brand/
│   ├── voice.md
│   ├── book.md
│   └── assets.md
├── social/
│   ├── schedule.md
│   ├── engage.md
│   └── viral.md
├── research/
│   ├── market.md
│   ├── persona.md
│   └── trend.md
└── content/
    ├── blog.md
    ├── social.md
    ├── email.md
    ├── landing.md
    └── ads.md

.claude/skills/
├── marketing-fundamentals/
│   ├── SKILL.md
│   └── references/
│       ├── funnel-psychology.md
│       ├── conversion-principles.md
│       ├── copywriting-frameworks.md
│       └── marketing-metrics.md
├── seo-mastery/
│   ├── SKILL.md
│   └── references/
│       ├── keyword-research.md
│       ├── on-page-seo.md
│       ├── technical-seo.md
│       ├── link-building.md
│       └── local-seo.md
├── social-media/
│   ├── SKILL.md
│   └── references/
│       ├── platform-algorithms.md
│       ├── content-formats.md
│       ├── engagement-tactics.md
│       └── viral-mechanics.md
├── email-marketing/
│   ├── SKILL.md
│   └── references/
│       ├── sequence-design.md
│       ├── deliverability.md
│       ├── segmentation.md
│       └── automation.md
├── paid-advertising/
│   ├── SKILL.md
│   └── references/
│       ├── meta-ads.md
│       ├── google-ads.md
│       ├── linkedin-ads.md
│       └── tiktok-ads.md
├── content-strategy/
│   ├── SKILL.md
│   └── references/
│       ├── content-pillars.md
│       ├── editorial-calendar.md
│       ├── repurposing.md
│       └── distribution.md
├── analytics-attribution/
│   ├── SKILL.md
│   └── references/
│       ├── google-analytics.md
│       ├── search-console.md
│       ├── attribution-models.md
│       └── dashboards.md
└── brand-building/
    ├── SKILL.md
    └── references/
        ├── brand-strategy.md
        ├── visual-identity.md
        ├── voice-tone.md
        └── positioning.md

.claude/workflows/
└── marketing-rules.md
```

### Files to MODIFY

```
CLAUDE.md
README.md
.claude/metadata.json
.claude/.mcp.json.example
.claude/workflows/primary-workflow.md
.claude/workflows/orchestration-protocol.md
.claude/agents/researcher.md
.claude/agents/brainstormer.md
.claude/agents/planner.md
.claude/agents/project-manager.md
.claude/agents/copywriter.md (minor)
.claude/agents/ui-ux-designer.md
```

### Files to DELETE

```
.claude/agents/
├── code-reviewer.md
├── database-admin.md
├── debugger.md
├── git-manager.md
├── journal-writer.md
├── scout.md
├── scout-external.md
└── tester.md

.claude/commands/
├── bootstrap/
├── cook/
├── debug.md
├── fix/
├── git/
├── review/
├── scout/
├── code.md
├── test.md
└── watzup.md

.claude/skills/
├── backend-development/
├── claude-code/
├── code-review/
├── databases/
├── debugging/
├── devops/
├── frontend-development/
├── mobile-development/
└── ui-styling/
```

---

## 7.3 Validation Criteria

### Success Metrics

| Metric | Target |
|--------|--------|
| Agent Coverage | All 6 funnel agents operational |
| Command Coverage | All 28 marketing commands functional |
| Skill Coverage | All 8 marketing skills with references |
| Workflow Integrity | Pipeline executes correctly |
| MCP Integration | Template includes 10+ platforms |

### Testing Checklist

- [ ] Each agent responds to appropriate triggers
- [ ] Each command produces expected output format
- [ ] Skills are activated in relevant contexts
- [ ] Workflow phases chain correctly
- [ ] MCP servers connect (with valid credentials)
- [ ] No orphaned references to removed components

---

## 7.4 Risk Assessment

### Technical Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| Breaking existing workflows | HIGH | Create backup before changes |
| MCP packages not available | MEDIUM | Create placeholder configs |
| Skill references broken | MEDIUM | Validate all file paths |
| Agent conflicts | LOW | Test agent delegation chains |

### Content Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| Incomplete skill references | MEDIUM | Prioritize core content |
| Inconsistent voice | LOW | Create style guide |
| Missing edge cases | LOW | Iterative improvement |
