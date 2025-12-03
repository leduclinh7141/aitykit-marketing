---
description: A/B testing framework for marketing optimization
argument-hint: [test-type] [element-to-test]
---

Activate `analytics-attribution`, `marketing-fundamentals`, `crm-workflow.md`, `sales-workflow.md` skills.

## Mission
Generate A/B testing plan:
<context>$ARGUMENTS</context>

## Agent Delegation
| Task | Agent | Trigger |
|------|-------|---------|
| Hypothesis creation | `brainstormer` | Test ideation |
| Copy variants | `copywriter` | Content testing |
| Analysis | `researcher` | Results review |
| Recommendations | `planner` | Next steps |

## Output Format
```markdown
# A/B Test Plan: [Test Name]

## Test Overview

| Field | Value |
|-------|-------|
| Test ID | [YYMMDD-001] |
| Element | [What's being tested] |
| Channel | [Email/Landing/Ad/etc] |
| Owner | [Name] |
| Start Date | [Date] |
| End Date | [Date] |
| Status | Planning/Running/Complete |

---

## Hypothesis

### Problem Statement
[What issue are you trying to solve?]

### Hypothesis
"If we [change X], then [metric Y] will [increase/decrease] because [reason Z]."

### Expected Outcome
- Primary metric: [Metric] will improve by [X%]
- Confidence: [High/Medium/Low]

---

## Test Design

### Control (A)
[Description of current/control version]

### Variant (B)
[Description of test variant]

### Variable Isolated
- **Testing:** [Single variable being changed]
- **Holding constant:** [Everything else]

### Sample Size Calculation
- Current conversion rate: [X%]
- Minimum detectable effect: [X%]
- Statistical significance: 95%
- Power: 80%
- **Required sample size:** [N per variant]

---

## Test Execution

### Pre-Test Checklist
- [ ] Hypothesis documented
- [ ] Success metrics defined
- [ ] Sample size calculated
- [ ] Test duration estimated
- [ ] Variants created
- [ ] QA completed on both variants
- [ ] Tracking verified
- [ ] Traffic split configured (50/50)
- [ ] Stakeholders informed

### During Test
- [ ] Monitor for technical issues
- [ ] Check traffic distribution
- [ ] Don't peek at results (wait for significance)
- [ ] Document any anomalies

### Post-Test
- [ ] Verify statistical significance reached
- [ ] Analyze primary metric
- [ ] Review secondary metrics
- [ ] Document learnings
- [ ] Implement winner
- [ ] Share results with team

---

## Results Template

### Primary Metric: [Metric Name]

| Variant | Visitors | Conversions | Rate | vs Control |
|---------|----------|-------------|------|------------|
| A (Control) | | | % | - |
| B (Variant) | | | % | +/-% |

### Statistical Analysis
- **Winner:** A / B / No winner
- **Confidence level:** [X%]
- **P-value:** [X]
- **Lift:** [+/-X%]

### Secondary Metrics

| Metric | Control | Variant | Change |
|--------|---------|---------|--------|
| [Metric 1] | | | |
| [Metric 2] | | | |
| [Metric 3] | | | |

---

## Common Tests by Channel

### Email Tests
| Element | Test Ideas |
|---------|------------|
| Subject line | Length, personalization, emoji, urgency |
| Preview text | Different hooks, CTAs |
| Sender name | Company vs person name |
| Send time | Day of week, time of day |
| CTA button | Color, text, placement |
| Content | Long vs short, images vs text |

### Landing Page Tests
| Element | Test Ideas |
|---------|------------|
| Headline | Benefit vs feature, question vs statement |
| Hero image | People vs product, video vs image |
| CTA button | Color, size, text, placement |
| Form length | Fields required, single vs multi-step |
| Social proof | Testimonials, logos, numbers |
| Page length | Short vs long form |

### Ad Tests
| Element | Test Ideas |
|---------|------------|
| Headline | Different value props |
| Description | Features vs benefits |
| Image/video | Different visuals |
| CTA | Different action words |
| Audience | Different targeting |
| Placement | Different platforms/positions |

---

## Testing Prioritization (ICE Framework)

| Test Idea | Impact (1-10) | Confidence (1-10) | Ease (1-10) | ICE Score |
|-----------|---------------|-------------------|-------------|-----------|
| | | | | |
| | | | | |
| | | | | |

**ICE Score = (Impact + Confidence + Ease) / 3**

Priority: Test highest ICE scores first.

---

## Testing Rules

### Do's
- Test one variable at a time
- Run until statistical significance
- Document everything
- Have clear hypothesis
- Define metrics upfront
- Use proper sample sizes

### Don'ts
- Don't stop tests early
- Don't peek and decide
- Don't test too many things
- Don't ignore segment data
- Don't forget to implement winners
- Don't test without hypothesis

### Minimum Test Duration
- Email: 24-48 hours (full send)
- Landing page: 2-4 weeks
- Ads: 1-2 weeks minimum
- Website: 2+ weeks

---

## Test Log

| ID | Element | Hypothesis | Winner | Lift | Date |
|----|---------|------------|--------|------|------|
| | | | | | |
| | | | | | |

---

## Learnings Library

### Proven Winners
- [Learning 1 with data]
- [Learning 2 with data]

### Failed Hypotheses
- [What we thought would work but didn't]

### Best Practices Discovered
- [Pattern that consistently works]
```
