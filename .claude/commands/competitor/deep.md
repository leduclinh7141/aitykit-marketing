---
description: Deep competitor analysis with strategic insights
argument-hint: [competitor-name-or-url]
---

## Language & Quality Standards

**CRITICAL**: Respond in the same language the user is using. If Vietnamese, respond in Vietnamese. If Spanish, respond in Spanish.

**Standards**: Token efficiency, sacrifice grammar for concision, list unresolved questions at end.

**Skills**: Activate `marketing-fundamentals`, `seo-mastery` skills.

---

## Mission
Conduct deep competitor analysis:
<competitor>$ARGUMENTS</competitor>

## Workflow

1. Use `researcher` agent to analyze:
   - Company overview & positioning
   - Product/service offerings
   - Marketing channels & tactics
   - Content strategy
   - SEO performance

2. Use `attraction-specialist` agent for:
   - Keyword gap analysis
   - Backlink opportunities
   - Content gaps

3. Use `sales-enabler` agent to create:
   - Competitive battlecard
   - Win/loss patterns
   - Differentiation strategy

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Company research | `researcher` | Competitor profile |
| SEO analysis | `attraction-specialist` | Keyword gaps |
| Content analysis | `researcher` | Content strategy |
| Battlecard creation | `sales-enabler` | Sales enablement |
| Positioning review | `brainstormer` | Differentiation |

## Output Format
```markdown
# Competitor Analysis: [Competitor Name]
**URL:** [Website]
**Date:** [Date]

---

## Company Overview

### Profile
- **Founded:** [Year]
- **Size:** [Employees]
- **Funding:** [Amount/Stage]
- **HQ:** [Location]

### Positioning
- **Tagline:** "[Their tagline]"
- **Target market:** [Description]
- **Value proposition:** [Core promise]

### Products/Services
| Offering | Price Point | Target |
|----------|-------------|--------|
| [Product 1] | $X/mo | [Segment] |
| [Product 2] | $X/mo | [Segment] |

---

## Marketing Analysis

### Channel Presence
| Channel | Active | Strength |
|---------|--------|----------|
| Organic Search | ✅/❌ | 1-5 |
| Paid Search | ✅/❌ | 1-5 |
| Social (LinkedIn) | ✅/❌ | 1-5 |
| Social (Twitter) | ✅/❌ | 1-5 |
| Email | ✅/❌ | 1-5 |
| Content/Blog | ✅/❌ | 1-5 |

### Top Traffic Sources
1. [Source 1] - X%
2. [Source 2] - X%
3. [Source 3] - X%

### Messaging Themes
- [Theme 1]
- [Theme 2]
- [Theme 3]

---

## SEO Analysis

### Domain Metrics
- Domain Authority: X
- Organic traffic: X/mo
- Keywords ranking: X
- Backlinks: X

### Top Keywords
| Keyword | Position | Volume | Our Position |
|---------|----------|--------|--------------|
| [KW 1] | X | X | X |
| [KW 2] | X | X | X |
| [KW 3] | X | X | X |

### Content Strategy
- Publishing frequency: X/week
- Avg word count: X
- Top content types: [Types]
- Top performing topics: [Topics]

---

## Social Media

| Platform | Followers | Engagement | Post Freq |
|----------|-----------|------------|-----------|
| LinkedIn | X | X% | X/wk |
| Twitter | X | X% | X/wk |
| Instagram | X | X% | X/wk |

### Content Themes
- [Theme 1]
- [Theme 2]

---

## Strengths & Weaknesses

### Their Strengths
1. **[Strength 1]:** [Details]
2. **[Strength 2]:** [Details]
3. **[Strength 3]:** [Details]

### Their Weaknesses
1. **[Weakness 1]:** [Opportunity for us]
2. **[Weakness 2]:** [Opportunity for us]
3. **[Weakness 3]:** [Opportunity for us]

---

## Competitive Battlecard

### Quick Comparison
| Factor | Us | Them |
|--------|-----|------|
| Price | $X | $X |
| [Feature 1] | ✅/❌ | ✅/❌ |
| [Feature 2] | ✅/❌ | ✅/❌ |
| [Feature 3] | ✅/❌ | ✅/❌ |

### Counter Their Strengths
- **They say:** "[Claim]"
- **We counter:** "[Response]"

### Exploit Their Weaknesses
- **Gap:** [Their weakness]
- **Our advantage:** [Our strength]
- **Proof point:** [Evidence]

### Trap Questions
1. "Ask them about [weakness area]"
2. "How do they handle [our strength]?"

---

## Opportunities

### Keyword Gaps (They rank, we don't)
| Keyword | Their Pos | Volume | Difficulty |
|---------|-----------|--------|------------|
| [KW 1] | X | X | Easy/Med/Hard |
| [KW 2] | X | X | Easy/Med/Hard |

### Content Gaps
- [Topic they cover well that we don't]
- [Format they use that we don't]

### Backlink Opportunities
- [Site linking to them, not us]
- [Industry directory they're in]

---

## Strategic Recommendations

1. **[Recommendation 1]:** [Action + expected impact]
2. **[Recommendation 2]:** [Action + expected impact]
3. **[Recommendation 3]:** [Action + expected impact]

### Win Scenarios
- We win when: [Scenario]
- They win when: [Scenario]
```
