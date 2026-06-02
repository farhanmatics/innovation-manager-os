# Financial Modeling Framework

Enterprise-grade product decisions require financial rigor. This framework defines the mandatory financial analysis for each classification level.

## Financial Analysis Requirements by Classification

| Classification | Required Financial Analysis |
|---|---|
| **Custom Project** | Project budget, margin, revenue |
| **Reusable Framework** | Above + estimated cost savings from reuse |
| **Enterprise Product** | Full financial model: ACV, CAC, LTV, margin, payback, 3-year ARR projection, funding requirement, breakeven |
| **Industry Platform** | Above + audited unit economics, multi-vertical P&L, platform monetization model |
| **Strategic Business Unit** | Above + board-grade 5-year model, valuation, exit analysis, standalone P&L |

## Mandatory Financial Metrics

For any recommendation of Enterprise Product or above, the following must be calculated with grade-B or higher evidence:

### Core Unit Economics

| Metric | Formula | Healthy Range | Red Flag |
|---|---|---|---|
| **Average Contract Value (ACV)** | Total contract value / years | Industry-dependent | < $10K (too small for enterprise sales) |
| **Annual Recurring Revenue (ARR)** | Sum of annualized contract values | Growing > 50% YoY (early) | Declining or flat |
| **Customer Acquisition Cost (CAC)** | Total sales + marketing spend / new customers | — | > 50% of ACV (enterprise) |
| **Lifetime Value (LTV)** | ACV × gross margin × avg customer lifespan (years) | — | < 3× CAC |
| **LTV:CAC Ratio** | LTV / CAC | > 3:1 for enterprise | < 2:1 |
| **CAC Payback Period** | CAC / (ACV × gross margin / 12) in months | < 18 months | > 24 months |
| **Gross Margin** | (Revenue - COGS) / Revenue | > 70% for SaaS | < 50% |
| **Net Revenue Retention (NRR)** | (Starting ARR + expansion - contraction - churn) / Starting ARR | > 100% | < 90% |
| **Annual Churn Rate** | Lost ARR / Starting ARR | < 10% enterprise | > 20% |

### ARR Projection Model

Must include three scenarios:

| Year | Conservative | Base Case | Optimistic |
|---|---|---|---|
| Year 1 | $ | $ | $ |
| Year 2 | $ | $ | $ |
| Year 3 | $ | $ | $ |
| Year 5 | $ | $ | $ |

**Key Drivers** (document assumptions for each scenario):
- New customers per year
- ACV growth/decline
- Churn rate
- Expansion revenue

### Cost Structure

| Category | Year 1 | Year 2 | Year 3 |
|---|---|---|---|
| **Engineering** | $ | $ | $ |
| — Headcount (n × avg salary) | | | |
| — Infrastructure / cloud | | | |
| — Tools / licenses | | | |
| **Product Management / Design** | $ | $ | $ |
| **Sales** | $ | $ | $ |
| — Headcount (n × OTE) | | | |
| — Marketing programs | | | |
| — Sales tools / travel | | | |
| **Customer Success / Support** | $ | $ | $ |
| **G&A Allocation** | $ | $ | $ |
| **TOTAL COSTS** | **$** | **$** | **$** |

### Funding Requirement

| Stage | Amount | Use of Funds | Timing | Milestone |
|---|---|---|---|---|
| VALIDATE | $ | Customer interviews, competitive research, LOI development | Months 0–2 | Go/No-Go gate |
| INCUBATE (MVP) | $ | Engineering + initial GTM | Months 3–8 | First paying customers |
| INCUBATE (V1) | $ | Engineering + initial sales hire | Months 9–14 | 10 customers, 2nd vertical |
| SCALE (V2) | $ | Full team + marketing | Months 15–24 | $1M ARR |
| **TOTAL** | **$** | | | |

### Cash Flow & Breakeven

| Metric | Value |
|---|---|
| Total investment to breakeven | $ |
| Months to cash flow breakeven | |
| Cumulative cash needed (peak negative) | $ |
| Capital efficiency (ARR / total invested) | |

**Rule of thumb**: Enterprise SaaS should target capital efficiency > 1.0 (ARR ≥ total invested) by Year 3.

## Financial Gates by Stage

### VALIDATE Stage Financial Requirements

- [ ] TAM > $100M (or documented strategic rationale for smaller)
- [ ] Estimated ACV range with basis (competitor pricing, customer willingness interviews)
- [ ] Rough COGS estimate (infrastructure, support, services)
- [ ] Plausible path to > 70% gross margin

**Gate**: If unit economics are clearly broken at this stage (e.g., ACV < $5K with enterprise sales motion), KILL.

### INCUBATE Stage Financial Requirements

- [ ] Real ACV data from first 3+ customers (not list price, actual paid)
- [ ] Real COGS data from live deployment (infrastructure, support tickets, services hours)
- [ ] Initial CAC data (sales cost for first customers)
- [ ] Validated or invalidated unit economics assumptions

**Gate**: If LTV:CAC < 2:1 with real data and no path to 3:1, KILL.

### SCALE Stage Financial Requirements

- [ ] Statistically significant unit economics (10+ customers)
- [ ] Sales efficiency improving (CAC declining)
- [ ] Gross margin stable or improving
- [ ] Expansion revenue validated (NRR measurable)
- [ ] Path to profitability modeled

**Gate**: If NRR < 90% or churn > 20%, PAUSE — fix product before scaling.

## Financial Red Flags

These patterns should block or pause investment:

| Red Flag | Severity | Action |
|---|---|---|
| LTV:CAC < 2:1 with no improvement trend | 🔴 Critical | KILL unless strategic rationale |
| Gross margin < 50% in SaaS | 🔴 Critical | Redesign architecture or KILL |
| CAC payback > 24 months | 🔴 Critical | PAUSE; improve sales efficiency |
| ACV < $10K with enterprise sales motion | 🟡 Warning | Either go PLG or KILL |
| Services > 30% of revenue | 🟡 Warning | Standardize product or accept services business |
| "We'll figure out pricing later" | 🟡 Warning | Validate willingness to pay NOW |
| All financial numbers are grade D or E | 🔴 Critical | BLOCK investment until validated |
| Revenue projections assume hockey-stick without basis | 🟡 Warning | Require bottoms-up model from known ACV × realistic customer count |

## Financial Assumptions Registry

Every financial model must document its assumptions:

| Assumption | Value | Basis | Grade | Validated? |
|---|---|---|---|---|
| ACV | $ | | | |
| New customers/month | | | | |
| Churn rate | | | | |
| Sales rep quota | | | | |
| Sales ramp time | | | | |
| Engineering cost/person | | | | |
| Cloud infra cost/customer | | | | |
| Support tickets/customer/month | | | | |
| Gross margin | | | | |
| (add rows as needed) | | | | |

**Rule**: Any assumption with grade D or E must be flagged as "must validate before next gate."
