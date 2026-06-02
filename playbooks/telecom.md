# Telecom Industry Playbook

Domain-specific guidance for evaluating product opportunities in Telecom.

## Industry DNA

Telecom is a high-volume, high-regulation, high-infrastructure industry. Products must handle massive scale and strict SLAs.

## Key Problems That Signal Product Opportunity

| Problem | Product Signal | Typical Buyer |
|---|---|---|
| Subscriber churn exceeds 2%/month | Analytics/Retention Platform | CMO, VP Customer Experience |
| SLA penalty payments increasing | Monitoring & Alert Platform | COO, VP Operations |
| Regulatory compliance audits failing | Compliance Automation | CCO, Legal |
| Network operations cost growing faster than revenue | AIOps / Automation | CTO, VP Network Ops |
| Customer onboarding takes > 7 days | Workflow Automation | COO, VP Digital |
| Fraud losses exceed 1% of revenue | Fraud Detection Platform | CISO, VP Risk |
| Legacy BSS/OSS can't support 5G/IoT | Modernization Platform | CIO, CTO |
| Partner settlements take > 30 days | Billing/Reconciliation Platform | CFO, VP Finance |

## Telecom Buyer Psychology

- **Risk-averse**: Telcos fear outages more than they desire innovation
- **Regulatory-driven**: Compliance is often the strongest buying trigger
- **Scale-obsessed**: "Will this work with 10M subscribers?" is always question #1
- **Vendor-fatigued**: They have 500+ vendors; you must stand out
- **Slow procurement**: 6-18 month sales cycles are normal
- **POC culture**: Expect to prove value before purchase

## Reusable Component Patterns in Telecom

Telecom projects naturally produce these reusable components:

- **Mediation Engine**: Transform data between formats/protocols (universal across industries)
- **Rating & Charging Engine**: Usage-based pricing, rating rules (applicable to utilities, logistics)
- **Dashboard/Portal**: Customer self-service, admin analytics (every industry)
- **Notification Engine**: SMS, email, push, in-app (every industry)
- **Workflow Engine**: Order management, provisioning, incident management (every industry)
- **SLA Monitoring**: Real-time KPI tracking, penalty calculation (enterprise IT, healthcare)
- **Fraud Detection**: Pattern recognition, anomaly detection (banking, insurance)
- **Reconciliation Engine**: Data matching, settlement (banking, retail)

## Telecom Product Archetypes

### Archetype 1: OSS/BSS Modernization Platform
- **Problem**: Legacy systems from 1990s-2000s can't support digital transformation
- **Product**: Cloud-native BSS/OSS stack with API-first architecture
- **Adjacent Markets**: ISPs, MVNOs, utilities, any subscription business
- **Product Score**: Usually 30-38 (high standardization, massive TAM, but complex sales)

### Archetype 2: Telecom AI/ML Platform
- **Problem**: Manual operations, reactive monitoring, undetected fraud
- **Product**: AI layer for network ops, customer analytics, fraud, chatbots
- **Adjacent Markets**: Any enterprise with large-scale operations
- **Product Score**: Usually 32-40 (high IP value, cross-industry, data moat)

### Archetype 3: Customer Experience Platform
- **Problem**: Siloed customer data, inconsistent experience, high churn
- **Product**: Unified CX platform with journey analytics, personalization
- **Adjacent Markets**: Banking, retail, hospitality
- **Product Score**: Usually 25-35 (competitive market but large TAM)

### Archetype 4: IoT/M2M Connectivity Platform
- **Problem**: Managing millions of connected devices
- **Product**: IoT device management, connectivity, analytics
- **Adjacent Markets**: Manufacturing, logistics, utilities, healthcare
- **Product Score**: Usually 30-38 (growing market, cross-industry, IP-intensive)

## Commercial Models That Work in Telecom

1. **Subscription + Usage**: Base platform fee + per-subscriber/transaction pricing
2. **Managed Service**: Telecoms prefer outsourced operations with SLA guarantees
3. **Revenue Share**: Take % of cost savings or revenue uplift (harder to sell but higher upside)
4. **Enterprise License**: For on-premise deployments (still common in telecom)

**Avoid**: Pure SaaS with no SLA — telecoms won't buy it.

## Telecom Red Flags

- Customer says "we're the only one with this problem" (unlikely to be productizable)
- Requires deep integration with a specific legacy vendor (lock-in risk)
- All value comes from custom AI models on customer-specific data
- 18+ month implementation timeline (too slow for product validation)
