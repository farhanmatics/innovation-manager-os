# Productization Framework

A systematic approach to transforming custom solutions into reusable enterprise products.

## Core Question

> Can 70% or more of this solution be standardized across multiple customers?

If yes, you have a product. If no, you have a services business.

## The Three-Layer Model

Every enterprise product has three layers:

```
┌─────────────────────────────────────────┐
│          CUSTOM EXTENSION LAYER          │ ← Customer-specific (0-30%)
│  Integrations, custom workflows,         │
│  proprietary algorithms, niche features  │
├─────────────────────────────────────────┤
│         CONFIGURATION LAYER              │ ← Industry/vertical-specific (10-40%)
│  Business rules, thresholds, templates,  │
│  compliance settings, branding           │
├─────────────────────────────────────────┤
│            PRODUCT CORE                  │ ← Universal (40-70%)
│  Engine, data model, security, APIs,     │
│  UI framework, core workflows            │
└─────────────────────────────────────────┘
```

### Product Core (40–70%)

These are features **every customer needs**. They form the foundation.

**Characteristics:**
- No configuration required for basic use
- Works out of the box
- Delivers standalone value
- Independent of industry vertical

**Examples:**
- Authentication and authorization (RBAC)
- Core data models and storage
- API layer and integration framework
- Dashboard and reporting engine
- Notification and alert infrastructure
- Audit trail and compliance logging
- Multi-tenancy architecture
- Basic CRUD workflows

**Acid Test:** Would a customer in a completely different industry find this useful?

### Configuration Layer (10–40%)

These are features that require **setup but not code changes**. Think settings, not development.

**Characteristics:**
- Changed via admin UI, config files, or API
- No developer required
- Industry-specific defaults and templates
- Tenant-specific business rules

**Examples:**
- Workflow definitions (BPMN or visual designer)
- Business rule thresholds (e.g., "alert if > $10,000")
- Report templates and schedules
- Notification templates and channels
- Role and permission definitions
- SLA parameters and escalation rules
- Data retention policies
- Branding and white-labeling
- Integration endpoint configurations

**Acid Test:** Can a business analyst configure this without involving engineering?

### Custom Extension Layer (0–30%)

These are **customer-specific developments** that cannot or should not be standardized.

**Characteristics:**
- Unique to one customer or a very small segment
- Requires custom development
- May involve proprietary algorithms
- Should be built as plugins/extensions, NOT core modifications

**Examples:**
- Integration with legacy proprietary systems
- Custom ML models trained on customer-specific data
- Unique regulatory requirements (single jurisdiction)
- Proprietary data formats and protocols
- Customer-specific UI customizations
- One-off reporting requirements

**Acid Test:** Would fewer than 3 customers ever need this?

## Productization Assessment Worksheet

### Step 1: Feature Inventory

List every feature/requirement in the project:

| # | Feature | Core? | Config? | Custom? | Rationale |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| ... | | | | | |

### Step 2: Calculate Percentages

```
Core Features:     ___ / ___ total = ___%
Config Features:   ___ / ___ total = ___%
Custom Features:   ___ / ___ total = ___%
```

### Step 3: Red Flag Check

Answer YES/NO:

- [ ] Custom layer exceeds 30%? → **Red Flag**: Low productization potential
- [ ] Core layer below 40%? → **Red Flag**: Too much variability
- [ ] Any custom feature that > 3 customers would need? → **Promote to Core or Config**
- [ ] Any config feature that requires developer to change? → **Redesign for admin UI**
- [ ] Any core feature that doesn't work standalone? → **Refactor for independence**

### Step 4: Productization Score

| Dimension | Weight | Score (1-5) | Weighted |
|---|---|---|---|
| Core coverage | 30% | | |
| Config flexibility | 25% | | |
| Custom isolation | 15% | | |
| API / extension points | 15% | | |
| Multi-tenancy readiness | 15% | | |
| **TOTAL** | 100% | | /5.0 |

**Interpretation:**
- 4.0+: Ready for productization
- 3.0–3.9: Needs refactoring before productization
- 2.0–2.9: Significant architecture changes needed
- < 2.0: Better as a services business

## Productization Patterns

### Pattern 1: Plugin Architecture
Custom features are built as plugins that plug into the core product.
- Core provides extension points (hooks, events, APIs)
- Plugins are independently deployable
- Plugin marketplace possible at scale

### Pattern 2: Multi-Tenant Configuration
Single codebase, multiple tenants, configuration-driven differentiation.
- Database-level or schema-level tenancy
- Tenant-specific config stored, not hardcoded
- Configuration versioning and migration support

### Pattern 3: White-Label Platform
Core product is rebrandable and resellable by partners.
- Full branding customization
- Domain/subdomain per tenant
- Partner admin portal
- Revenue sharing or licensing model

### Pattern 4: Industry Verticalization
Start horizontal, then build vertical-specific config packs.
- Core: universal platform
- Vertical Pack 1: Telecom-specific rules, dashboards, reports
- Vertical Pack 2: Banking-specific compliance, workflows
- Vertical Pack 3: Government-specific procurement, security

## Anti-Patterns to Avoid

1. **Forking the codebase per customer** — maintenance nightmare
2. **Hardcoding customer-specific business rules** — use configuration instead
3. **Building features without extension points** — every customization becomes a core modification
4. **Ignoring multi-tenancy from day one** — retrofitting is expensive
5. **Making configuration too technical** — requires developer, defeating the purpose
