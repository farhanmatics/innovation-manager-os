# Product Opportunity Scorecard

A structured scoring framework to evaluate whether a custom project can become an enterprise product.

## Scoring Guide

Score each dimension from 1 to 5 (1 = weak, 5 = exceptional).

### Market Assessment (1–15 points)

#### Problem Frequency (1–5)
How often does the target customer face this problem?

| Score | Criteria |
|---|---|
| 1 | Rarely — once a year or less |
| 2 | Occasionally — quarterly |
| 3 | Regularly — monthly |
| 4 | Frequently — weekly |
| 5 | Constantly — daily or continuous |

#### Problem Severity (1–5)
How painful or costly is this problem when it occurs?

| Score | Criteria |
|---|---|
| 1 | Minor inconvenience — no measurable cost |
| 2 | Noticeable friction — minor cost (< $10K/year) |
| 3 | Significant pain — measurable cost ($10K–$100K/year) |
| 4 | Major disruption — substantial cost ($100K–$1M/year) |
| 5 | Existential threat — catastrophic cost (> $1M/year) or compliance risk |

#### Industry Applicability (1–5)
How many industries face this same problem?

| Score | Criteria |
|---|---|
| 1 | Single niche industry |
| 2 | 2–3 adjacent industries |
| 3 | 4–6 industries |
| 4 | 7–10 industries |
| 5 | Cross-industry universal problem |

### Product Assessment (1–15 points)

#### Standardization Potential (1–5)
What percentage of the solution can be standardized?

| Score | Criteria |
|---|---|
| 1 | < 30% — mostly custom |
| 2 | 30–49% — some reuse |
| 3 | 50–69% — significant standardization |
| 4 | 70–85% — highly standardized |
| 5 | > 85% — nearly fully standardized |

#### Reuse Potential (1–5)
How many reusable components exist in the solution?

| Score | Criteria |
|---|---|
| 1 | 0–1 components — pure custom |
| 2 | 2–3 components |
| 3 | 4–6 components |
| 4 | 7–9 components |
| 5 | 10+ components or entire framework is reusable |

#### Competitive Differentiation (1–5)
How difficult is this to replicate?

| Score | Criteria |
|---|---|
| 1 | Trivial — any team can build it in weeks |
| 2 | Low barrier — several competitors exist |
| 3 | Moderate barrier — domain knowledge + 6 months |
| 4 | High barrier — proprietary data, patents, or network effects |
| 5 | Very high barrier — years of data, regulatory moat, or unique IP |

### Business Assessment (1–15 points)

#### Sales Potential (1–5)
How many customers would buy this as a product?

| Score | Criteria |
|---|---|
| 1 | 1–3 customers |
| 2 | 4–10 customers |
| 3 | 11–50 customers |
| 4 | 51–500 customers |
| 5 | 500+ customers or mass market |

#### Implementation Scalability (1–5)
Can this be deployed without heavy customization per customer?

| Score | Criteria |
|---|---|
| 1 | Full custom implementation required for each customer |
| 2 | 30–50% reuse per implementation |
| 3 | 50–70% reuse with configuration |
| 4 | 70–90% standard deployment with light configuration |
| 5 | Fully self-service or near-zero-touch deployment |

#### Support Scalability (1–5)
Can we support this at scale with reasonable margins?

| Score | Criteria |
|---|---|
| 1 | High-touch dedicated support team per customer |
| 2 | Shared support team, high ticket volume |
| 3 | Standard support tier, manageable volume |
| 4 | Largely self-serve, low-touch support |
| 5 | Fully automated support, negligible marginal cost |

## Total Score Calculation

```
Market Score (__/15) + Product Score (__/15) + Business Score (__/15) = Total (__/45)
```

## Interpretation Matrix

| Score Range | Scorecard Label | Maps to Final Verdict | Action |
|---|---|---|---|
| 0–15 | **Custom Project** | Custom Project | Build for delivery only. Charge for services. No product investment. |
| 16–25 | **Reusable Framework** | Reusable Framework | Extract common patterns. Build internal libraries. Reduce future project costs. |
| 26–35 | **Enterprise Product Candidate** | Reusable Framework or Enterprise Product (see SKILL.md mapping table) | Validate with 3–5 design partners. Build MVP. Assign product manager. Seek first external sale. |
| 36–45 | **Strategic Product Opportunity** | Enterprise Product, Industry Platform, or Strategic Business Unit (see SKILL.md mapping table) | Form dedicated team. Create business plan. Allocate serious budget. Consider separate P&L or business unit. |

**Note**: The scorecard labels are screening terms. Final verdict classification follows the mapping table in `skills/enterprise-product-innovation/SKILL.md`. Evidence quality and confidence-adjusted scores determine the defensible classification — the raw scorecard label is an aspiration, not a claim.

## Scoring Rules

1. **Be conservative.** Round down when uncertain.
2. **Require evidence.** Every score needs a one-sentence justification.
3. **Re-score quarterly.** Market conditions change.
4. **Compare against past scores.** Track trajectory over time.
5. **Use with venture analyst review.** Scorecard + investment analysis = board-ready recommendation.

## Example: Hypothetical Surveillance Platform

| Dimension | Score | Justification |
|---|---|---|
| Problem Frequency | 5 | Security teams monitor continuously, 24/7 |
| Problem Severity | 5 | Security breaches cost millions + regulatory fines |
| Industry Applicability | 5 | Every industry needs surveillance |
| Standardization Potential | 4 | 80% can be standard; 20% industry-specific rules |
| Reuse Potential | 5 | 10+ reusable components (alert engine, dashboard, RBAC, audit trail, AI analytics) |
| Competitive Differentiation | 3 | Several competitors, but AI analytics + industry specialization differentiates |
| Sales Potential | 5 | 500+ potential customers across Banking, Telecom, Government |
| Implementation Scalability | 3 | Requires configuration per vertical |
| Support Scalability | 3 | Monitoring platforms need ongoing tuning |
| **TOTAL** | **38/45** | **Strategic Product Opportunity** |
