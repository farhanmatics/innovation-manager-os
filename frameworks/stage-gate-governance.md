# Stage-Gate Governance Framework

Enterprise innovation is not "go build and see what happens." It is a disciplined process of staged investment with explicit gates that can kill, redirect, or accelerate opportunities.

## The 5-Stage Model

```
EXPLORE ──→ VALIDATE ──→ INCUBATE ──→ SCALE ──→ OPTIMIZE
   │            │            │            │           │
   └────────────┴────────────┴────────────┴───────────┘
                         KILL (any stage)
```

### Stage 1: EXPLORE

**Purpose**: Identify and triage opportunities. Is this worth a deeper look?

**Entry Criteria**: Anyone can submit an idea, project observation, or RFP pattern.

**Investment**: $0–$5K of time. 1–2 days of analysis.

**Activities**:
- Complete 8-phase innovation assessment
- Initial scorecard (allows low-confidence scores)
- Identify top 3 unknown risks
- Preliminary classification

**Exit Gate → VALIDATE**:
- [ ] Scorecard ≥ 20/45 (or confidence-adjusted ≥ 12)
- [ ] At least one evidence-backed reason this COULD be a product
- [ ] No fatal flaws identified (zero TAM, illegal, impossible tech)
- [ ] Sponsor identified for validation phase

**Exit Gate → KILL**:
- Scorecard < 20/45 with no path to improve
- Fatal flaw identified
- Clear strategic misalignment

**Output**: 1-page opportunity brief + evidence ledger

---

### Stage 2: VALIDATE

**Purpose**: Prove or disprove the critical assumptions. Is there real demand?

**Entry Criteria**: EXPLORE gate passed and sponsor committed.

**Investment**: $5K–$50K. 4–8 weeks.

**Activities**:
- 20+ customer problem interviews (NOT solution pitches)
- Competitive deep-dive with source attribution
- Technical feasibility spike (can we build the core?)
- Market sizing with analyst sources
- Initial financial model (ranges, not precise numbers)
- 3–5 letters of intent or design partner commitments

**Exit Gate → INCUBATE**:
- [ ] 60%+ of interviewed customers describe urgent pain with emotional language
- [ ] 3+ signed LOIs or committed design partners
- [ ] Market TAM > $100M (or strategic rationale for smaller)
- [ ] All evidence grades at B or higher on key claims
- [ ] Financial model shows plausible path to 3:1 LTV:CAC
- [ ] No competitor with unassailable moat identified
- [ ] Internal capability exists or plan to acquire it

**Exit Gate → KILL**:
- Customers are polite but won't commit
- No clear buying trigger found
- TAM too small
- Competitor moat is impenetrable
- Unit economics don't work

**Output**: Validation report + confidence-weighted scorecard + evidence ledger with 10+ grade-B or higher entries

---

### Stage 3: INCUBATE

**Purpose**: Build MVP, get first paying customers, prove product-market fit.

**Entry Criteria**: VALIDATE gate passed.

**Investment**: $50K–$500K. 3–6 months.

**Activities**:
- Build product core (NOT full feature set)
- Deploy to 3–5 design partners
- Iterate based on usage data and feedback
- Begin configuration layer design
- Hire initial product-dedicated team
- Set up financial tracking separate from services P&L

**Exit Gate → SCALE**:
- [ ] 3+ paying customers (not free, not discounted below 50%)
- [ ] Net revenue retention > 100%
- [ ] < 20% custom code per new deployment
- [ ] Customer-reported value validated (case studies, references)
- [ ] At least 2 customers would be "very disappointed" if product disappeared
- [ ] Repeatable sales motion identified (not founder-led)
- [ ] Unit economics validated with real data: LTV:CAC > 3:1, gross margin > 70%

**Exit Gate → KILL**:
- Customers won't pay full price
- Customization requests dominate (solution is not standardized enough)
- Churn exceeds 20% annually
- Acquisition cost unsustainable
- Better-funded competitor entering with superior offering

**Output**: Product-market fit evidence package + audited unit economics + 2+ referenceable customers

---

### Stage 4: SCALE

**Purpose**: Grow customer base, enter new verticals, build platform capabilities.

**Entry Criteria**: INCUBATE gate passed.

**Investment**: $500K–$5M/year. 12–36 months.

**Activities**:
- Build dedicated sales and marketing team
- Enter 2nd and 3rd industry verticals
- Build configuration layer for self-service / low-touch deployment
- Develop partner/reseller channel
- Build API platform and extension marketplace
- Pursue industry analyst recognition

**Exit Gate → OPTIMIZE**:
- [ ] 20+ paying customers across 2+ verticals
- [ ] ARR > $1M and growing > 50% YoY
- [ ] Gross margin > 70%
- [ ] Recognized in at least one analyst report
- [ ] Partner/channel generating > 20% of pipeline
- [ ] Platform stickiness: < 5% annual churn

**Exit Gate → KILL**:
- Growth stalls below 30% YoY for 2 consecutive quarters
- Competitive dynamics shift unfavorably
- Gross margin declining (customization creep)
- Key team members leaving
- Better internal opportunity demanding resources

**Output**: Scalable GTM playbook + multi-vertical case studies + analyst recognition

---

### Stage 5: OPTIMIZE

**Purpose**: Maximize profitability, market leadership, and platform ecosystem.

**Entry Criteria**: SCALE gate passed.

**Investment**: Variable. Profit-center operation.

**Activities**:
- Expand to all viable verticals
- Build ecosystem: developer platform, marketplace, SI partners
- Pursue market leadership position
- Consider spin-out as separate business unit
- Explore strategic acquisitions to fill gaps
- Optimize for profitability or growth based on strategy

**Exit Gate → STRATEGIC BUSINESS UNIT**:
- Market leader or strong #2 position
- Sustainable competitive moat
- $10M+ ARR with path to $50M+
- Independent leadership team

---

## Gate Decision Rules

### Who Decides?

| Gate | Authority | Forum |
|---|---|---|
| EXPLORE → VALIDATE | Product Innovation Director | Weekly pipeline review |
| VALIDATE → INCUBATE | VP Product + VP Engineering + CFO | Monthly innovation board |
| INCUBATE → SCALE | CEO / GM + CFO + Board observer | Quarterly portfolio review |
| SCALE → OPTIMIZE | CEO + Board | Annual strategy review |
| KILL (any stage) | Stage gate authority | Same forum as advancement |

### Decision Outcomes

At each gate, exactly one decision:

| Decision | Meaning |
|---|---|
| **ADVANCE** | Proceed to next stage with allocated budget |
| **ADVANCE WITH CONDITIONS** | Proceed but specific risks must be resolved by milestone |
| **RECYCLE** | Return to current or prior stage; opportunity is real but not ready |
| **PAUSE** | Stop spending; reassess at specified date or trigger event |
| **KILL** | Terminate investment; archive learnings; reassign resources |

### Kill Criteria That Trigger Review at Any Stage

1. **Market disappeared**: Regulatory change, technology shift, or competitor move eliminated demand
2. **Unit economics broken**: Real data shows LTV:CAC < 1.5:1 and no path to improvement
3. **Execution failed**: 2 consecutive missed milestones with no credible recovery plan
4. **Key person loss**: Irreplaceable founder/leader departed
5. **Better opportunity**: Higher-ROI opportunity needs the same resources
6. **Strategic pivot**: Company strategy changed; this no longer fits
7. **Fraud or ethics violation**: Opportunity built on unsustainable or unethical premise

## Stage-Gate Tracking

Every product opportunity should carry a stage tracker:

| Field | Value |
|---|---|
| **Opportunity Name** | |
| **Current Stage** | EXPLORE / VALIDATE / INCUBATE / SCALE / OPTIMIZE |
| **Date Entered Stage** | |
| **Gate Review Date** | |
| **Investment to Date** | $ |
| **Budget Remaining** | $ |
| **Stage Exit Criteria** | \<link to checklist\> |
| **Top 3 Risks** | |
| **Next Gate Decision** | [ ] ADVANCE / [ ] CONDITIONAL / [ ] RECYCLE / [ ] PAUSE / [ ] KILL |
