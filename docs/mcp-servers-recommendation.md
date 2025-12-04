# MCP Servers Recommendation for Marketing Kit

## Overview

Model Context Protocol (MCP) servers enable AI assistants to securely connect to marketing tools, APIs, and data sources. This document outlines recommended MCP servers for our marketing kit, supporting **Global**, **Japan**, and **Vietnam** markets.

## Current Configuration

Already configured in `.claude/.mcp.json.example`:

| Category | Server | Status |
|----------|--------|--------|
| Analytics | Google Analytics, Search Console | Configured |
| Advertising | Google Ads, Meta Ads | Configured |
| Social | Twitter, LinkedIn, TikTok | Configured |
| CRM | HubSpot | Configured |
| Email | Mailchimp | Configured |
| SEO | Ahrefs, Semrush | Configured |
| Communication | Slack, Discord | Configured |
| Payments | Stripe | Configured |

---

## Recommended Additional MCP Servers

### Priority 1: Essential for Marketing Operations

#### 1. SE Ranking MCP
**Purpose**: SEO data, keyword research, backlink analysis
**Why Needed**: Alternative/complement to Ahrefs/Semrush with competitive pricing

```json
"se-ranking": {
  "command": "npx",
  "args": ["-y", "@seranking/seo-data-api-mcp-server"],
  "env": { "SE_RANKING_API_KEY": "YOUR_KEY" }
}
```

**GitHub**: [seranking/seo-data-api-mcp-server](https://github.com/seranking/seo-data-api-mcp-server)
**Use Cases**:
- Real-time keyword rankings
- Competitor backlink analysis
- Site audit automation

#### 2. DataForSEO MCP
**Purpose**: SERP data, keyword research, content analysis
**Why Needed**: Comprehensive SEO API access

```json
"dataforseo": {
  "command": "npx",
  "args": ["-y", "dataforseo-mcp-server"],
  "env": {
    "DATAFORSEO_LOGIN": "YOUR_LOGIN",
    "DATAFORSEO_PASSWORD": "YOUR_PASSWORD"
  }
}
```

**Source**: [PulseMCP - DataForSEO](https://www.pulsemcp.com/servers/dataforseo)
**Use Cases**:
- SERP analysis
- Keyword difficulty scoring
- Content gap analysis

#### 3. Notion MCP (Official)
**Purpose**: Content calendar, documentation, project management
**Why Needed**: Central content hub for marketing teams

```json
"notion": {
  "command": "npx",
  "args": ["-y", "@notionhq/notion-mcp-server"],
  "env": { "NOTION_API_KEY": "YOUR_KEY" }
}
```

**GitHub**: [makenotion/notion-mcp-server](https://github.com/makenotion/notion-mcp-server)
**Docs**: [Notion MCP](https://developers.notion.com/docs/mcp)
**Use Cases**:
- Content calendar management
- Campaign documentation
- Editorial workflow automation

#### 4. Asana MCP
**Purpose**: Task management, campaign tracking
**Why Needed**: Project management for marketing campaigns

```json
"asana": {
  "type": "sse",
  "url": "https://mcp.asana.com/sse"
}
```

**Docs**: [Asana MCP](https://developers.asana.com/docs/using-asanas-mcp-server)
**Use Cases**:
- Campaign task tracking
- Team collaboration
- Deadline management

#### 5. Metricool MCP
**Purpose**: Social media analytics & scheduling
**Why Needed**: Multi-platform social media management

```json
"metricool": {
  "command": "npx",
  "args": ["-y", "@metricool/mcp-server"],
  "env": { "METRICOOL_API_KEY": "YOUR_KEY" }
}
```

**Source**: [PulseMCP - Metricool](https://www.pulsemcp.com/servers/metricool-social-analytics)
**Use Cases**:
- Cross-platform analytics (Instagram, Facebook, Twitter, LinkedIn, TikTok, YouTube)
- Content scheduling
- Performance reporting

---

### Priority 2: Japan Market

#### 6. LINE Bot MCP Server (Official)
**Purpose**: LINE Official Account messaging & marketing
**Why Needed**: LINE has 97M+ monthly active users in Japan (94% smartphone reach)

```json
"line": {
  "command": "npx",
  "args": ["-y", "@line/line-bot-mcp-server"],
  "env": {
    "CHANNEL_ACCESS_TOKEN": "YOUR_TOKEN",
    "DESTINATION_USER_ID": "YOUR_DEFAULT_USER_ID"
  }
}
```

**GitHub**: [line/line-bot-mcp-server](https://github.com/line/line-bot-mcp-server)
**Docs**: [LINE Developers News](https://developers.line.biz/ja/news/2025/04/14/line-bot-mcp-server/)

**Tools Available**:
| Tool | Description |
|------|-------------|
| `push_text_message` | Send text to specific user |
| `push_flex_message` | Send rich flex messages |
| `broadcast_text_message` | Broadcast to all followers |
| `broadcast_flex_message` | Broadcast flex messages |
| `get_profile` | Get user profile info |

**Use Cases**:
- Customer engagement campaigns
- Promotional broadcasts
- 1-on-1 CRM communication
- Coupon distribution

#### 7. Yahoo Japan Ads (Manual Integration)
**Status**: No official MCP yet
**Workaround**: Use Yahoo Japan Marketing Solutions API directly

**Resources**:
- [Yahoo Japan Marketing Solutions](https://global-marketing.yahoo-net.jp/)
- API documentation available for campaign management

---

### Priority 3: Vietnam Market

#### 8. Zalo Integration
**Status**: No official MCP server available yet
**Market Context**: 70M+ active users in Vietnam (86.6% reach)

**Recommended Approach**:
1. **Zalo Official Account API** - Direct integration
2. **Custom MCP Server** - Build using Zalo Open API

**Zalo Official Account Features**:
- Broadcast messages
- Customer chat
- Zalo Pay integration
- CRM-linked campaigns

**Resources**:
- [Zalo Developers](https://developers.zalo.me/)
- [Zalo Official Account](https://oa.zalo.me/)

**Future Consideration**: Build custom MCP server for Zalo OA API

---

### Priority 4: Enhanced Capabilities

#### 9. Mailtrap MCP
**Purpose**: Email testing & deliverability
**Why Needed**: QA email campaigns before sending

```json
"mailtrap": {
  "command": "npx",
  "args": ["-y", "@mailtrap/mcp-server"],
  "env": { "MAILTRAP_API_TOKEN": "YOUR_TOKEN" }
}
```

**Use Cases**:
- Email template testing
- Deliverability optimization
- Spam score checking

#### 10. Apify Social Media Leads
**Purpose**: Lead generation from social platforms
**Why Needed**: Find prospects across 400+ platforms

```json
"apify-social": {
  "command": "npx",
  "args": ["-y", "@apify/social-media-leads-analyzer"],
  "env": { "APIFY_TOKEN": "YOUR_TOKEN" }
}
```

**Source**: [Apify MCP](https://apify.com/apify/social-media-leads-analyzer/api/mcp)
**Use Cases**:
- Lead discovery
- Competitor follower analysis
- Influencer identification

#### 11. Late API (Multi-Platform Scheduling)
**Purpose**: Schedule posts across 10 platforms
**Why Needed**: Unified social media scheduling

**Platforms**: Twitter, Instagram, TikTok, LinkedIn, Facebook, YouTube, Threads, Reddit, Pinterest, Bluesky

**Source**: [getlate.dev](https://getlate.dev)

---

## MCP Server Summary by Use Case

### SEO & Content

| Server | Features | Priority |
|--------|----------|----------|
| Ahrefs | Backlinks, keywords, site audit | Configured |
| Semrush | Keywords, competitors, content | Configured |
| SE Ranking | Rankings, audits, backlinks | Add |
| DataForSEO | SERP, keywords, content gaps | Add |
| Search Console | Performance, indexing | Configured |

### Social Media

| Server | Platforms | Priority |
|--------|-----------|----------|
| Twitter | X/Twitter | Configured |
| LinkedIn | LinkedIn | Configured |
| TikTok | TikTok | Configured |
| Meta Ads | Facebook, Instagram | Configured |
| Metricool | Multi-platform analytics | Add |
| LINE | Japan market | Add |

### CRM & Email

| Server | Features | Priority |
|--------|----------|----------|
| HubSpot | CRM, contacts, deals | Configured |
| Mailchimp | Email campaigns | Configured |
| Mailtrap | Email testing | Add |

### Project Management

| Server | Features | Priority |
|--------|----------|----------|
| Notion | Content calendar, docs | Add |
| Asana | Task management | Add |

### Advertising

| Server | Platforms | Priority |
|--------|-----------|----------|
| Google Ads | Search, Display, YouTube | Configured |
| Meta Ads | Facebook, Instagram | Configured |

---

## Regional Market Support

### Japan Market Stack

| Tool | MCP Status | Alternative |
|------|------------|-------------|
| LINE | Official MCP | - |
| Yahoo Japan | No MCP | Direct API |
| Twitter Japan | Use Twitter MCP | - |
| Instagram Japan | Use Meta Ads MCP | - |

### Vietnam Market Stack

| Tool | MCP Status | Alternative |
|------|------------|-------------|
| Zalo | No MCP | Custom build / Direct API |
| Facebook Vietnam | Use Meta Ads MCP | - |
| TikTok Vietnam | Use TikTok MCP | - |
| YouTube Vietnam | Use Google Ads | - |

### Global Stack

All configured MCP servers support global markets.

---

## Implementation Priority

### Phase 1: Immediate (Week 1)
1. LINE Bot MCP - Japan market essential
2. Notion MCP - Content calendar
3. SE Ranking or DataForSEO - SEO redundancy

### Phase 2: Short-term (Week 2-3)
4. Metricool - Social analytics
5. Asana - Project management
6. Mailtrap - Email QA

### Phase 3: Custom Development (Month 2+)
7. Zalo Custom MCP - Vietnam market
8. Yahoo Japan API integration

---

## Installation Commands

```bash
# SE Ranking
npm install -g @seranking/seo-data-api-mcp-server

# Notion (Official)
npm install -g @notionhq/notion-mcp-server

# LINE Bot (Official)
npm install -g @line/line-bot-mcp-server

# Or use npx (no install needed)
npx -y @line/line-bot-mcp-server
```

---

## Sources

### SEO & Analytics
- [Ahrefs MCP](https://ahrefs.com/blog/what-is-mcp-server/)
- [Semrush MCP](https://developer.semrush.com/api/basics/semrush-mcp/)
- [SE Ranking MCP](https://seranking.com/api/integrations/mcp/)
- [Google Analytics MCP](https://developers.google.com/analytics/devguides/MCP)

### Social Media
- [Metricool MCP](https://www.pulsemcp.com/servers/metricool-social-analytics)
- [Social Media MCP Guide](https://medium.com/data-science-in-your-pocket/best-social-media-mcp-servers-automate-social-media-using-ai-for-free-08eb8a75856e)

### Japan Market
- [LINE Bot MCP Server](https://github.com/line/line-bot-mcp-server)
- [LINE MCP Tech Blog](https://techblog.lycorp.co.jp/en/introduction-to-mcp-and-building-mcp-server-using-line-messaging-api)
- [Yahoo Japan Marketing](https://global-marketing.yahoo-net.jp/)

### Vietnam Market
- [Zalo Business](https://www.salesmartly.com/en/blog/docs/what-is-zalo)
- [Vietnam Social Media 2025](https://vectorgroup.vn/vietnam-social-media-trends-and-user-behavior-2025-update/)

### Project Management
- [Notion MCP](https://developers.notion.com/docs/mcp)
- [Asana MCP](https://developers.asana.com/docs/using-asanas-mcp-server)
- [HubSpot MCP](https://developers.hubspot.com/mcp)

### General
- [MCP Servers for Marketing](https://blog.coupler.io/mcp-servers/)
- [Digital Marketing MCP Guide](https://blackbearmedia.io/model-context-protocol-mcp-servers-for-digital-marketing/)
