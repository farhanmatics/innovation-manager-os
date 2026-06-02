# Healthcare Industry Playbook

Domain-specific guidance for evaluating product opportunities in Healthcare, Life Sciences, and HealthTech.

## Industry DNA

Healthcare is the largest sector of the U.S. economy ($4.3T). It is simultaneously the most regulation-heavy, data-sensitive, and innovation-hungry industry. Products that navigate compliance successfully command premium pricing.

## Key Problems That Signal Product Opportunity

| Problem | Product Signal | Typical Buyer |
|---|---|---|
| EHR/EMR systems don't interoperate | Interoperability Platform / FHIR Gateway | CIO, CMIO |
| Prior authorization takes 7-14 days | Workflow Automation / PA Platform | COO, VP Revenue Cycle |
| Patient no-show rate exceeds 20% | Patient Engagement / Scheduling Platform | COO, VP Operations |
| Claims denial rate > 5% | RCM / Denial Management Platform | CFO, VP Revenue Cycle |
| Manual clinical documentation burdens clinicians | AI Clinical Documentation / Ambient AI | CMIO, CMO |
| Care coordination across providers fails | Care Coordination Platform | CMO, VP Population Health |
| Regulatory audits cause revenue clawbacks | Compliance / Audit Automation | CCO, VP Compliance |
| Patient acquisition cost rising | Patient Acquisition / CRM for Healthcare | CMO, VP Marketing |

## Healthcare Buyer Psychology

- **Patient safety above all**: Any product that could impact patient care faces extreme scrutiny
- **Compliance is existential**: HIPAA violations can kill a business. Compliance is not optional.
- **Clinician burnout is real**: Products must reduce, not increase, clinician workload
- **Interoperability is the holy grail**: "Does it work with Epic/Cerner/Meditech?" is question #1
- **ROI is measured in clinical + financial terms**: Show both or don't bother
- **Long adoption cycles**: 12-24 months from evaluation to enterprise-wide deployment
- **Evidence-obsessed**: Peer-reviewed studies, clinical trials, published outcomes matter

## Reusable Component Patterns in Healthcare

- **Interoperability Engine**: FHIR/HL7 data transformation (also in government, insurance for data exchange)
- **Workflow Automation**: Prior auth, referrals, discharge planning (every industry)
- **Clinical Decision Support**: Rules engine + evidence database (applicable to legal, compliance, any expert system)
- **Patient/Customer Portal**: Self-service, scheduling, communication (every consumer-facing industry)
- **Claims Processing Engine**: Adjudication rules, edits, payment calculation (insurance, government benefits)
- **Audit & Compliance Engine**: Regulatory mapping + evidence collection (every regulated industry)
- **AI/ML Diagnostic Support**: Image analysis, NLP for clinical notes (legal document review, insurance claims)
- **Care/Case Management**: Multi-stakeholder coordination (legal, social services, insurance claims)

## Healthcare Product Archetypes

### Archetype 1: Interoperability Platform
- **Problem**: Healthcare data trapped in siloed EHR systems
- **Product**: FHIR-based data exchange, normalization, API layer
- **Adjacent Markets**: Government (agency data sharing), Insurance (claims data), Life Sciences (RWD)
- **Product Score**: Usually 32-40 (regulatory mandate, universal problem, high IP)

### Archetype 2: Revenue Cycle Automation
- **Problem**: Manual billing, high denial rates, slow collections
- **Product**: AI-driven RCM with denial prediction, automated appeals, workflow
- **Adjacent Markets**: Insurance claims, legal billing, any complex billing
- **Product Score**: Usually 30-38 (massive TAM, quantifiable ROI, configurable rules)

### Archetype 3: AI Clinical Documentation
- **Problem**: Clinicians spend 2 hours on EHR for every 1 hour with patients
- **Product**: Ambient AI scribe, NLP documentation, CDI support
- **Adjacent Markets**: Legal (court transcription), enterprise (meeting notes), media
- **Product Score**: Usually 28-36 (high demand, AI IP, but competitive and EHR-dependent)

### Archetype 4: Patient Engagement Platform
- **Problem**: Disconnected patient experience, high no-shows, low adherence
- **Product**: Omnichannel engagement, scheduling, reminders, telehealth, education
- **Adjacent Markets**: Hospitality, retail, any appointment-based business
- **Product Score**: Usually 25-33 (large TAM but competitive, lower moat)

### Archetype 5: Regulatory Compliance Automation
- **Problem**: HIPAA, CMS, Joint Commission, state regulations — manual compliance
- **Product**: Continuous compliance monitoring, automated evidence collection, audit readiness
- **Adjacent Markets**: Banking, government, energy, any regulated industry
- **Product Score**: Usually 33-41 (regulation = moat, cross-industry, urgency-driven)

## Commercial Models That Work in Healthcare

1. **Subscription (SaaS)**: Increasingly standard for non-clinical systems. Fastest growing.
2. **Per Provider/Per Patient**: Pricing tied to usage metrics. Aligns with value.
3. **% of Revenue Uplift**: For RCM products. Risk-sharing model.
4. **Enterprise License + Maintenance**: For on-premise deployments at large health systems.
5. **Free Platform + Transaction Fees**: Growing model in patient payments, telehealth.

**Context**: ACV ranges from $10K (small practice) to $1M+ (large health system, per module).

## Healthcare-Specific Requirements

- **HIPAA Compliance** — Mandatory, BAA required
- **HITRUST Certification** — Increasingly required by payers and health systems
- **FDA / SaMD** — If clinical decision support, may require FDA clearance
- **SOC 2 Type II** — Standard enterprise requirement
- **21st Century Cures Act** — Information blocking rules, interoperability requirements
- **EHR Integration** — Epic App Orchard, Cerner code, at minimum FHIR APIs
- **Accessibility** — WCAG 2.1 AA, Section 508

## Healthcare Red Flags

- Product touches clinical care delivery (FDA risk, longer validation, liability)
- "Our solution replaces the EHR" (nobody replaces the EHR; integrate with it)
- Patient data stored outside HIPAA-compliant infrastructure
- Single-practice solution with no path to enterprise/health system
- Requires clinicians to change their workflow (adoption killer)
- Customer can't articulate ROI in both clinical AND financial terms
