# Part 3: Command Specifications

## 3.1 Command Structure

```
.claude/commands/
├── product/
│   ├── create.md          # /product:create
│   ├── optimize.md        # /product:optimize
│   ├── bulk.md            # /product:bulk
│   ├── seo.md             # /product:seo
│   └── marketplace.md     # /product:marketplace
├── inventory/
│   ├── status.md          # /inventory:status
│   ├── forecast.md        # /inventory:forecast
│   ├── reorder.md         # /inventory:reorder
│   └── clearance.md       # /inventory:clearance
├── support/
│   ├── respond.md         # /support:respond
│   ├── return.md          # /support:return
│   ├── escalate.md        # /support:escalate
│   └── review.md          # /support:review
├── marketing/
│   ├── email.md           # /marketing:email
│   ├── ad.md              # /marketing:ad
│   ├── promo.md           # /marketing:promo
│   ├── segment.md         # /marketing:segment
│   └── flow.md            # /marketing:flow
├── analytics/
│   ├── sales.md           # /analytics:sales
│   ├── product.md         # /analytics:product
│   ├── customer.md        # /analytics:customer
│   └── forecast.md        # /analytics:forecast
└── order/
    ├── process.md         # /order:process
    ├── track.md           # /order:track
    ├── fulfill.md         # /order:fulfill
    └── exception.md       # /order:exception
```

---

## 3.2 Product Commands

### /product:create
```yaml
---
description: Create product listing with optimized content
argument-hint: [product-info] [platform]
---
```

**Workflow:**
1. Gather product details
2. Write compelling description
3. Optimize title for platform
4. Add SEO elements
5. Output complete listing

**Agent:** `product-manager`

---

### /product:optimize
```yaml
---
description: Optimize existing product listing
argument-hint: [product-id] [optimization-focus]
---
```

**Workflow:**
1. Analyze current listing
2. Identify improvement areas
3. Rewrite/enhance content
4. Update SEO elements
5. Output optimized listing

**Agent:** `product-manager`

---

### /product:bulk
```yaml
---
description: Bulk update product catalog
argument-hint: [update-type] [products]
---
```

**Workflow:**
1. Parse update requirements
2. Generate updates for all products
3. Validate changes
4. Create import file
5. Output bulk update file

**Agent:** `product-manager`

---

### /product:seo
```yaml
---
description: Optimize product SEO
argument-hint: [product-id] [keywords]
---
```

**Workflow:**
1. Research keywords
2. Optimize title
3. Enhance description
4. Add meta data
5. Output SEO package

**Agent:** `product-manager`

---

### /product:marketplace
```yaml
---
description: Optimize listing for marketplace
argument-hint: [product] [marketplace]
---
```

**Workflow:**
1. Understand marketplace requirements
2. Adapt content for platform
3. Optimize for search
4. Add required attributes
5. Output marketplace listing

**Agent:** `product-manager`

---

## 3.3 Inventory Commands

### /inventory:status
```yaml
---
description: Generate inventory status report
argument-hint: [scope] [filters]
---
```

**Workflow:**
1. Pull inventory data
2. Calculate key metrics
3. Identify low stock
4. Flag issues
5. Output status report

**Agent:** `inventory-optimizer`

---

### /inventory:forecast
```yaml
---
description: Forecast inventory needs
argument-hint: [products] [period]
---
```

**Workflow:**
1. Analyze sales history
2. Factor seasonality
3. Calculate demand forecast
4. Recommend stock levels
5. Output forecast report

**Agent:** `inventory-optimizer`

---

### /inventory:reorder
```yaml
---
description: Generate reorder recommendations
argument-hint: [threshold] [lead-time]
---
```

**Workflow:**
1. Check current levels
2. Calculate reorder points
3. Factor lead times
4. Generate PO suggestions
5. Output reorder list

**Agent:** `inventory-optimizer`

---

### /inventory:clearance
```yaml
---
description: Identify and plan clearance for slow stock
argument-hint: [criteria]
---
```

**Workflow:**
1. Identify slow-moving stock
2. Calculate holding costs
3. Recommend discounts
4. Create clearance plan
5. Output clearance strategy

**Agent:** `inventory-optimizer`

---

## 3.4 Support Commands

### /support:respond
```yaml
---
description: Generate customer support response
argument-hint: [inquiry] [context]
---
```

**Workflow:**
1. Analyze inquiry
2. Check order/account context
3. Generate helpful response
4. Include relevant links
5. Output response

**Agent:** `customer-service`

---

### /support:return
```yaml
---
description: Process return/refund request
argument-hint: [order-id] [reason]
---
```

**Workflow:**
1. Verify order details
2. Check return eligibility
3. Generate RMA
4. Create customer response
5. Output return package

**Agent:** `customer-service`

---

### /support:escalate
```yaml
---
description: Escalate complex customer issue
argument-hint: [issue] [priority]
---
```

**Workflow:**
1. Summarize issue
2. Document history
3. Assess priority
4. Route to appropriate team
5. Output escalation ticket

**Agent:** `customer-service`

---

### /support:review
```yaml
---
description: Generate response to customer review
argument-hint: [review] [sentiment]
---
```

**Workflow:**
1. Analyze review sentiment
2. Identify key points
3. Craft appropriate response
4. Maintain brand voice
5. Output review response

**Agent:** `customer-service`

---

## 3.5 Marketing Commands

### /marketing:email
```yaml
---
description: Create email campaign
argument-hint: [campaign-type] [audience]
---
```

**Workflow:**
1. Define campaign goal
2. Segment audience
3. Write email content
4. Add personalization
5. Output email campaign

**Agent:** `marketing-automator`

---

### /marketing:ad
```yaml
---
description: Create ad copy for platform
argument-hint: [platform] [product-or-promo]
---
```

**Workflow:**
1. Understand platform specs
2. Define value proposition
3. Write ad variations
4. Add CTAs
5. Output ad copy set

**Agent:** `marketing-automator`

---

### /marketing:promo
```yaml
---
description: Plan promotional campaign
argument-hint: [promo-type] [products]
---
```

**Workflow:**
1. Define promotion goals
2. Select products/categories
3. Set discount structure
4. Plan marketing support
5. Output promo plan

**Agent:** `marketing-automator`

---

### /marketing:segment
```yaml
---
description: Create customer segment
argument-hint: [criteria] [purpose]
---
```

**Workflow:**
1. Define segment criteria
2. Analyze customer data
3. Create segment rules
4. Estimate segment size
5. Output segment definition

**Agent:** `marketing-automator`

---

### /marketing:flow
```yaml
---
description: Create automated email flow
argument-hint: [flow-type] [triggers]
---
```

**Workflow:**
1. Define flow purpose
2. Map customer journey
3. Create email sequence
4. Set timing/triggers
5. Output flow blueprint

**Agent:** `marketing-automator`

---

## 3.6 Analytics Commands

### /analytics:sales
```yaml
---
description: Generate sales report
argument-hint: [period] [breakdown]
---
```

**Workflow:**
1. Pull sales data
2. Calculate metrics
3. Identify trends
4. Compare periods
5. Output sales report

**Agent:** `sales-analyst`

---

### /analytics:product
```yaml
---
description: Analyze product performance
argument-hint: [products] [period]
---
```

**Workflow:**
1. Pull product metrics
2. Rank by performance
3. Identify winners/losers
4. Suggest actions
5. Output product analysis

**Agent:** `sales-analyst`

---

### /analytics:customer
```yaml
---
description: Analyze customer behavior
argument-hint: [segment] [metrics]
---
```

**Workflow:**
1. Pull customer data
2. Calculate LTV, CAC
3. Analyze cohorts
4. Identify patterns
5. Output customer analysis

**Agent:** `sales-analyst`

---

### /analytics:forecast
```yaml
---
description: Forecast sales/revenue
argument-hint: [period] [factors]
---
```

**Workflow:**
1. Analyze historical data
2. Factor seasonality
3. Apply growth factors
4. Generate projections
5. Output forecast

**Agent:** `sales-analyst`

---

## 3.7 Order Commands

### /order:process
```yaml
---
description: Process pending orders
argument-hint: [orders] [priority]
---
```

**Workflow:**
1. Validate orders
2. Check inventory
3. Route to fulfillment
4. Update status
5. Output processing report

**Agent:** `order-processor`

---

### /order:track
```yaml
---
description: Get order tracking information
argument-hint: [order-id]
---
```

**Workflow:**
1. Pull order details
2. Get carrier tracking
3. Calculate delivery estimate
4. Format for customer
5. Output tracking info

**Agent:** `order-processor`

---

### /order:fulfill
```yaml
---
description: Generate fulfillment instructions
argument-hint: [orders] [warehouse]
---
```

**Workflow:**
1. Group orders by location
2. Generate pick lists
3. Select shipping method
4. Create shipping labels
5. Output fulfillment package

**Agent:** `order-processor`

---

### /order:exception
```yaml
---
description: Handle order exception
argument-hint: [order-id] [issue-type]
---
```

**Workflow:**
1. Identify issue
2. Determine resolution
3. Update customer
4. Process correction
5. Output exception report

**Agent:** `order-processor`

---

## 3.8 Command Quick Reference

| Command | Description | Agent |
|---------|-------------|-------|
| `/product:create` | Create listing | product-manager |
| `/product:optimize` | Optimize listing | product-manager |
| `/product:bulk` | Bulk updates | product-manager |
| `/product:seo` | SEO optimization | product-manager |
| `/product:marketplace` | Marketplace listing | product-manager |
| `/inventory:status` | Inventory report | inventory-optimizer |
| `/inventory:forecast` | Demand forecast | inventory-optimizer |
| `/inventory:reorder` | Reorder recommendations | inventory-optimizer |
| `/inventory:clearance` | Clearance planning | inventory-optimizer |
| `/support:respond` | Customer response | customer-service |
| `/support:return` | Return processing | customer-service |
| `/support:escalate` | Issue escalation | customer-service |
| `/support:review` | Review response | customer-service |
| `/marketing:email` | Email campaign | marketing-automator |
| `/marketing:ad` | Ad copy | marketing-automator |
| `/marketing:promo` | Promotion planning | marketing-automator |
| `/marketing:segment` | Customer segment | marketing-automator |
| `/marketing:flow` | Email flow | marketing-automator |
| `/analytics:sales` | Sales report | sales-analyst |
| `/analytics:product` | Product analysis | sales-analyst |
| `/analytics:customer` | Customer analysis | sales-analyst |
| `/analytics:forecast` | Sales forecast | sales-analyst |
| `/order:process` | Order processing | order-processor |
| `/order:track` | Order tracking | order-processor |
| `/order:fulfill` | Fulfillment | order-processor |
| `/order:exception` | Exception handling | order-processor |
