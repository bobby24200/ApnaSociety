# 🏡 ApnaSociety
### **A Better Community Together**

> **Money people can understand.  
> Water people can measure.  
> Security people can access.  
> Communication people can trust.  
> Services people can rely on.**

ApnaSociety is a **resident-first smart apartment community management platform** designed for urban apartment communities in India.

It brings the most important parts of apartment living into one trusted digital ecosystem — **maintenance, expenses, water, communication, complaints, security, emergencies and local services**.

This README is a project-level implementation guide based on the **ApnaSociety Detailed Product Requirements Document (PRD)**.

---

# 🌱 Why ApnaSociety?

Apartment life is more than paying a monthly maintenance bill.

Residents need to know:

- Where their maintenance money is going
- How much water their home is consuming
- Whether their complaint is actually being resolved
- Where important society announcements are
- Who to contact during an emergency
- Which local service providers can be trusted
- What is happening inside their community

At the same time, society management needs better ways to manage:

**Residents → Bills → Expenses → Water → Complaints → Communication → Security → Services**

ApnaSociety connects these workflows into **one governed platform**.

---

# 🎯 Product Vision

> **Make every apartment community more transparent, connected, secure and responsible.**

## Mission

Give residents one trusted digital place to:

- Understand bills
- Monitor water
- Communicate with their community
- Access safety information
- Track complaints
- Get everyday services

And give society management the tools needed to operate the community efficiently.

---

# 🧩 The ApnaSociety Ecosystem

```text
                    APNASOCIETY
                         │
        ┌────────────────┼────────────────┐
        │                │                │
     RESIDENT         MANAGEMENT       PLATFORM
       APP             DASHBOARD         ADMIN
        │                │                │
        ├── Bills       ├── Billing      ├── Societies
        ├── Water       ├── Expenses     ├── Plans
        ├── Community   ├── Water        ├── Support
        ├── Complaints  ├── Complaints   ├── Audit
        ├── Security    ├── Security     └── Analytics
        └── Services    └── Reports
                         │
                         ▼
                  SMART WATER / IoT
                         │
                         ▼
                 DATA + ANALYTICS
```

---

# 🏢 Product Identity

| Property | Definition |
|---|---|
| Product | ApnaSociety |
| Tagline | A Better Community Together |
| Product Type | B2B2C apartment/community management platform |
| Market | Urban apartment communities in India |
| Domain | Residential Property Management / PropTech |
| Theme | Surakshit Bharat — Community Security |
| Primary Users | Residents, RWAs, society committees, property/facility managers |
| Platforms | Android/iOS app + web applications |
| Initial Revenue Model | Society subscription |
| Indicative Price | ₹100 per flat/month |

---

# 💚 Six Product Principles

### 1. 👨‍👩‍👧 Resident-First
Complex management processes should become simple resident experiences.

### 2. 🔎 Transparency
Bills, expenses and community information should be understandable.

### 3. ⚖️ Fairness
Where individual meters exist, residents should be able to see and pay according to their usage.

### 4. 🔐 Security
Financial, personal and CCTV information must have strong access controls.

### 5. 🚀 Progressive Adoption
A society should receive value even before smart IoT meters are installed.

### 6. 📈 Scalability
The architecture must support multiple independent apartment societies.

---

# 🔥 The Problem

## For Residents

Traditional apartment management can create:

- Lump-sum maintenance bills
- Limited visibility into expense categories
- Shared or fixed water allocation
- No visibility into current water consumption
- Scattered WhatsApp/notice-board communication
- Poor complaint tracking
- Difficulty finding trusted technicians
- Confusion around emergency information
- Lower trust between residents and management

## For Management

Management teams may deal with:

- Separate spreadsheets and systems
- Manual resident records
- Manual billing
- Payment follow-up and reconciliation
- Manual water readings
- Repeated communication
- Difficult complaint coordination
- Limited operational dashboards

### The Core Opportunity

> **Replace fragmented workflows with one governed platform connecting residents, management, payments, water data, security and local services.**

---

# 👥 Who Uses ApnaSociety?

| Role | What They Need |
|---|---|
| 🏠 Resident | Bills, water, updates, complaints, safety, services |
| 🏢 RWA/Society Admin | Residents, bills, expenses, communication |
| 💰 Treasurer | Collections, expenses, financial reporting |
| 📢 Secretary | Communication and administration |
| 🛠️ Facility Manager | Operations and issue resolution |
| 🛡️ Security Staff | Incidents, alerts and access tasks |
| 🔧 Service Provider | Approved service requests and profile |
| ⚙️ Platform Admin | Multi-society operations, support and audit |

---

# 📱 Resident Experience

## Home Dashboard

The resident's home screen brings important information together:

- Flat identifier
- Current maintenance amount
- Due status
- Current water consumption
- Previous-period comparison
- Open complaints
- Unread announcements
- Emergency/security shortcut
- Trusted-service shortcuts

The dashboard can be configured according to society needs.

---

# 💰 Transparent Maintenance & Billing

ApnaSociety turns a confusing maintenance amount into an understandable bill.

### Example

```text
Monthly Maintenance
────────────────────────
Security             ₹1,200
Housekeeping           ₹800
Utilities              ₹500
Repairs                ₹300
Water                  ₹250
Sinking Fund           ₹500
Other                  ₹150
────────────────────────
Total                ₹3,700
```

Residents can see:

- Current bill
- Due date
- Payment state
- Line-item breakdown
- Previous bills
- Receipts
- Fixed charges
- Variable charges
- One-time charges
- Late fees where configured
- Bill-related queries

---

# 🔍 Expense Transparency

Residents can view configured society expense information without exposing another resident's private financial data.

Management can maintain:

- Expense categories
- Monthly totals
- Supporting documents
- Approval states
- Closed-period records
- Audit history

Residents can see:

- Expense summaries
- Month-over-month movement
- Management explanations where configured
- Simple charts that improve understanding

---

# 💧 Fair Water: A Core ApnaSociety Experience

Water is one of the most important differentiators in the product.

Instead of only seeing a final water charge, residents can understand their consumption.

## Resident Water Dashboard

```text
THIS MONTH

Water Used
██████████████░░  7,840 L

Previous Month
6,950 L

Change
+12.8%

Estimated Charge
₹392

Meter
● Online
```

The system supports:

- Current-cycle usage
- Daily trends
- Weekly trends
- Monthly trends
- Previous-period comparison
- Estimated/actual charges
- Meter status
- Abnormal-use warnings
- Possible continuous-flow warnings
- Water issue reporting

---

# 📡 Smart Water Architecture

The proposed IoT architecture is:

```text
Smart Ultrasonic Meter
          ↓
   LoRaWAN Module
          ↓
   Society Gateway
          ↓
 Internet / 4G / Ethernet
          ↓
    IoT Ingestion
          ↓
       Validation
          ↓
        Storage
          ↓
 Billing + Analytics
          ↓
ApnaSociety App/Dashboard
```

### Meter Data

The platform can process:

- Meter ID
- Flat ID
- Timestamp
- Cumulative litres
- Interval consumption
- Flow rate
- Battery/device health
- Connectivity state
- Data-quality flags

### Data Quality Protection

The system should detect:

- Duplicate readings
- Impossible negative cumulative values
- Meter resets
- Sudden jumps
- Missing intervals
- Meter replacement events

Raw readings should be preserved separately from processed readings.

---

# ⚖️ Flexible Water Billing

ApnaSociety supports different society realities.

### Supported Models

1. Fixed monthly charge
2. Per-litre/per-unit charge
3. Tiered rate
4. Minimum charge + usage
5. Shared allocation
6. Hybrid fixed + usage-based charge

This allows a society to start simple and move toward smarter metering later.

---

# 🚨 Abnormal Usage ≠ Confirmed Leak

The initial system can use configurable thresholds and historical baselines.

For example:

```text
Normal Usage
██████████

Current Usage
██████████████████

⚠ Possible Abnormal Usage
```

The product should say **“possible abnormal usage”** rather than confirming a leak without verification.

---

# 📢 Community Communication

Residents should not have to search through hundreds of messages.

Announcements support:

- Title
- Category
- Message
- Attachments
- Expiry
- Priority
- Push notifications
- Pinned critical notices
- Read/unread state
- Society/tower/group targeting

### Priority Levels

| Priority | Example |
|---|---|
| 🔴 Critical | Emergency/security incident |
| 🟠 Important | Water shutdown/maintenance due |
| 🟢 Normal | Events/general notices |
| 🔵 Transactional | Bill/receipt/complaint update |

---

# 🛠️ Complaints & Issue Tracking

Every complaint becomes a trackable ticket.

### Lifecycle

```text
Created
   ↓
Assigned
   ↓
In Progress
   ↓
Resolved
   ↓
Confirmed
   │
   └──→ Reopened
```

A complaint can include:

- Category
- Description
- Photo/video where supported
- Location
- Priority
- Assigned person
- Ticket ID
- Status timeline
- Resolution details
- Resident confirmation

This replaces “I complained, but what happened?” with a visible workflow.

---

# 🛡️ Security & Emergency Center

ApnaSociety provides a central location for safety information.

### Features

- Emergency contacts
- Security notices
- Emergency alerts
- Incident reporting
- Quick-call actions
- Authorized CCTV access
- Camera access logs
- Revocable permissions

### Emergency Contacts

Configured contacts may include:

- Security
- Police
- Fire
- Ambulance
- Nearby hospital
- Electricity
- Water services

Emergency information must be verified by the society before launch.

---

# 📹 CCTV: Controlled, Not Open

CCTV is sensitive.

Therefore:

```text
User
 ↓
Role Check
 ↓
Society Policy
 ↓
Authorized Camera
 ↓
Logged Access
```

Access must be:

- Explicitly authorized
- Role-controlled
- Logged
- Revocable
- Limited to approved feeds

---

# 🔧 Trusted Local Services

Residents can discover verified providers for:

- Plumbing
- Electrical work
- Cleaning
- AC service
- Carpentry
- Appliance repair

Provider information can include:

- Verification status
- Service area
- Availability
- Ratings
- Reviews

### Rollout Strategy

**Phase 1:** Verified directory

**Later:** Service requests → Booking → Completion → Rating → Commission

---

# 🖥️ Management Command Center

The management dashboard is structured around:

```text
Overview
Residents
Billing
Expenses
Water
Complaints
Announcements
Security
Services
Reports
Settings
```

Management can:

- Create societies/towers/floors/flats
- Import residents
- Invite and verify residents
- Configure billing
- Generate bills in bulk
- Reconcile payments
- Manage expenses
- Configure water rules
- Manage complaints
- Publish announcements
- Manage security
- Verify providers
- Export reports

---

# 🔐 Security & Privacy Architecture

ApnaSociety treats trust as a product feature.

The PRD requires:

- HTTPS/TLS
- Secure authentication
- OTP rate limiting
- Role-based access control
- Society-level tenant isolation
- Flat-level data restrictions
- Least-privilege permissions
- Encryption at rest where appropriate
- Secrets management
- Audit logs
- Backup and restore testing
- Data retention/deletion policies

Payment credentials should not be stored by ApnaSociety.

---

# 💳 Payments & Financial Controls

Payments should use a compliant third-party gateway.

Supported states:

```text
Pending
   ↓
Paid

Pending → Failed
Pending → Refunded
Paid → Reversed
```

The platform should support:

- UPI
- Unique transaction IDs
- Webhooks
- Reconciliation
- Receipts
- Refund/reversal handling
- Idempotency
- Financial audit trails

**Goal:** a payment retry must never create a duplicate transaction.

---

# 🔔 Notification System

ApnaSociety uses priority-based communication.

```text
CRITICAL
Emergency / Security / Urgent Water Outage
        ↓
Push + Optional SMS/Email + Persistent Alert

IMPORTANT
Maintenance Due / Planned Shutdown
        ↓
Push + In-App

NORMAL
Events / General Notices
        ↓
In-App + Optional Push

TRANSACTIONAL
Receipts / Bills / Complaint Updates
        ↓
In-App / Push + Optional Email/SMS
```

---

# 📊 Analytics

## Resident Analytics

- Water trends
- Bill/payment history
- Complaint history
- Notification history

## Society Analytics

- Collection percentage
- Outstanding amount
- Expense distribution
- Water consumption
- Abnormal usage
- Complaint volume
- Resolution time
- Announcement reach
- Provider performance

## Platform Analytics

- Societies onboarded
- Monthly active residents
- Feature adoption
- Monthly recurring revenue
- Support tickets
- Retention/churn

---

# 🧠 Future Intelligence

ApnaSociety is designed to grow beyond basic management.

## 🤖 AI Bill Checker

Future capabilities:

- Detect unusual month-to-month increases
- Identify duplicate/unexpected line items
- Explain complex bills in plain language
- Flag charges requiring management explanation

## 📈 Community Transparency Score

Potential factors:

- Expense reporting
- Complaint resolution
- Communication
- Water reporting
- Resident participation

The score should be an **improvement indicator**, not a public shaming/ranking system.

## 🏙️ Future Smart Community

Possible future capabilities:

- Predictive maintenance
- Smart parking
- Energy monitoring
- More IoT sensors
- Community voting
- AI community assistant

---

# 🏗️ Technical Architecture

```text
┌───────────────────────────────┐
│     Resident App / Web        │
└───────────────┬───────────────┘
                ↓
┌───────────────────────────────┐
│          API Gateway          │
└───────────────┬───────────────┘
                ↓
┌───────────────────────────────┐
│       Authentication          │
└───────────────┬───────────────┘
                ↓
┌───────────────────────────────┐
│     Application Services      │
└───────────────┬───────────────┘
                ↓
┌───────────────────────────────┐
│ PostgreSQL + Object Storage   │
└───────────────┬───────────────┘
                ↓
   ┌────────────┬────────────┬────────────┐
   ↓            ↓            ↓            ↓
Payments   Notifications     IoT          CCTV
Gateway       / FCM       Ingestion      Adapter
```

---

# 💻 Recommended Technology Stack

| Layer | Technology |
|---|---|
| Mobile | React Native |
| Web | React.js / Next.js |
| Backend | Node.js + TypeScript |
| Database | PostgreSQL |
| IoT | MQTT + LoRaWAN |
| Cloud | AWS / Azure / GCP equivalent |
| Notifications | Firebase Cloud Messaging |
| Payments | Third-party compliant gateway |
| Monitoring | Cloud monitoring + error tracking |

---

# 🗄️ Core Data Model

```text
Society
 ├── Towers / Blocks
 │     └── Floors
 │           └── Flats
 │                 └── Residents
 │
 ├── Bills
 │     └── Bill Line Items
 │
 ├── Payments
 ├── Expenses
 ├── Water Meters
 │     └── Water Readings
 │
 ├── Complaints
 ├── Announcements
 ├── Emergency Contacts
 ├── Security Incidents
 ├── Cameras
 ├── Service Providers
 │     └── Service Requests
 │
 ├── Notifications
 ├── Audit Logs
 └── Subscription
```

---

# 🔌 API & Integration Areas

The platform should provide APIs for:

- Authentication
- Society/flat/resident management
- Billing
- Expenses
- Payments and webhooks
- Water-meter ingestion
- Water analytics
- Announcements
- Notifications
- Complaints
- CCTV adapters
- Service providers
- Reports/exports
- Audit/admin functions

---

# 🚦 MVP Prioritization

## P0 — Build First

```text
Authentication
Society Management
Resident Management
Maintenance Billing
Expense Breakdown
Payments
Announcements
Complaints
Emergency
Basic Water Dashboard
```

## P1 — Pilot / Phase 2

```text
Smart Meters
CCTV Integration
Verified Service Directory
```

## P2 — Later

```text
Service Booking
AI Bill Checker
Community Transparency Score
```

## P3 — Future

```text
Predictive Maintenance
```

---

# 🧪 Quality & Testing Strategy

Testing must cover:

### Functional
- Billing calculations
- Water calculations
- Complaint status transitions
- Payment states
- Notifications

### Security
- Authentication
- Permissions
- API security
- Tenant isolation
- CCTV access

### IoT
- Duplicate readings
- Missing readings
- Meter resets
- Outliers
- Connectivity problems

### Performance
- Monthly bill generation
- Announcement spikes
- Normal API response time

### UX
- Resident onboarding
- Bill/payment journey
- Water journey
- Complaint journey
- Real resident usability testing

---

# ⚡ Non-Functional Requirements

### Performance
Target common app/API actions at **under 2 seconds** under normal conditions, excluding external services.

### Availability
MVP target: **99.5%+**

### Scalability
Support multiple independent societies through multi-tenant architecture.

### Reliability
Payments, notifications and IoT ingestion should be idempotent where applicable.

### Observability
Use:

- Logs
- Metrics
- Traces
- Error tracking
- Health checks

### Resilience
The platform should gracefully handle:

- Weak connectivity
- Offline states
- Missing IoT data
- External service failures

---

# 🎨 Design System

The official ApnaSociety logo is the authoritative visual reference.

### Brand Palette

```text
Deep Navy   #062B3D  → Trust / Security / Navigation
Apna Green  #008F63  → Primary Actions / Success
Leaf Green  #59B92C  → Water / Sustainability
Sun Orange  #F7A916  → Warnings / Attention
White       #FFFFFF  → Surfaces / Backgrounds
```

### UX Rules

- Mobile-first resident experience
- Large readable bill and water numbers
- Clear paid/due/overdue states
- Clear warning/emergency states
- Plain-language labels
- Accessible contrast
- Comfortable touch targets
- Empty/loading/offline/error states
- Avoid dashboard overload
- Use charts only when they improve understanding
- Important actions should be reachable within 1–2 taps

---

# 🗺️ Product Roadmap

```text
PHASE 0
Design
  ↓
UX + Brand + Architecture + Prototype

PHASE 1
MVP
  ↓
Residents + Billing + Expenses + Payments
+ Announcements + Complaints + Emergency + Water

PHASE 2
Pilot
  ↓
Real Society + Support + Analytics

PHASE 3
IoT
  ↓
Smart Meters + Meter Health + Usage Alerts

PHASE 4
Growth
  ↓
Services + AI + Advanced Security

PHASE 5
Scale
  ↓
Multi-City + Integrations + Enterprise
```

---

# 💼 Business Model

## Primary Revenue

### Society Subscription

**Indicative price: ₹100 per flat/month**

Illustrative Year 1 example from the PRD:

```text
10 Societies
× 100 Flats
× ₹100/month
× 12 Months
────────────────
≈ ₹12 Lakh Revenue
```

## Future Revenue

- Service booking commissions
- Smart-meter installation/integration fees
- Premium analytics
- Advanced security integrations
- Enterprise/property-manager plans

### Indicative Initial Budget

| Area | Amount |
|---|---:|
| App + Web Development | ₹1.20 lakh |
| Cloud/Database/Software | ₹0.30 lakh |
| Smart-Meter Integration/Testing | ₹0.40 lakh |
| Marketing/Onboarding | ₹0.40 lakh |
| Support/Admin | ₹0.30 lakh |
| Legal/Miscellaneous | ₹0.20 lakh |
| **Total** | **₹2.80 lakh** |

> Financial figures in the PRD are planning assumptions, not audited forecasts or vendor quotations.

---

# 🥊 Competitive Positioning

ApnaSociety should not claim that competitors lack individual features.

The positioning is based on the **combination and clarity of the resident experience**.

| Alternative | Broad Positioning | ApnaSociety Position |
|---|---|---|
| MyGate | Community, security, payments, management | Transparency-led resident experience + fair-water story |
| NoBrokerHood | Operations, billing, security, smart-meter integrations | Resident-centric information design + unified transparency |
| ADDA | Accounting, ERP, community management | Simple resident experience + water visibility + convenience |
| WhatsApp/Sheets/Manual | Fragmented communication and records | One governed community platform |

---

# ⚠️ Risks & Mitigation

| Risk | Mitigation |
|---|---|
| Management resistance | Pilot with cooperative RWAs and prove time savings |
| Low resident engagement | Make bills, payments, water and emergency features highly useful |
| Smart-meter cost | Start with manual/imported data |
| IoT data gaps | Retries, buffering, validation and health states |
| Privacy concerns | Least privilege, consent and audit logs |
| Payment failures | Webhook reconciliation and idempotency |
| Feature overload | Strict MVP and phased roadmap |
| Feature overlap | Focus on resident experience, transparency and integration quality |

---

# 📏 Success Metrics

## Adoption
- Societies onboarded
- Registered residents

## Engagement
- Monthly active residents
- Feature usage

## Billing
- Collection rate
- Payment completion
- Billing queries

## Transparency
- Billing-related complaints
- Resident feedback

## Water
- Residents viewing usage
- Connected meters
- Abnormal-usage investigations

## Operations
- Complaint volume
- Average resolution time

## Communication
- Announcement reach/read rate

## Business
- MRR
- Average revenue per society
- Renewal/churn

## Services
- Provider count
- Service requests
- Completion/rating

---

# 🚀 Pilot Strategy

## Stage 1 — Prototype

Build clickable resident and management journeys.

**Success signal:** Users understand the key journeys.

## Stage 2 — MVP

Build core modules using manual/imported water data.

**Success signal:** Pilot-ready workflows.

## Stage 3 — Pilot

Onboard selected apartment societies.

**Success signal:** Real usage, feedback and operational validation.

## Stage 4 — IoT Pilot

Connect a limited number of smart meters.

**Success signal:** Accurate and stable readings and billing.

## Stage 5 — Growth

Add service booking, AI capabilities and advanced security.

**Success signal:** Higher retention and revenue.

## Stage 6 — Scale

Expand across cities and societies.

**Success signal:** Repeatable onboarding and support.

---

# ✅ Launch Readiness

Before launch:

- [ ] Official ApnaSociety logo finalized
- [ ] Brand colors finalized
- [ ] Privacy policy ready
- [ ] Terms ready
- [ ] Payment gateway verified
- [ ] Role/permission matrix reviewed
- [ ] Backup/recovery tested
- [ ] Audit logging enabled
- [ ] Resident onboarding guide ready
- [ ] Management guide ready
- [ ] Support escalation process ready
- [ ] Pilot society agreement completed
- [ ] Water-meter integration validated
- [ ] Emergency contacts verified
- [ ] Society security information verified

---

# 🧑‍💻 Development Philosophy

ApnaSociety should **not be built as only a landing page or visual mockup**.

The implementation should provide:

- Working navigation
- Role-based views
- Functional forms
- CRUD workflows
- Database persistence
- Authentication
- Realistic sample data
- Search/filter functionality
- Loading states
- Error states
- Notifications
- Resident and management workflows

The PRD should remain the **source of truth** when implementing features.

---

# 🧭 Representative User Stories

### Resident

> I want a line-item maintenance bill so I understand what I pay for.

### Resident

> I want to see my apartment's water consumption so I can monitor usage and charges.

### Resident

> I want emergency contacts in one place so I can respond quickly.

### Resident

> I want complaint tracking so I know whether my issue is progressing.

### Treasurer

> I want bulk bill generation and collections so monthly administration is easier.

### Manager

> I want water and meter-health analytics so abnormal usage can be investigated.

### Secretary

> I want targeted announcements so residents receive relevant information.

### Service Provider

> I want approved service requests so I can serve residents through a trusted channel.

---

# 🔮 What ApnaSociety Becomes

ApnaSociety starts with the everyday problems residents already face.

Then it grows into a connected smart-community layer:

```text
                    APNASOCIETY
                         │
       ┌─────────────────┼─────────────────┐
       ↓                 ↓                 ↓
   TRANSPARENT        FAIR WATER        COMMUNITY
      MONEY             USAGE          COMMUNICATION
       │                 │                 │
       └─────────────────┼─────────────────┘
                         ↓
                    SECURITY
                         ↓
                    SERVICES
                         ↓
                   SMART SOCIETY
                         ↓
                  AI + PREDICTION
```

The long-term vision is not simply to digitize society management.

It is to make apartment communities **easier to understand, easier to operate, safer to live in, and more connected**.

---

# 📌 Product Boundaries

The PRD explicitly identifies several items that require validation:

- Smart-water IoT architecture must be validated with actual hardware/network vendors.
- Financial projections and the ₹2.80 lakh development estimate are planning assumptions.
- Competitor capabilities should be rechecked before external publication.
- CCTV/security features must follow society authorization policies and applicable law.

---

# 🏁 Final Definition

> **ApnaSociety is a resident-first smart apartment community platform connecting the financial, water, communication, security and service layers of community living.**

### **A Better Community Together.** 🏡💚

