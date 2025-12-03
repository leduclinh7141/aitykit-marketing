# Part 2: Agent Specifications

## 2.1 Agent Overview

| Agent | Function | Model |
|-------|----------|-------|
| **product-manager** | Catalog & listings | sonnet |
| **inventory-optimizer** | Stock & fulfillment | sonnet |
| **customer-service** | Support & inquiries | sonnet |
| **marketing-automator** | Campaigns & promotions | sonnet |
| **sales-analyst** | Revenue & performance | sonnet |
| **order-processor** | Orders & shipping | haiku |

---

## 2.2 Product Manager

**File:** `.claude/agents/product-manager.md`

```yaml
---
name: product-manager
description: Product catalog and listing specialist. Use for writing product descriptions, optimizing titles, managing categories, and bulk catalog updates. Handles SEO and marketplace optimization.
model: sonnet
---
```

### Core Capabilities

- **Product Descriptions**: Compelling, SEO-optimized copy
- **Title Optimization**: Platform-specific titles
- **Category Management**: Taxonomy and organization
- **Bulk Updates**: Mass catalog operations
- **SEO Optimization**: Keywords, meta data
- **Marketplace Listing**: Amazon, eBay optimization

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Product Listing | Markdown | New products |
| Bulk Update | CSV | Mass changes |
| SEO Report | Markdown | Optimization |
| Category Structure | Table | Organization |

### Skills Used

- `product-catalog` - Catalog management
- `ecommerce-seo` - Search optimization
- `copywriting` - Product copy

---

## 2.3 Inventory Optimizer

**File:** `.claude/agents/inventory-optimizer.md`

```yaml
---
name: inventory-optimizer
description: Inventory and fulfillment specialist. Use for stock level management, reorder point calculation, demand forecasting, and supplier coordination. Handles inventory optimization and warehouse efficiency.
model: sonnet
---
```

### Core Capabilities

- **Stock Management**: Level monitoring, alerts
- **Demand Forecasting**: Predictive inventory
- **Reorder Points**: Optimal reorder calculation
- **Supplier Management**: PO generation, coordination
- **Multi-location**: Warehouse optimization
- **Dead Stock**: Identification and clearance

### Key Metrics

| Metric | Description |
|--------|-------------|
| Stock Levels | Current inventory by SKU |
| Turnover Rate | How fast stock sells |
| Stockout Rate | Out-of-stock frequency |
| Carrying Cost | Cost to hold inventory |
| Reorder Point | When to reorder |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Inventory Report | Table | Status check |
| Reorder List | Table | Purchasing |
| Forecast | Markdown | Planning |
| Clearance Plan | Markdown | Dead stock |

### Skills Used

- `inventory-management` - Stock control
- `demand-forecasting` - Predictions
- `supply-chain` - Supplier management

---

## 2.4 Customer Service

**File:** `.claude/agents/customer-service.md`

```yaml
---
name: customer-service
description: Customer support specialist. Use for answering inquiries, handling complaints, processing returns, and escalating issues. Handles pre-sale questions and post-purchase support.
model: sonnet
---
```

### Core Capabilities

- **Inquiry Response**: Product questions, FAQs
- **Order Support**: Status, tracking, changes
- **Returns/Refunds**: Process management
- **Complaint Handling**: Resolution, compensation
- **Escalation**: Complex issue routing
- **Review Response**: Public review management

### Support Types

| Type | Response Time | Priority |
|------|---------------|----------|
| Pre-sale | < 2 hrs | Medium |
| Order status | < 1 hr | High |
| Returns | < 4 hrs | High |
| Complaints | < 2 hrs | Critical |
| General | < 24 hrs | Low |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Response | Text | Customer reply |
| FAQ | Markdown | Knowledge base |
| Escalation | Ticket | Complex issues |
| Report | Markdown | Support metrics |

### Skills Used

- `customer-support` - Service excellence
- `returns-management` - RMA process
- `conflict-resolution` - Complaints

---

## 2.5 Marketing Automator

**File:** `.claude/agents/marketing-automator.md`

```yaml
---
name: marketing-automator
description: Marketing and promotions specialist. Use for email campaigns, ad copy, promotional planning, and customer segmentation. Handles lifecycle marketing and retention.
model: sonnet
---
```

### Core Capabilities

- **Email Campaigns**: Flows, broadcasts
- **Ad Copy**: Social ads, Google ads
- **Promotions**: Sales, discounts, bundles
- **Segmentation**: Customer grouping
- **Lifecycle Marketing**: Welcome, winback, VIP
- **A/B Testing**: Campaign optimization

### Campaign Types

| Type | Trigger | Goal |
|------|---------|------|
| Welcome | New subscriber | Convert |
| Abandoned Cart | Cart left | Recover |
| Post-Purchase | Order placed | Repeat |
| Winback | Inactive | Re-engage |
| VIP | High value | Retain |
| Promotion | Scheduled | Revenue |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Email Campaign | Markdown | Automation |
| Ad Copy | Markdown | Advertising |
| Promo Plan | Markdown | Planning |
| Segment | Table | Targeting |

### Skills Used

- `email-marketing` - Email automation
- `paid-advertising` - Ad campaigns
- `promotions` - Sales planning

---

## 2.6 Sales Analyst

**File:** `.claude/agents/sales-analyst.md`

```yaml
---
name: sales-analyst
description: Sales analytics and insights specialist. Use for revenue reporting, performance analysis, trend identification, and forecasting. Handles business intelligence and data-driven recommendations.
model: sonnet
---
```

### Core Capabilities

- **Revenue Reporting**: Sales dashboards
- **Performance Analysis**: Product, channel, customer
- **Trend Identification**: Patterns, seasonality
- **Forecasting**: Revenue predictions
- **Cohort Analysis**: Customer behavior
- **Attribution**: Marketing ROI

### Key Reports

| Report | Frequency | Audience |
|--------|-----------|----------|
| Daily Sales | Daily | Operations |
| Weekly Performance | Weekly | Management |
| Monthly P&L | Monthly | Leadership |
| Product Performance | Weekly | Merchandising |
| Customer Analysis | Monthly | Marketing |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Sales Report | Markdown/Table | Review |
| Dashboard | Table | Monitoring |
| Forecast | Markdown | Planning |
| Analysis | Markdown | Insights |

### Skills Used

- `ecommerce-analytics` - Metrics
- `data-analysis` - Insights
- `forecasting` - Predictions

---

## 2.7 Order Processor

**File:** `.claude/agents/order-processor.md`

```yaml
---
name: order-processor
description: Order management and fulfillment specialist. Use for order processing, shipping coordination, tracking updates, and fulfillment optimization. Handles order lifecycle management.
model: haiku
---
```

### Core Capabilities

- **Order Processing**: Validation, routing
- **Shipping Coordination**: Carrier selection
- **Tracking Updates**: Status notifications
- **Exception Handling**: Issues, holds
- **Bulk Operations**: Mass processing
- **Fulfillment Rules**: Routing logic

### Order Statuses

| Status | Description |
|--------|-------------|
| Pending | Awaiting payment |
| Processing | Being prepared |
| Shipped | In transit |
| Delivered | Complete |
| Returned | RMA initiated |
| Cancelled | Voided |

### Output Formats

| Output | Format | Use Case |
|--------|--------|----------|
| Order Status | Text | Updates |
| Shipping Label | Integration | Fulfillment |
| Tracking | Text | Customer |
| Exception Report | Table | Operations |

### Skills Used

- `order-management` - Processing
- `shipping` - Fulfillment
- `exception-handling` - Issues

---

## 2.8 Agent Interaction Matrix

| Scenario | Primary Agent | Supporting Agents |
|----------|---------------|-------------------|
| New product | product-manager | inventory-optimizer |
| Stock alert | inventory-optimizer | order-processor |
| Customer inquiry | customer-service | order-processor |
| Campaign launch | marketing-automator | sales-analyst |
| Performance review | sales-analyst | marketing-automator |
| Order issue | order-processor | customer-service |
