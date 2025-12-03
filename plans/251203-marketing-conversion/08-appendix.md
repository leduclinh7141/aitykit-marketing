# Part 8: Appendix

## A. Reference Architecture

```
ClaudeKit Marketing Architecture

┌─────────────────────────────────────────────────────────────────┐
│                        CLAUDE.md (Entry Point)                  │
│                    Marketing Automation Kit                     │
└─────────────────────────────────────────────────────────────────┘
                                │
                ┌───────────────┴───────────────┐
                ▼                               ▼
┌───────────────────────┐       ┌───────────────────────────────┐
│      WORKFLOWS        │       │           AGENTS              │
│                       │       │                               │
│ • primary-workflow    │       │ Funnel Agents:                │
│   Research→Measure    │       │ • attraction-specialist       │
│                       │       │ • lead-qualifier              │
│ • marketing-rules     │       │ • email-wizard                │
│   Quality standards   │       │ • sales-enabler               │
│                       │       │ • continuity-specialist       │
│ • orchestration       │       │ • upsell-maximizer            │
│   Agent coordination  │       │                               │
└───────────────────────┘       │ Support Agents:               │
                                │ • researcher                  │
                                │ • brainstormer                │
                                │ • copywriter                  │
                                │ • planner                     │
                                │ • project-manager             │
                                └───────────────────────────────┘
                                                │
                ┌───────────────────────────────┴──────────────┐
                ▼                                              ▼
┌───────────────────────┐                     ┌───────────────────────┐
│      COMMANDS         │                     │        SKILLS         │
│                       │                     │                       │
│ /campaign:*           │                     │ marketing-fundamentals│
│ /seo:*                │                     │ seo-mastery           │
│ /leads:*              │                     │ social-media          │
│ /analytics:*          │                     │ email-marketing       │
│ /brand:*              │                     │ paid-advertising      │
│ /social:*             │                     │ content-strategy      │
│ /research:*           │                     │ analytics-attribution │
│ /content:*            │                     │ brand-building        │
└───────────────────────┘                     └───────────────────────┘
                                                        │
                                                        ▼
                                        ┌───────────────────────────┐
                                        │     MCP INTEGRATIONS      │
                                        │                           │
                                        │ • Meta Ads API            │
                                        │ • Google Ads API          │
                                        │ • GA4 / Search Console    │
                                        │ • Discord / Slack         │
                                        │ • Stripe / Payment        │
                                        │ • TikTok / Facebook       │
                                        │ • Meme Generator          │
                                        └───────────────────────────┘
```

---

## B. Marketing Funnel Mapping

```
┌─────────────────────────────────────────────────────────────────┐
│                      MARKETING FUNNEL                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  TOFU (Top of Funnel) ──────────────────────────────────────── │
│  │ Agent: attraction-specialist                                 │
│  │ Commands: /seo:*, /content:blog, /research:*                │
│  │ Goal: Awareness & Traffic                                   │
│  │                                                             │
│  ▼                                                             │
│  MOFU (Middle of Funnel) ─────────────────────────────────────│
│  │ Agents: lead-qualifier, email-wizard                        │
│  │ Commands: /leads:*, /content:email, /analytics:funnel       │
│  │ Goal: Engagement & Qualification                            │
│  │                                                             │
│  ▼                                                             │
│  BOFU (Bottom of Funnel) ─────────────────────────────────────│
│  │ Agent: sales-enabler                                        │
│  │ Commands: /content:landing, /content:ads, /campaign:*       │
│  │ Goal: Conversion & Purchase                                 │
│  │                                                             │
│  ▼                                                             │
│  POST-SALE ──────────────────────────────────────────────────│
│  │ Agents: continuity-specialist, upsell-maximizer             │
│  │ Commands: /social:engage, /analytics:roi                    │
│  │ Goal: Retention & Expansion                                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## C. Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/campaign:plan` | Campaign plan | planner |
| `/campaign:brief` | Creative brief | copywriter |
| `/campaign:calendar` | Content calendar | project-manager |
| `/campaign:analyze` | Performance analysis | researcher |
| `/seo:audit` | SEO audit | attraction-specialist |
| `/seo:keywords` | Keyword research | attraction-specialist |
| `/seo:competitor` | Competitor analysis | researcher |
| `/seo:optimize` | On-page optimization | copywriter |
| `/leads:qualify` | Lead qualification | lead-qualifier |
| `/leads:score` | Lead scoring | lead-qualifier |
| `/leads:nurture` | Nurture sequence | email-wizard |
| `/analytics:report` | Performance report | researcher |
| `/analytics:funnel` | Funnel analysis | lead-qualifier |
| `/analytics:roi` | ROI calculation | upsell-maximizer |
| `/brand:voice` | Voice guidelines | copywriter |
| `/brand:book` | Brand book | copywriter |
| `/brand:assets` | Asset management | project-manager |
| `/social:schedule` | Posting schedule | project-manager |
| `/social:engage` | Engagement strategy | continuity-specialist |
| `/social:viral` | Viral content | copywriter |
| `/research:market` | Market research | researcher |
| `/research:persona` | Buyer personas | lead-qualifier |
| `/research:trend` | Trend analysis | researcher |
| `/content:blog` | Blog posts | copywriter |
| `/content:social` | Social content | copywriter |
| `/content:email` | Email copy | email-wizard |
| `/content:landing` | Landing pages | copywriter |
| `/content:ads` | Ad copy | copywriter |
| `/content:cro` | CRO optimization | copywriter |

---

## D. Agent Delegation Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| New campaign | planner | researcher, copywriter |
| SEO content | attraction-specialist | copywriter |
| Email sequence | email-wizard | copywriter, lead-qualifier |
| Sales collateral | sales-enabler | copywriter |
| Churn prevention | continuity-specialist | email-wizard |
| Upsell campaign | upsell-maximizer | sales-enabler |
| Market research | researcher | attraction-specialist |
| Brand guidelines | copywriter | ui-ux-designer |

---

## E. MCP Integration Matrix

| Platform | Use Case | Required Credentials |
|----------|----------|---------------------|
| Meta Ads | Ad campaigns | META_ACCESS_TOKEN |
| Google Ads | Search/Display ads | GOOGLE_ADS_DEVELOPER_TOKEN |
| GA4 | Analytics | GA_PROPERTY_ID |
| Search Console | SEO data | GSC_SITE_URL |
| Discord | Community | DISCORD_BOT_TOKEN |
| Slack | Team comms | SLACK_BOT_TOKEN |
| Stripe | Payments | STRIPE_SECRET_KEY |
| TikTok | Social ads | TIKTOK_ACCESS_TOKEN |
| Meme Generator | Creative | None |

---

## F. Glossary

| Term | Definition |
|------|------------|
| TOFU | Top of Funnel - Awareness stage |
| MOFU | Middle of Funnel - Consideration stage |
| BOFU | Bottom of Funnel - Decision stage |
| CAC | Customer Acquisition Cost |
| LTV | Lifetime Value |
| ROAS | Return on Ad Spend |
| MQL | Marketing Qualified Lead |
| SQL | Sales Qualified Lead |
| CRO | Conversion Rate Optimization |
| ICP | Ideal Customer Profile |
| NPS | Net Promoter Score |
| RFM | Recency, Frequency, Monetary (segmentation) |

---

## G. Open Questions

1. **Content Hub Implementation**
   - Should R2 storage integration be a skill or MCP server?
   - How to handle asset versioning?

2. **AI Artist Integration**
   - Extend `ai-multimodal` skill or create separate `brand-artist` skill?
   - Gemini Imagen 4 vs other image generation options?

3. **Analytics Data Sources**
   - Which MCP servers are actually available vs need building?
   - How to handle rate limits and quotas?

4. **Existing Content Commands**
   - Keep `/content:cro` and `/content:enhance` as-is or restructure?
   - Merge with new content commands?

5. **Shopify Skill**
   - Keep for e-commerce marketing or remove as engineering-focused?
   - Add e-commerce specific commands?

---

**Document Status:** Ready for Review
**Next Action:** Await approval to proceed with implementation
