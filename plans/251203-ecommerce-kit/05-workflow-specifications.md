# Part 5: Workflow & Configuration Specifications

## 5.1 Primary E-commerce Workflow

**File:** `.claude/workflows/primary-workflow.md`

```markdown
# Primary E-commerce Workflow

## Operations Cycle

Catalog → Inventory → Orders → Support → Marketing → Analytics

### Phase 1: Catalog
- Delegate to `product-manager` for listings
- Use `product-catalog` skill
- Output: Optimized product listings

### Phase 2: Inventory
- Delegate to `inventory-optimizer` for stock
- Use `inventory-management` skill
- Output: Optimal stock levels

### Phase 3: Orders
- Delegate to `order-processor` for fulfillment
- Process, ship, track orders
- Output: Fulfilled orders

### Phase 4: Support
- Delegate to `customer-service` for inquiries
- Use `customer-support` skill
- Output: Resolved tickets, happy customers

### Phase 5: Marketing
- Delegate to `marketing-automator` for campaigns
- Use `ecommerce-marketing` skill
- Output: Revenue-driving campaigns

### Phase 6: Analytics
- Delegate to `sales-analyst` for insights
- Use `sales-analytics` skill
- Output: Data-driven decisions
```

---

## 5.2 E-commerce Rules

**File:** `.claude/workflows/ecommerce-rules.md`

```markdown
# E-commerce Rules

## Product Standards
- Accurate product descriptions
- High-quality images
- Correct pricing and inventory
- Clear shipping information

## Order Standards
- Process orders within 24 hours
- Ship within stated timeframe
- Provide tracking immediately
- Handle exceptions promptly

## Support Standards
- Respond within 24 hours
- Resolve issues fairly
- Follow return policy
- Escalate appropriately

## Marketing Standards
- Honor all promotions
- Comply with CAN-SPAM
- Accurate advertising
- Respect opt-outs

## Data Standards
- Protect customer data
- Comply with GDPR/CCPA
- Secure payment info
- Maintain accurate records
```

---

## 5.3 Orchestration Protocol

**File:** `.claude/workflows/orchestration-protocol.md`

```markdown
# E-commerce Agent Orchestration

## Sequential Workflows

### Order Flow
order-processor → inventory-optimizer → customer-service
1. Process and fulfill order
2. Update inventory levels
3. Send customer updates

### Launch Flow
product-manager → inventory-optimizer → marketing-automator
1. Create product listings
2. Set up inventory tracking
3. Launch marketing campaign

## Parallel Workflows

### Daily Operations
- order-processor: Process pending orders
- customer-service: Handle tickets
- inventory-optimizer: Check stock alerts
→ Daily operations report

### Weekly Review
- sales-analyst: Performance analysis
- marketing-automator: Campaign review
- inventory-optimizer: Stock planning
→ Weekly business review

## Agent Handoffs

| Trigger | From | To |
|---------|------|-----|
| New product | product-manager | inventory-optimizer |
| Low stock | inventory-optimizer | marketing-automator |
| Order placed | order-processor | customer-service |
| Order issue | customer-service | order-processor |
| Campaign end | marketing-automator | sales-analyst |
| Insights ready | sales-analyst | marketing-automator |
```

---

## 5.4 Configuration Files

### metadata.json

```json
{
  "version": "1.0.0",
  "name": "claudekit-ecommerce",
  "description": "AI-powered e-commerce kit with specialized agents for product management, inventory, customer service, marketing, analytics, and order processing.",
  "buildDate": "2025-12-03T00:00:00.000Z",
  "repository": {
    "type": "git",
    "url": "https://github.com/claudekit/claudekit-ecommerce.git"
  }
}
```

### CLAUDE.md

```markdown
# CLAUDE.md

## Role & Responsibilities

Your role is to assist e-commerce businesses with catalog management, inventory, customer service, marketing, and analytics while maximizing revenue and customer satisfaction.

## Workflows

- Primary workflow: `./.claude/workflows/primary-workflow.md`
- E-commerce rules: `./.claude/workflows/ecommerce-rules.md`
- Orchestration: `./.claude/workflows/orchestration-protocol.md`

## E-commerce Agents

- `product-manager` - Catalog & listings
- `inventory-optimizer` - Stock & fulfillment
- `customer-service` - Support
- `marketing-automator` - Campaigns
- `sales-analyst` - Analytics
- `order-processor` - Orders

## Skills Catalog

- `product-catalog` - Listings, SEO
- `inventory-management` - Stock control
- `customer-support` - Service
- `ecommerce-marketing` - Campaigns
- `sales-analytics` - Insights
```

### .mcp.json.example

```json
{
  "mcpServers": {
    "shopify": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-shopify"],
      "env": { "SHOPIFY_ACCESS_TOKEN": "YOUR_TOKEN", "SHOPIFY_STORE": "YOUR_STORE" }
    },
    "woocommerce": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-woocommerce"],
      "env": { "WC_URL": "YOUR_URL", "WC_KEY": "YOUR_KEY", "WC_SECRET": "YOUR_SECRET" }
    },
    "amazon": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-amazon-sp"],
      "env": { "AMAZON_REFRESH_TOKEN": "YOUR_TOKEN" }
    },
    "stripe": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-stripe"],
      "env": { "STRIPE_API_KEY": "YOUR_KEY" }
    },
    "klaviyo": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-klaviyo"],
      "env": { "KLAVIYO_API_KEY": "YOUR_KEY" }
    },
    "shipstation": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-shipstation"],
      "env": { "SHIPSTATION_API_KEY": "YOUR_KEY", "SHIPSTATION_API_SECRET": "YOUR_SECRET" }
    },
    "gorgias": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-gorgias"],
      "env": { "GORGIAS_DOMAIN": "YOUR_DOMAIN", "GORGIAS_API_KEY": "YOUR_KEY" }
    },
    "google-analytics": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-analytics"],
      "env": { "GA_CREDENTIALS": "YOUR_CREDS" }
    },
    "facebook-ads": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-facebook-ads"],
      "env": { "FB_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "google-ads": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-google-ads"],
      "env": { "GOOGLE_ADS_CREDENTIALS": "YOUR_CREDS" }
    },
    "quickbooks": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-quickbooks"],
      "env": { "QB_ACCESS_TOKEN": "YOUR_TOKEN" }
    },
    "slack": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-slack"],
      "env": { "SLACK_BOT_TOKEN": "YOUR_TOKEN" }
    },
    "yotpo": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-yotpo"],
      "env": { "YOTPO_API_KEY": "YOUR_KEY" }
    },
    "cin7": {
      "command": "npx",
      "args": ["-y", "@claudekit/mcp-cin7"],
      "env": { "CIN7_API_KEY": "YOUR_KEY" }
    }
  }
}
```

---

## 5.5 MCP Integration Summary

| Integration | Purpose | Priority |
|-------------|---------|----------|
| Shopify | E-commerce platform | HIGH |
| WooCommerce | E-commerce platform | HIGH |
| Amazon SP | Marketplace | HIGH |
| Stripe | Payments | HIGH |
| Klaviyo | Email marketing | HIGH |
| ShipStation | Shipping | HIGH |
| Gorgias | Customer support | MEDIUM |
| Google Analytics | Analytics | HIGH |
| Facebook Ads | Advertising | MEDIUM |
| Google Ads | Advertising | MEDIUM |
| QuickBooks | Accounting | MEDIUM |
| Slack | Notifications | LOW |
| Yotpo | Reviews | LOW |
| Cin7 | Inventory | MEDIUM |
