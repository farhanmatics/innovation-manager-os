# Government Industry Playbook

Domain-specific guidance for evaluating product opportunities in Government and Public Sector.

## Industry DNA

Government is the world's largest buyer of software. Procurement is complex, but contracts are large and sticky. Products must address compliance, security, and procurement requirements.

## Key Problems That Signal Product Opportunity

| Problem | Product Signal | Typical Buyer |
|---|---|---|
| Manual paper-based processes | Digital Workflow / e-Government Platform | CIO, Department Head |
| Citizens wait weeks for services | Case Management / Service Delivery Platform | Agency Director |
| Multiple agencies use incompatible systems | Integration / Interoperability Platform | CIO, CTO |
| Compliance audit findings repeat annually | Compliance Automation / Audit Management | Inspector General, CCO |
| Procurement takes 6+ months | Procurement Automation | CPO, CFO |
| Legacy systems past end-of-life with no migration path | Modernization Platform | CIO |
| Data sharing between agencies is impossible | Data Exchange / API Gateway | CDO, CIO |
| Citizen satisfaction scores declining | CX Platform for Government | Agency Director |

## Government Buyer Psychology

- **Procurement-driven**: Must follow RFP processes; relationship matters before RFP
- **Compliance-first**: FedRAMP, SOC 2, StateRAMP, GDPR, local data residency
- **Security-obsessed**: On-premise often preferred over cloud; air-gapped deployments
- **Budget-cyclical**: Annual budget cycles; must spend by fiscal year-end
- **Reference-dependent**: "Who else in government uses this?" is the first question
- **Risk-averse**: Nobody got fired for buying IBM/Microsoft/Salesforce
- **Long-cycle**: 6-24 months from first meeting to signed contract

## Reusable Component Patterns in Government

- **Case Management**: Track citizen requests, applications, investigations (also in insurance, legal, healthcare)
- **Workflow Automation**: Approval routing, multi-step processes (every enterprise)
- **Document Management**: Storage, OCR, classification, retention (every industry)
- **Audit Trail**: Immutable logging, chain of custody (banking, healthcare, any regulated industry)
- **RBAC with Clearance Levels**: Hierarchical access control (defense, intelligence, enterprise)
- **Citizen/Constituent Portal**: Self-service, status tracking, document upload (banking, insurance, utilities)
- **Data Exchange**: Cross-agency, standards-based integration (healthcare, supply chain)
- **Compliance Engine**: Regulation mapping, control automation, evidence collection (every regulated industry)
- **FOIA/Records Request**: Public records management (regulated industries with disclosure requirements)

## Government Product Archetypes

### Archetype 1: e-Government / Digital Services Platform
- **Problem**: Paper-based, in-person government services
- **Product**: Platform for digitizing any government service (permits, licenses, benefits)
- **Adjacent Markets**: Insurance claims, banking applications, university admissions
- **Product Score**: Usually 28-38 (huge TAM, high standardization, but government-specific procurement)

### Archetype 2: Regulatory Compliance Platform
- **Problem**: Keeping up with changing regulations, audit preparation
- **Product**: Regulatory intelligence + compliance management platform
- **Adjacent Markets**: Banking, healthcare, energy, any regulated industry
- **Product Score**: Usually 32-40 (cross-industry, regulation creates moat)

### Archetype 3: Government Data & Analytics Platform
- **Problem**: Data siloed across agencies, no insights
- **Product**: Data integration, analytics, BI for government
- **Adjacent Markets**: Enterprise data platforms (with government-specific compliance)
- **Product Score**: Usually 28-35 (large TAM but competitive)

### Archetype 4: Procurement Modernization
- **Problem**: Slow, manual, non-compliant procurement
- **Product**: e-Procurement platform with marketplace, workflow, compliance
- **Adjacent Markets**: Enterprise procurement (manufacturing, retail, healthcare)
- **Product Score**: Usually 30-38 (cross-industry, high standardization potential)

## Commercial Models That Work in Government

1. **Enterprise License + Annual Maintenance**: Government prefers CapEx over OpEx; one-time license with annual maintenance (18-22%) works well
2. **Subscription (SaaS)**: Growing acceptance, especially for cloud-first agencies; needs FedRAMP
3. **Fixed-Price Implementation + Recurring Platform Fee**: Common for larger deployments
4. **GSA Schedule / Framework Agreement**: Pre-negotiated pricing on government procurement vehicles accelerates sales

**Critical**: FedRAMP, StateRAMP, or equivalent certification is table stakes for U.S. government SaaS.

## Government-Specific Requirements to Plan For

- Section 508 / WCAG accessibility compliance
- FedRAMP / StateRAMP security authorization
- Data residency and sovereignty
- FOIA-compatible records management
- NIST cybersecurity framework alignment
- CJIS for law enforcement, HIPAA for health agencies
- Procurement vehicle: GSA Schedule, SEWP, NCPA, etc.

## Government Red Flags

- Customer insists on 100% on-premise, no cloud (shrinking but real segment)
- Requires security clearance for all support staff (limits scalability)
- Customization for one agency's unique legislation (not reusable)
- Procurement cycle > 18 months (capital efficiency problem)
- Customer is the only agency with this regulatory framework
