# Evidence Quality Framework

Enterprise-grade innovation decisions require knowing what you know, what you assume, and what you need to validate. This framework forces rigor.

## Evidence Grading System

Every factual claim in a product assessment must carry an evidence grade:

| Grade | Label | Definition | Example |
|---|---|---|---|
| **A** | Verified Fact | Confirmed by primary source, data, or direct customer statement | "3 design partners signed LOIs at $50K ACV" |
| **B** | Strong Signal | Corroborated by multiple secondary sources or strong proxies | "Gartner reports market at $4.2B growing 18% CAGR" |
| **C** | Reasonable Estimate | Extrapolated from partial data or comparable markets | "Estimated 2,000 mid-size banks in North America" |
| **D** | Educated Assumption | Based on domain expertise without direct evidence | "Assumed CAC will be $40K based on similar enterprise products" |
| **E** | Unvalidated Guess | No evidence; placeholder requiring validation | "Guess: 5% of telecom operators face this problem" |
| **V** | Requires Validation | Needs to be validated before decision — tag with method | "V: Need 10 customer interviews to confirm pain severity" |

## Confidence Levels

Each major assertion carries a confidence level:

| Level | % | Meaning | Action |
|---|---|---|---|
| **High** | > 80% | Confident enough to commit resources | Proceed with standard risk management |
| **Medium** | 50–80% | Directionally correct; needs confirmation | Invest to validate before major commitment |
| **Low** | < 50% | Speculative; major assumption | DO NOT commit resources; validate first |
| **Unknown** | — | No basis for assessment | Explicitly flag; design validation experiment |

## Evidence Ledger

Every product assessment **must** include an evidence ledger. This is a structured log of claims, their evidence grade, confidence, and validation plan.

### Evidence Ledger Template

| # | Claim | Category | Grade | Confidence | Source / Basis | Validation Method | Validated? |
|---|---|---|---|---|---|---|---|
| 1 | Market size is $X | Market | C | Medium | Gartner report, extrapolated | Cross-reference 2 analyst reports | No |
| 2 | Customers lose $Y/yr to this problem | Problem | B | High | 15 customer interviews | Verify with 5 more | Yes |
| 3 | Competitor A charges $Z | Competitive | A | High | Competitor pricing page + 3 customer references | — | Yes |
| 4 | 70% of features can be standardized | Product | D | Low | Architect assessment | Build config layer prototype | No |
| 5 | Telecom is the best second vertical | Strategy | E | Unknown | Guess based on industry similarity | Conduct 10 telecom interviews | No |

### Rules for the Evidence Ledger

1. **No grade-A claims without source attribution.** "Trust me" is not a source.
2. **Financial claims must be grade B or higher** for any recommendation above Reusable Framework.
3. **Any grade-D or E claim blocks** Enterprise Product or higher classification until validated.
4. **Any grade-V tag** must have a named validation method and a deadline.
5. **Confidence-weighted scoring**: Final scorecard scores must be annotated with confidence level. A score of 5 with low confidence is worth less than a 3 with high confidence.

## Confidence-Weighted Scorecard

For each scorecard dimension, apply the fixed multiplier formula:

```
Adjusted Score = Raw Score × Confidence Multiplier
```

| Confidence Level | Multiplier |
|---|---|
| High (> 80%) | 1.0 |
| Medium (50–80%) | 0.7 |
| Low (< 50%) | 0.4 |
| Unknown | 0.0 |

### Example

| Dimension | Raw Score | Confidence | Multiplier | Adjusted Score | Rationale |
|---|---|---|---|---|---|
| Problem Frequency | 5 | High | 1.0 | 5.0 | Seen across 15/15 interviewed customers |
| Problem Severity | 4 | Medium | 0.7 | 2.8 | Estimated from interviews; need CFO validation |
| Industry Applicability | 4 | Low | 0.4 | 1.6 | Assumed; only validated in 1 industry so far |
| Standardization Potential | 3 | Medium | 0.7 | 2.1 | Architect review; not yet tested with config layer |
| Reuse Potential | 4 | High | 1.0 | 4.0 | 8 components clearly reusable |
| Competitive Differentiation | 3 | Low | 0.4 | 1.2 | Assumed; no competitive deep-dive yet |
| Sales Potential | 4 | Medium | 0.7 | 2.8 | LOI interest from 3; need broader validation |
| Implementation Scalability | 3 | Low | 0.4 | 1.2 | First deployment not yet complete |
| Support Scalability | 3 | Unknown | 0.0 | 0.0 | No data; purely speculative |
| **TOTAL** | **33/45** | — | — | **20.7** | Raw score masks major evidence gaps |

### Confidence-Adjusted Interpretation

| Raw Score | Confidence-Adjusted | Meaning |
|---|---|---|
| 33/45 | 20.7 | High raw score but weak evidence. **Do not classify as Enterprise Product until evidence gaps closed.** Maximum classification: Reusable Framework with validation plan. |

**Note**: The fixed multipliers produce a floor of 0.0 (Unknown dimensions add nothing) and a ceiling of 45.0 (all High). This is intentionally conservative — unknown evidence should not contribute to the score at all.

## Evidence Requirements by Classification

Different classifications demand different minimum evidence standards:

| Classification | Minimum Requirements |
|---|---|
| **Custom Project** | No evidence requirements beyond project scope |
| **Reusable Framework** | At least 5 grade-B claims; component reuse validated by engineering |
| **Enterprise Product** | ALL scorecard dimensions at medium confidence or higher; at least 3 grade-A claims; customer validation evidence (interviews, LOI, or pilot data); financial model with grade-B inputs |
| **Industry Platform** | ALL scorecard dimensions at high confidence; 10+ grade-A claims; multi-industry validation data; reference customers in 2+ industries; audited financial model |
| **Strategic Business Unit** | All Industry Platform requirements + board-grade financial model; 3rd-party market validation; competitive due diligence; executive sponsor confirmed |

## Violations

These patterns should trigger automatic downgrade in classification:

1. **Evidence-free assertions**: "This is obviously a $10B market" without source → downgrade one tier
2. **Confidence inflation**: Claiming "high confidence" on assumptions → require re-grading
3. **Missing validation plan**: Grade-V tags without named method and date → reject classification
4. **Financial model on guesses**: LTV, CAC, or ACV built on grade-D or E evidence → block Enterprise Product+
5. **Competitive analysis without source**: "No competitors" or generic competitor descriptions without source → require competitive deep-dive
