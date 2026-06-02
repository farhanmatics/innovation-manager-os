# Banking & Financial Services Playbook

Domain-specific guidance for evaluating product opportunities in Banking, Insurance, and Financial Services.

## Industry DNA

Financial services is the most regulated, security-conscious, and data-intensive industry. Products must be bulletproof on compliance, security, and reliability. The reward: some of the highest ACVs in enterprise software.

## Key Problems That Signal Product Opportunity

| Problem | Product Signal | Typical Buyer |
|---|---|---|
| KYC/AML compliance costs rising 20%+ annually | Compliance Automation / RegTech | CCO, CRO |
| Fraud losses increasing year-over-year | Fraud Detection / AI Platform | CISO, VP Fraud |
| Customer onboarding takes 2+ weeks | Digital Onboarding / Workflow | COO, VP Digital |
| Legacy core banking limits product innovation | Core Modernization / Middleware | CIO, CTO |
| Regulatory exam findings repeat | Compliance / Audit Management | CCO, Internal Audit |
| 60%+ of transactions still through branches | Digital Banking Platform | CMO, Head of Digital |
| Open banking compliance deadlines approaching | API Banking Platform | CTO, CDO |
| Manual reconciliation across systems | Reconciliation / Matching Engine | CFO, Controller |

## Banking Buyer Psychology

- **Security-paranoid**: Breach = existential crisis. Security is the #1 evaluation criterion.
- **Regulation-driven**: New regulation = new product opportunity. Timing matters.
- **Vendor risk management**: 6-12 month vendor assessment process. Plan for it.
- **Conservative**: "Who else in banking uses this?" — peer references are mandatory
- **High ACV, high expectation**: Will pay more but demands enterprise-grade everything
- **Build vs. buy bias**: Large banks prefer to build; mid-tier and community banks prefer to buy

## Reusable Component Patterns in Banking

- **Transaction Monitoring**: Real-time pattern detection (also in telecom, retail, gaming)
- **Risk Scoring Engine**: Calculate risk scores based on rules and ML (insurance, telecom, healthcare)
- **Compliance Rule Engine**: Codify regulations as executable rules (every regulated industry)
- **Workflow Engine with 4-Eyes Principle**: Maker-checker, multi-level approvals (government, legal, enterprise)
- **Reconciliation Engine**: Match transactions across systems (retail, logistics, telecom)
- **Customer 360**: Unified customer view across products (telecom, retail, hospitality)
- **Document Verification**: OCR, fraud detection, liveness check (government, telecom, sharing economy)
- **Case Management**: Investigation workflows, evidence collection (government, legal, insurance)

## Banking Product Archetypes

### Archetype 1: RegTech / Compliance Automation
- **Problem**: Keeping up with 200+ regulatory changes/year per jurisdiction
- **Product**: Regulatory intelligence + policy management + control automation + evidence collection
- **Adjacent Markets**: Insurance, healthcare, energy, any regulated industry
- **Product Score**: Usually 34-42 (regulation creates urgency + moat, massive cross-industry applicability)

### Archetype 2: Fraud & Financial Crime Platform
- **Problem**: Sophisticated fraud schemes, rising losses, regulatory pressure
- **Product**: Real-time fraud detection using ML, network analysis, behavioral biometrics
- **Adjacent Markets**: Insurance (claims fraud), government (benefits fraud), telecom (subscription fraud), e-commerce
- **Product Score**: Usually 35-43 (high IP, data network effects, cross-industry)

### Archetype 3: Digital Onboarding & KYC
- **Problem**: Slow, paper-based customer onboarding
- **Product**: Digital identity verification, document scanning, biometric authentication, automated KYC checks
- **Adjacent Markets**: Telecom, sharing economy, crypto, government services
- **Product Score**: Usually 30-38 (high demand, configurable rules, cross-industry)

### Archetype 4: Open Banking / API Platform
- **Problem**: Regulatory mandate to open APIs, legacy systems can't support
- **Product**: API gateway, developer portal, consent management, monetization
- **Adjacent Markets**: Any industry with partner ecosystems (telecom, healthcare, utilities)
- **Product Score**: Usually 28-35 (regulatory tailwind, platform potential)

## Commercial Models That Work in Banking

1. **Enterprise License + Annual Maintenance**: Preferred for on-premise/core systems. Maintenance is 18-22%.
2. **Subscription (SaaS)**: Growing acceptance for non-core systems (compliance, analytics, onboarding)
3. **Transaction-Based**: Per transaction, per KYC check, per alert investigated
4. **Managed Service**: For fraud operations, compliance monitoring — banks outsource operations

**Context**: Average ACV ranges from $50K (community bank) to $5M+ (tier-1 global bank).

## Banking-Specific Requirements

- SOC 2 Type II — minimum
- PCI DSS — if handling card data
- FFIEC compliance — U.S. banking
- GDPR / PSD2 — European banking
- Data residency — often required
- Penetration testing — annual, by approved firms
- Business continuity / DR — RTO < 4 hours, RPO < 15 minutes
- Vendor risk assessment — 6-12 month process

## Banking Red Flags

- Core banking replacement (too complex, too risky, too long — 3-5 year projects)
- Customer says "compliance isn't a concern" (not a real bank)
- 100% on-premise requirement with no migration path (shrinking market)
- Single jurisdiction regulatory solution with no path to multi-jurisdiction
- Customer is the only bank that does things this way
