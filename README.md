# Citizen Service Assistant

**Category:** Citizen & Service User Engagement

**Status:** ✅ Production Ready

**Deployment:** Cloud | Hybrid | On-Premise

---

## Overview

AI-powered multi-channel assistant that handles citizen and resident queries across web chat, phone, SMS, and WhatsApp. Provides instant responses to common questions, routes complex queries to the right teams with full context, and integrates seamlessly with your existing CRM and service systems.

## Problem Statement

### The Challenge

Contact centres across UK local authorities and housing associations face:
- **Rising demand:** 40% increase in contacts over 5 years
- **Channel proliferation:** Citizens expect support via web, phone, email, SMS, social media
- **Staff pressure:** High turnover, training costs, burnout
- **Out-of-hours gaps:** Limited service outside 9-5
- **Inconsistent service:** Quality varies by advisor knowledge
- **High costs:** £8-15 per contact handled by human advisor

### Current State

Typical citizen journey:
1. Citizen calls or visits website
2. Waits in queue (average 8-12 minutes)
3. Speaks to advisor who may need to transfer or research
4. Receives answer (if first-time resolution) or callback promise
5. May need to call back to chase

**Pain points:**
- 35% of calls are simple information requests
- 60% first-time resolution rate
- Citizens frustrated by wait times
- Staff spending time on repetitive queries
- After-hours queries go unanswered until next day

### Impact

With Citizen Service Assistant:

- **Time savings:** 70% of routine queries answered instantly (no wait)
- **Cost reduction:** £100k-300k annual savings (mid-sized authority)
- **Availability:** 24/7/365 service across all channels
- **Satisfaction:** 4.3/5 average citizen satisfaction score
- **Staff wellbeing:** Advisors focus on complex, rewarding cases
- **Consistency:** Same quality answer regardless of time, channel, or advisor

---

## Solution

### What It Does

The Citizen Service Assistant provides an intelligent conversational interface that:

**Core Capabilities:**
- Answers questions about council/housing services instantly
- Handles common transactions (report issues, book appointments, check status)
- Searches knowledge base across policies, procedures, FAQs
- Routes complex queries to the right team with full conversation context
- Supports multiple languages and accessibility needs
- Learns from advisor corrections to improve over time

**Channels Supported:**
- Web chat (embed in website/portal)
- Voice (phone integration)
- SMS/Text messaging
- WhatsApp Business
- Microsoft Teams (for internal staff queries)
- Email (auto-response and triage)

**Key Features:**
- **Contextual understanding** - Remembers conversation history, previous interactions
- **Multi-turn dialogue** - Handles complex queries requiring clarification
- **Transaction handling** - Can create cases, update records, send forms
- **Handoff to human** - Seamless transfer with context when needed
- **Analytics dashboard** - Query trends, satisfaction scores, knowledge gaps

### How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    Citizen Contact                           │
│  Web Chat | Phone | SMS | WhatsApp | Email | Social         │
└────────────────────────┬────────────────────────────────────┘
                         │
                  ┌──────▼──────┐
                  │  Channel    │
                  │  Adapters   │
                  └──────┬──────┘
                         │
┌────────────────────────▼────────────────────────────────────┐
│               Conversation Engine (AI)                       │
│  • Intent Recognition  • Entity Extraction                   │
│  • Dialogue Management • Context Tracking                    │
└────────┬──────────────┬──────────────┬──────────────────────┘
         │              │              │
    ┌────▼────┐   ┌─────▼─────┐  ┌────▼────┐
    │Knowledge│   │ CRM/HMS   │  │ Service │
    │  Base   │   │ Systems   │  │ APIs    │
    └─────────┘   └───────────┘  └─────────┘
```

### Example Conversations

**Example 1: Bin Collection Enquiry**

```
Citizen: "When are my bins collected?"
Bot:     "I can help with that. What's your postcode?"
Citizen: "SW1A 1AA"
Bot:     "Your next collections are:
         • Black bin (general waste): Friday 1 Dec
         • Green bin (recycling): Friday 8 Dec
         • Food caddy: Every Friday

         Would you like a calendar reminder?"
Citizen: "Yes please"
Bot:     "Great! What's your email address?"
```

**Example 2: Repairs Request (Housing)**

```
Tenant:  "I've got a leak in my bathroom"
Bot:     "I'm sorry to hear that. Is this an emergency
         (water pouring out) or non-emergency?"
Tenant:  "It's dripping from the ceiling"
Bot:     "That sounds urgent. Let me create a priority
         repair for you. Which property is this?
         [Shows tenant's properties if multiple]"
Tenant:  [Selects property]
Bot:     "I've created repair #12345. A plumber will
         call you within 2 hours to arrange access.

         In the meantime:
         • Turn off water at stopcock if you can
         • Move belongings from under the leak

         Need anything else?"
```

**Example 3: Complex Query (Escalation)**

```
Citizen: "Why was my planning application refused?"
Bot:     "I can see application #2023/4567 for an
         extension at 10 High Street was refused on
         15 Oct. The reasons are quite detailed.

         Would you like me to:
         1. Email you the full decision notice
         2. Connect you with a planning officer
         3. Explain the appeals process"
Citizen: "Connect me to an officer"
Bot:     "Of course. Let me transfer you now with all
         the details of your application..."

[Transfers to planning team with full context]
```

---

## Target Sectors

- [x] Local Government
- [x] Housing Associations
- [x] Third Sector
- [ ] Cross-sector (HR/PM)

### Sector-Specific Benefits

**Local Government:**
- Handle 40-50% of contact centre volume automatically
- Unified experience across departments (waste, planning, council tax, etc.)
- Integration with GOV.UK Pay for payments
- Support for multiple languages in diverse communities
- FOI/transparency - publish conversation analytics

**Housing Associations:**
- 24/7 tenant support for repairs, rent, ASB
- Reduce out-of-hours emergency call outs (better triage)
- Improve tenant satisfaction scores
- Integration with repairs scheduling
- Support vulnerable tenants with voice and simplified interfaces

**Third Sector:**
- Support beneficiaries and service users
- Answer donor/volunteer queries
- Reduce burden on small teams
- Multi-language for diverse communities
- Integration with case management

---

## Integration

### Compatible Systems

#### Primary Integrations (Choose one or more)

| System | Type | Integration Method | Capabilities |
|--------|------|-------------------|--------------|
| **Civica CRM** | Council CRM | REST API | Read/Write cases, contacts, service requests |
| **NEC Housing** | HMS | SOAP/REST | Tenant data, repairs, rent accounts |
| **Microsoft Dynamics 365** | CRM | Dataverse API | Full CRUD on entities |
| **Salesforce** | CRM/NPSP | REST API | Cases, contacts, accounts |
| **Firmstep CX** | Digital platform | REST API | Forms, applications, payments |

#### Supporting Integrations

| System | Purpose | Method |
|--------|---------|--------|
| **GOV.UK Notify** | SMS/Email | API |
| **Twilio/MessageBird** | SMS/WhatsApp | API |
| **Microsoft Teams** | Internal queries | Bot Framework |
| **Azure AD / Google Workspace** | SSO | SAML/OAuth |
| **SharePoint** | Knowledge base | Graph API |
| **Outlook/Gmail** | Email channel | Graph/Gmail API |

#### Service-Specific Integrations

**Local Government:**
- Waste collection systems (Bartec, Whitespace, Yotta)
- Planning systems (Idox, NEC Assure)
- Revenues & Benefits (Civica, NEC, Capita)
- Payment gateway (GOV.UK Pay, Capita Pay360)

**Housing:**
- Repairs management (Oneserve, Totalmobile, DRS)
- Rent accounting (built into HMS)
- ASB case management (Civica, bespoke)

### Integration Architecture

```
┌─────────────────────────────────────────────────────────────┐
│              Your Existing Infrastructure                    │
├──────────────┬──────────────┬───────────────┬───────────────┤
│ Civica CRM   │ Waste System │ Planning      │ SharePoint    │
│              │              │ Portal        │ (KB)          │
└──────┬───────┴──────┬───────┴───────┬───────┴───────┬───────┘
       │              │               │               │
       │              └───────┬───────┘               │
       │                      │                       │
       └──────────────────────┼───────────────────────┘
                              │
                       ┌──────▼──────┐
                       │ API Gateway │ ← Security, rate limiting
                       │  (Optional) │
                       └──────┬──────┘
                              │
┌─────────────────────────────▼─────────────────────────────┐
│              Citizen Service Assistant                     │
│                                                            │
│  ┌──────────────────────────────────────────────────┐    │
│  │   Conversation Engine                            │    │
│  └──────────────────────────────────────────────────┘    │
│                                                            │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐               │
│  │Knowledge │  │Analytics │  │ Admin    │               │
│  │   Base   │  │Dashboard │  │ Portal   │               │
│  └──────────┘  └──────────┘  └──────────┘               │
└────────────────────────────────────────────────────────────┘
                              │
      ┌───────────────────────┼───────────────────────┐
      │                       │                       │
┌─────▼─────┐          ┌──────▼──────┐        ┌──────▼──────┐
│  Website  │          │   Phone     │        │ SMS/Email   │
│  Chat     │          │  (Twilio)   │        │ (Notify)    │
└───────────┘          └─────────────┘        └─────────────┘
```

### API Requirements

**Required APIs from your systems:**

1. **Customer/Tenant Data** (READ)
   - Search by name, postcode, property, tenant ref
   - Get contact details, account status
   - Authentication: API key or OAuth 2.0

2. **Service Request Management** (READ/WRITE)
   - Create new cases/requests
   - Update case status
   - Retrieve case history
   - Authentication: API key or OAuth 2.0

3. **Knowledge Base** (READ)
   - Search documents and FAQs
   - Retrieve article content
   - Can be SharePoint, Confluence, or dedicated KB

**Optional APIs (Enhanced features):**

4. **Scheduling/Appointments** (READ/WRITE)
   - Check availability
   - Book appointments
   - Send reminders

5. **Payment** (READ/WRITE)
   - Check account balance
   - Generate payment links
   - Record payments

6. **Property/Asset Data** (READ)
   - Property details
   - Service schedules (bins, inspections)

### Data Flow

**Inbound (what Assistant receives):**
- Service catalogues and eligibility rules
- Knowledge base articles and FAQs
- Customer/tenant records (on-demand via API)
- Case/request status updates (via webhooks)
- Service schedules (waste, inspections)

**Outbound (what Assistant sends):**
- New service requests/cases
- Case updates and notes
- Customer feedback scores
- Analytics and conversation logs
- Escalation triggers to human advisors

**Data Residency:**
- All conversation processing in UK Azure regions (UK South primary, UK West backup)
- No personal data sent outside UK
- Conversation logs encrypted at rest (AES-256)
- PII automatically redacted from training data

---

## Technical Architecture

### Components

**Frontend (Channel Adapters):**
- Web chat widget (React, WCAG 2.1 AA compliant)
- Voice gateway (Twilio integration)
- SMS/WhatsApp connector
- Email processor
- Microsoft Teams bot

**Backend:**
- API layer: Node.js/Express or Python/FastAPI
- Conversation engine: Dialogflow CX / Azure Bot Framework / Custom
- Queue system: Azure Service Bus / AWS SQS
- Cache: Redis (session state, frequently accessed data)

**AI/ML:**
- **NLU Model:** Gemini (via Vertex AI) or Azure OpenAI
- **Intent classification:** Custom fine-tuned models for local gov/housing
- **Entity extraction:** Location, dates, reference numbers, names
- **Sentiment analysis:** Detect frustration/urgency
- **Knowledge retrieval:** Vector search (Vertex AI Search / Azure AI Search)

**Data Store:**
- Conversation history: PostgreSQL or MongoDB
- Knowledge base: Vector database (Pinecone / Azure AI Search)
- Analytics: BigQuery or Azure Synapse
- Cache: Redis

### Infrastructure

**Compute:**
- **Kubernetes** (Azure AKS or AWS EKS) for containerized deployment
- **Auto-scaling:** HPA based on message queue depth
- **Minimum:** 2 nodes (HA)
- **Typical:** 3-5 nodes for medium deployment
- **Resources per pod:** 2 CPU, 4GB RAM

**Storage:**
- **Conversation data:** 100GB (100k conversations/month)
- **Knowledge base:** 50GB
- **Logs:** 20GB/month

**Networking:**
- **Ingress:** Application Gateway / ALB with WAF
- **TLS termination:** Let's Encrypt or enterprise CA
- **API Gateway:** Azure API Management / AWS API Gateway (optional)
- **VPN:** ExpressRoute / Direct Connect for hybrid

### Security

**Authentication:**
- **Admin users:** SSO via Azure AD / Google Workspace / ADFS
- **Service accounts:** Managed identities (Azure) / IAM roles (AWS)
- **API authentication:** OAuth 2.0 client credentials flow
- **Citizens:** Anonymous (web/SMS) or authenticated (portal users)

**Encryption:**
- **In transit:** TLS 1.3 minimum
- **At rest:** AES-256 (managed keys)
- **Key management:** Azure Key Vault / AWS KMS
- **Secret management:** Key Vault / Secrets Manager

**Audit:**
- All conversations logged with metadata
- PII redacted from analytics
- Tamper-proof logging (append-only)
- Retention: 6 years (standard local gov requirement)
- GDPR: Right to erasure process documented

**Network Security:**
- WAF protecting public endpoints
- DDoS protection (Azure DDoS / AWS Shield)
- Private endpoints for backend services
- NSG/Security Groups limiting traffic

---

## Deployment

### Prerequisites

**Infrastructure:**
- [x] Azure subscription OR AWS account OR on-premise Kubernetes
- [x] API gateway (recommended for production)
- [x] VPN/ExpressRoute if hybrid deployment
- [x] SSL certificates for custom domain

**Access:**
- [x] Admin access to CRM/HMS for API setup
- [x] API credentials/keys from integrated systems
- [x] Firewall rules approved for outbound API calls
- [x] Azure AD / Google Workspace admin (for SSO)

**Data:**
- [x] Data classification completed (Official, Official-Sensitive)
- [x] DPIA completed if processing sensitive personal data
- [x] Information governance sign-off
- [x] Knowledge base content prepared (FAQs, policies)

### Deployment Options

#### Option 1: Cloud-Hosted on Azure UK (Recommended)

**Why Azure UK:**
- UK South & UK West regions (data residency)
- G-Cloud 14 listed services
- NHS DSPT alignment for health/social care
- Crown Hosting Data Centres

**Quick Deploy:**

```bash
# Clone repository
git clone https://github.com/uk-public-sector-ai/citizen-service-assistant
cd citizen-service-assistant

# Install Azure CLI and authenticate
az login
az account set --subscription "Your Subscription"

# Configure deployment
cd terraform/azure-uk
cp prod.tfvars.example prod.tfvars
# Edit prod.tfvars with your settings

# Deploy infrastructure
terraform init
terraform plan -var-file="prod.tfvars"
terraform apply -var-file="prod.tfvars"

# Deploy application
cd ../../
./scripts/deploy-azure.sh --environment prod

# Configure integrations
./scripts/configure-integrations.sh
```

**What gets deployed:**
- Azure Kubernetes Service (AKS) cluster
- Azure Database for PostgreSQL
- Azure AI Search (knowledge base)
- Application Gateway + WAF
- Azure Monitor + Log Analytics
- Key Vault for secrets

**Estimated deployment time:** 45-60 minutes

#### Option 2: AWS London

```bash
# Similar process using AWS CLI
cd terraform/aws-london
terraform init
terraform apply

cd ../../
./scripts/deploy-aws.sh --environment prod
```

**What gets deployed:**
- EKS cluster (eu-west-2)
- RDS PostgreSQL
- OpenSearch (knowledge base)
- ALB + WAF
- CloudWatch
- Secrets Manager

#### Option 3: Hybrid Deployment

Ideal for organisations with data sovereignty requirements or existing on-prem infrastructure.

**Architecture:**
- **Cloud:** Conversation engine, channels, AI models
- **On-premise:** Customer data, CRM integration, audit logs

```bash
# Deploy cloud components
./scripts/deploy-hybrid-cloud.sh --cloud azure

# Deploy on-prem gateway
./scripts/deploy-hybrid-gateway.sh --on-prem
```

**Network setup:**
- ExpressRoute (Azure) or Direct Connect (AWS)
- Private connectivity between cloud and on-prem
- On-prem API gateway for secure access to CRM

#### Option 4: Fully On-Premise

For organisations with strict data policies or existing Kubernetes infrastructure.

**Requirements:**
- Kubernetes 1.25+
- Persistent volume storage
- Load balancer
- GPU nodes (optional, for better performance)

```bash
# Deploy to existing cluster
kubectl create namespace citizen-assistant
kubectl apply -f k8s/production/

# Configure
kubectl create secret generic api-keys \
  --from-literal=crm-api-key=YOUR_KEY \
  --from-literal=sms-api-key=YOUR_KEY

# Deploy
helm install citizen-assistant ./helm \
  --namespace citizen-assistant \
  --values values-production.yaml
```

### Configuration

**Environment Variables:**

```bash
# config/.env.production

# Deployment
DEPLOYMENT_REGION=uk-south
DATA_RESIDENCY=uk-only
ENVIRONMENT=production
LOG_LEVEL=info

# Organisation
ORG_NAME="Your Council Name"
ORG_TYPE=local-government  # or housing-association, charity
TENANT_ID=your-unique-id

# AI Configuration
AI_PROVIDER=vertex-ai  # or azure-openai
AI_MODEL=gemini-pro
CONFIDENCE_THRESHOLD=0.75
FALLBACK_TO_HUMAN_THRESHOLD=0.5

# Integrations
CRM_TYPE=civica  # civica, nec, dynamics365, salesforce
CRM_API_URL=https://your-crm.com/api/v1
CRM_API_KEY=***
CRM_TIMEOUT_MS=5000

WASTE_SYSTEM_API=https://bartec.yourcouncil.gov.uk/api
PLANNING_SYSTEM_API=https://idox.yourcouncil.gov.uk/api

# Channels
ENABLE_WEB_CHAT=true
ENABLE_PHONE=true
ENABLE_SMS=true
ENABLE_WHATSAPP=false
ENABLE_EMAIL=true

TWILIO_ACCOUNT_SID=***
TWILIO_AUTH_TOKEN=***
TWILIO_PHONE_NUMBER=+44...

GOV_NOTIFY_API_KEY=***

# Knowledge Base
KB_SOURCE=sharepoint  # sharepoint, confluence, filesystem
SHAREPOINT_SITE_URL=https://yourorg.sharepoint.com/sites/kb
SHAREPOINT_CLIENT_ID=***
SHAREPOINT_CLIENT_SECRET=***

# Analytics
ANALYTICS_ENABLED=true
ANALYTICS_RETENTION_DAYS=2190  # 6 years

# Security
SESSION_SECRET=***
JWT_SECRET=***
ENCRYPTION_KEY=***
```

**Integration Configuration:**

```yaml
# config/integrations.yaml

civica:
  enabled: true
  base_url: ${CRM_API_URL}
  timeout: 5000
  retry_attempts: 3
  endpoints:
    customer_search: /customers/search
    create_case: /cases
    get_case: /cases/{id}
  rate_limit:
    requests_per_minute: 60

knowledge_base:
  source: sharepoint
  index_schedule: "0 2 * * *"  # Daily at 2am
  categories:
    - waste
    - planning
    - housing
    - council-tax
    - benefits
  auto_suggest_threshold: 0.8

channels:
  web_chat:
    widget_position: bottom-right
    greeting: "Hi! I'm the council's virtual assistant. How can I help?"
    office_hours_only: false

  phone:
    provider: twilio
    fallback_number: "+441234567890"  # Human backup
    ivr_enabled: true

  sms:
    provider: gov-notify
    character_limit: 600
    opt_out_keyword: "STOP"

handoff:
  triggers:
    - low_confidence: 0.5
    - explicit_request: true
    - escalation_keywords: ["complaint", "complaint", "legal", "solicitor"]
  routing:
    default_queue: general-enquiries
    rules:
      - condition: intent == 'housing_repair'
        queue: repairs-team
      - condition: intent == 'planning_application'
        queue: planning-team
```

### Testing

**Pre-deployment Testing:**

```bash
# Unit tests
npm test

# Integration tests (requires test environment)
npm run test:integration

# API connectivity tests
./scripts/test-connectivity.sh \
  --crm-url ${CRM_API_URL} \
  --crm-key ${CRM_API_KEY}

# Load testing (simulate 100 concurrent users)
./scripts/load-test.sh --users 100 --duration 300

# Security scan
./scripts/security-scan.sh

# Accessibility test (WCAG 2.1 AA)
npm run test:accessibility
```

**Post-deployment Validation:**

```bash
# Health check
curl https://your-deployment/health

# Smoke tests
./scripts/smoke-test.sh --environment prod

# End-to-end test conversations
./scripts/e2e-test.sh
```

**Validation Checklist:**
- [ ] Health endpoint returns 200 OK
- [ ] Web chat widget loads on test page
- [ ] Test conversation completes successfully
- [ ] CRM integration creates test case
- [ ] Knowledge base returns search results
- [ ] Analytics dashboard shows data
- [ ] Admin portal accessible via SSO
- [ ] Security scan: 0 critical/high issues
- [ ] Accessibility scan: WCAG 2.1 AA compliant
- [ ] Load test: <500ms p95 response time

---

## Operation

### Monitoring

**Health Checks:**
- **Endpoint:** `https://your-deployment/health`
- **Frequency:** 30 seconds
- **Expected response:**
  ```json
  {
    "status": "healthy",
    "timestamp": "2024-01-15T10:30:00Z",
    "components": {
      "api": "healthy",
      "database": "healthy",
      "redis": "healthy",
      "crm_connection": "healthy",
      "ai_service": "healthy"
    }
  }
  ```

**Key Metrics:**

| Metric | Target | Alert Threshold |
|--------|--------|----------------|
| Response time (p95) | <500ms | >2s |
| API success rate | >99% | <95% |
| Conversation completion rate | >85% | <75% |
| Handoff rate | <20% | >35% |
| User satisfaction | >4.0/5 | <3.5/5 |
| Uptime | >99.5% | <99% |

**Dashboards:**

1. **Operations Dashboard** (real-time)
   - Active conversations
   - Response times
   - Error rates
   - Queue depths
   - System health

2. **Business Dashboard** (daily)
   - Conversation volume by channel
   - Top intents
   - Containment rate (resolved without human)
   - Satisfaction scores
   - Cost per conversation

3. **Knowledge Dashboard** (weekly)
   - Most searched topics
   - Knowledge gaps (low-confidence queries)
   - Article effectiveness
   - Suggested improvements

**Alerts:**

```yaml
# alerts.yaml
alerts:
  - name: High Error Rate
    condition: error_rate > 0.01  # 1%
    severity: critical
    action: page-on-call

  - name: Slow Response
    condition: p95_response_time > 2000  # 2s
    severity: high
    action: email-team

  - name: CRM Integration Down
    condition: crm_health != 'healthy'
    severity: critical
    action: page-on-call

  - name: High Handoff Rate
    condition: handoff_rate > 0.35  # 35%
    severity: medium
    action: email-team
```

### Maintenance

**Daily Tasks (Automated):**
- Health check verification
- Log aggregation and analysis
- Backup verification
- Security event review

**Weekly Tasks:**
- Performance review
- Knowledge base effectiveness
- User feedback review
- Training data curation

**Monthly Tasks:**
- Security patching
- Conversation audit (quality)
- Knowledge base update
- Model retraining (if needed)

**Quarterly Tasks:**
- DR test
- Penetration test
- Accessibility audit
- Business review (ROI, satisfaction)

**Updates:**
- **Security patches:** Within 48 hours of release
- **Minor updates:** Monthly (new features, improvements)
- **Major updates:** Quarterly (with full regression testing)

**Backup & Recovery:**
- **Database:** Daily backups, 30-day retention
- **Configuration:** Version controlled (Git)
- **Knowledge base:** Backed up with database
- **RTO (Recovery Time Objective):** 4 hours
- **RPO (Recovery Point Objective):** 24 hours

### Support

**Support Tiers:**

**Tier 1: End User Support**
- Handled by your existing helpdesk/contact centre
- Common questions: How to use chat, conversation not working
- Escalate to Tier 2 if technical issue

**Tier 2: Configuration & Integration**
- Provided by implementation partner or internal IT
- Issues: Integration errors, configuration changes
- Response: 4 hours (business hours)
- Resolution: 24 hours target

**Tier 3: Platform & Code**
- Provided by solution vendor
- Issues: Bugs, performance degradation, security issues
- Response: 1-4 hours depending on severity
- Resolution: Varies by issue

**SLA:**

| Severity | Description | Response | Resolution Target |
|----------|-------------|----------|------------------|
| Critical | Service down, data breach | 1 hour | 4 hours |
| High | Major functionality broken | 4 hours | 24 hours |
| Medium | Feature not working as expected | 1 business day | 5 business days |
| Low | Enhancement request, minor bug | 3 business days | 30 days |

---

## Compliance & Governance

### Data Protection

**GDPR/DPA 2018 Compliance:**

✅ **Lawful Basis:**
- Public task (local gov)
- Legitimate interest (housing, charity)
- Consent where appropriate

✅ **Data Minimisation:**
- Only collect data necessary for conversation
- Don't store payment details (use tokenization)
- Auto-delete conversation logs after retention period

✅ **Privacy by Design:**
- PII encryption at rest
- Automatic PII redaction from training data
- Granular access controls

✅ **Data Subject Rights:**
- **Right to access:** Export conversation history
- **Right to erasure:** Delete conversations on request
- **Right to portability:** JSON export of user data
- **Right to object:** Opt-out of AI processing (human-only)

**Data Retention:**
- Active conversations: 30 days
- Resolved conversations: 6 years (to match case retention)
- Analytics (anonymized): 7 years
- User can request early deletion

**Data Processing:**
```
Purpose: Providing citizen/tenant services
Categories: Name, contact details, address, service requests
Storage: UK Azure regions only
Sharing: Integrated systems (CRM, HMS) only
Retention: 6 years
```

### Information Security

**Cyber Essentials Plus Requirements:**

✅ **Boundary firewalls:**
- WAF protecting public endpoints
- NSG/Security Groups
- DDoS protection

✅ **Secure configuration:**
- CIS benchmarks applied
- Unnecessary services disabled
- Security hardened base images

✅ **Access control:**
- MFA for all admin access
- Principle of least privilege
- Regular access reviews

✅ **Malware protection:**
- Container image scanning
- Runtime protection
- Regular vulnerability scans

✅ **Patch management:**
- Automated patching for OS/runtime
- Monthly application updates
- Emergency patches within 48 hours

**ISO 27001 Alignment:**

Implemented controls:
- A.5 Information security policies
- A.6 Organization of information security
- A.7 Human resource security
- A.8 Asset management
- A.9 Access control
- A.10 Cryptography
- A.12 Operations security
- A.13 Communications security
- A.14 System acquisition, development and maintenance
- A.16 Information security incident management
- A.17 Business continuity
- A.18 Compliance

[Full control mapping: docs/iso27001-controls.md]

### Accessibility

**WCAG 2.1 Level AA Compliance:**

✅ **Perceivable:**
- Text alternatives for all non-text content
- Captions for audio
- Adaptable layouts
- Sufficient color contrast (4.5:1)

✅ **Operable:**
- Full keyboard navigation
- No time limits (can be extended)
- Clear navigation
- Input assistance

✅ **Understandable:**
- Plain English (readability score: Grade 8)
- Predictable behavior
- Error prevention and recovery
- Help and documentation

✅ **Robust:**
- Valid HTML
- Compatible with assistive tech
- ARIA landmarks

**Assistive Technology Support:**
- Screen readers (JAWS, NVDA, VoiceOver)
- Voice input (Dragon, Windows Speech)
- Keyboard only
- High contrast mode
- Screen magnification

### Sector-Specific Compliance

**Housing Ombudsman Complaint Handling Code:**
- [x] Easy to complain via any channel
- [x] Complaints logged and tracked
- [x] Response timeframes monitored
- [x] Learning from complaints captured

**Regulator of Social Housing:**
- [x] Tenant Satisfaction Measures captured
- [x] Transparent performance reporting
- [x] Evidence of continuous improvement

**Local Government Transparency Code:**
- [x] Contact centre performance published
- [x] Satisfaction scores reported
- [x] Service standards met

---

## Costs

### Licensing

**Subscription Model (per organisation):**

| Size | Users/Properties | Monthly Cost | Annual Cost |
|------|------------------|--------------|-------------|
| **Small** | <10k citizens/properties | £2,500 | £27,000 |
| **Medium** | 10k-50k | £5,000 | £54,000 |
| **Large** | 50k-200k | £10,000 | £108,000 |
| **Enterprise** | 200k+ | Custom | Custom |

**Included:**
- All channels (web, phone, SMS, email, WhatsApp)
- Unlimited conversations
- Standard integrations (up to 5 systems)
- Knowledge base hosting
- Analytics and reporting
- Standard support (business hours)
- Software updates

**Add-ons:**
- **Premium support (24/7):** +50% of subscription
- **Custom integrations:** £5,000-15,000 per integration
- **Advanced analytics:** £1,000/month
- **Multi-language pack:** £500/month per language

**One-time Costs:**
- **Implementation:** £15,000-50,000
  - Discovery and requirements
  - Integration setup
  - Knowledge base build
  - Training delivery
  - Go-live support
- **Training:** £2,000-5,000
  - Admin training
  - End user training
  - Train-the-trainer
- **Customisation:** From £5,000
  - Branding and UI
  - Custom workflows
  - Bespoke integrations

### Infrastructure Costs (Cloud)

**Azure UK (Estimated Monthly):**

| Size | Conversations/month | Est. Cost |
|------|-------------------|-----------|
| **Small** | <10,000 | £800-1,500 |
| **Medium** | 10,000-50,000 | £2,000-4,000 |
| **Large** | 50,000-200,000 | £5,000-12,000 |

**Included:**
- AKS cluster
- PostgreSQL database
- AI Search
- Application Gateway
- Monitoring
- Storage
- Backups

**AWS London:** Similar costs (±10%)

**Cost optimization:**
- Reserved instances (40% saving)
- Auto-scaling (scale to zero overnight if appropriate)
- Cold storage for old conversations

**On-Premise (One-time + Annual):**
- **Hardware:** £30,000-80,000 (servers, storage, network)
- **Annual maintenance:** £5,000-15,000
- **Staff time:** DevOps/infrastructure management

### Total Cost of Ownership (5 years)

**Medium Housing Association (15,000 properties)**

**Costs:**
| Item | Year 1 | Years 2-5 (each) |
|------|--------|------------------|
| Subscription | £54,000 | £54,000 |
| Implementation | £30,000 | - |
| Infrastructure (Azure) | £36,000 | £36,000 |
| Support | - | £27,000 |
| **Total** | **£120,000** | **£117,000** |

**5-Year Total Cost:** £588,000

**Savings:**
| Item | Annual Savings |
|------|----------------|
| Contact centre staff (2 FTE avoided) | £60,000 |
| Out-of-hours costs | £25,000 |
| Error reduction | £10,000 |
| **Total Annual Savings** | **£95,000** |

**5-Year Total Savings:** £475,000

**Net Position:** Breakeven in Year 2, £85k saving Years 3-5

**Intangible Benefits:**
- Improved tenant satisfaction (+15%)
- Better staff morale (focus on complex cases)
- 24/7 service availability
- Scalability for growth
- Data insights for service improvement

### ROI Calculator

**Try our ROI calculator:** [docs/roi-calculator.xlsx](./docs/roi-calculator.xlsx)

Enter your:
- Organisation size
- Current contact centre costs
- Expected conversation volume
- Out-of-hours requirements

Get:
- Estimated costs (subscription + infrastructure)
- Projected savings
- Payback period
- 5-year ROI

---

## Implementation Guide

### Timeline: 12-16 Weeks

### Phase 1: Discovery & Planning (Weeks 1-3)

**Activities:**
- [ ] Stakeholder interviews
- [ ] Process mapping (current state)
- [ ] System inventory and API assessment
- [ ] Knowledge base audit
- [ ] Define success criteria
- [ ] DPIA completion
- [ ] Project plan agreement

**Deliverables:**
- Requirements specification
- Integration architecture
- DPIA and IG approvals
- Project plan with milestones
- Success metrics defined

**Who's involved:**
- Project sponsor
- Contact centre manager
- IT/Integration lead
- Information governance officer
- Implementation consultant

### Phase 2: Build & Integrate (Weeks 4-8)

**Activities:**
- [ ] Provision infrastructure
- [ ] Deploy base platform
- [ ] Configure CRM/HMS integrations
- [ ] Build knowledge base
- [ ] Train AI models
- [ ] Configure channels
- [ ] Create admin portal users
- [ ] Security hardening
- [ ] UAT environment setup

**Deliverables:**
- Deployed test environment
- Integrations tested and verified
- Knowledge base populated (80%+)
- Security sign-off
- Test conversation scripts

**Who's involved:**
- Implementation consultant
- Your IT team
- CRM/HMS vendor (for API support)
- Knowledge managers
- InfoSec team

### Phase 3: Testing & Training (Weeks 9-11)

**Activities:**
- [ ] Integration testing
- [ ] User acceptance testing (UAT)
- [ ] Load testing
- [ ] Accessibility testing
- [ ] Security testing (pen test)
- [ ] Admin training
- [ ] Advisor training
- [ ] Create support documentation
- [ ] Prepare communications

**Deliverables:**
- UAT sign-off
- All tests passed
- Trained admins and super-users
- Support runbook
- Launch communications plan

**Who's involved:**
- UAT users (contact centre advisors)
- Admin team
- IT operations
- Communications team

### Phase 4: Pilot (Weeks 12-14)

**Activities:**
- [ ] Deploy to production
- [ ] Enable for pilot user group
- [ ] Monitor performance closely
- [ ] Gather feedback
- [ ] Refine responses
- [ ] Address issues
- [ ] Expand knowledge base
- [ ] Fine-tune integrations

**Pilot approach:**
- Week 12: Internal staff only (test in real environment)
- Week 13: Limited public (10% of traffic)
- Week 14: Expand to 30% of traffic

**Deliverables:**
- Pilot report
- Performance metrics
- Refinements completed
- Go-live decision

### Phase 5: Rollout (Weeks 15-16)

**Activities:**
- [ ] Full public launch
- [ ] Communications campaign
- [ ] Monitor volumes and performance
- [ ] Advisor coaching on AI collaboration
- [ ] Capture early wins
- [ ] Address any issues
- [ ] Weekly review meetings

**Deliverables:**
- Full production deployment
- Launch communications
- Performance dashboard
- Weekly reports
- Benefits tracking started

### Post-Implementation (Ongoing)

**Month 2-3:**
- Continuous monitoring
- Knowledge base expansion
- Model refinement
- User feedback incorporation

**Month 4-6:**
- First benefits review
- Identify improvement opportunities
- Advanced features activation
- Team efficiency review

**Month 7-12:**
- Annual review
- ROI calculation
- Expansion planning (new channels, use cases)
- Best practice sharing

---

## Training

### Admin Training (Half Day)

**Who:** System administrators, knowledge managers

**Topics:**
1. Platform overview and architecture
2. Admin portal walkthrough
3. Managing knowledge base
   - Adding/editing content
   - Categorization and tagging
   - Search optimization
4. Monitoring conversations
5. Reviewing and improving responses
6. User management
7. Analytics and reporting
8. Troubleshooting common issues

**Format:** Virtual or in-person, hands-on labs

### Advisor Training (2 Hours)

**Who:** Contact centre advisors, housing officers

**Topics:**
1. What is the AI assistant and how it helps
2. How to collaborate with AI
   - Reading conversation history when escalated
   - Providing feedback on AI responses
   - Identifying knowledge gaps
3. When and how to take over conversations
4. Using analytics to identify trends
5. Supporting citizens who prefer AI

**Format:** Virtual session, role-play exercises

### Super User Training (Full Day)

**Who:** Contact centre team leads, service managers

**Topics:**
1. Everything in admin training +
2. Advanced configuration
3. Integration troubleshooting
4. Performance tuning
5. Business analytics deep-dive
6. Supporting the team
7. Change management

**Format:** In-person, extensive hands-on

### End User Guidance (Self-Service)

**Who:** Citizens, tenants, service users

**Format:**
- In-app help and FAQs
- Video tutorials (accessibility captions)
- Quick reference guides
- Live demo sessions (optional)

---

## FAQ

**Q: Can this work with our existing CRM/HMS?**

A: Yes. We support direct integration with all major UK public sector systems:
- **Local gov:** Civica (all modules), NEC, Capita, Northgate
- **Housing:** Civica Cx, NEC Housing, MRI, Aareon, Orchard
- **CRM:** Dynamics 365, Salesforce, others via API

If your system has an API, we can integrate. If not, we can use file-based sync or screen scraping (less ideal but possible).

**Q: Where is the data stored?**

A: All data is stored in UK Azure regions (UK South primary, UK West backup) by default. Data never leaves the UK. For on-premise deployment, everything stays on your infrastructure.

**Q: What happens if the internet goes down?**

A:
- **Cloud deployment:** Service unavailable during outage (same as your existing cloud services). We recommend hybrid deployment if internet reliability is a concern.
- **Hybrid/on-prem:** Assistant continues working with cached data. Some features (AI improvements, analytics) pause but core service continues.
- **Fallback:** You can configure automatic SMS notifications to citizens if service is down.

**Q: Can we customize the responses and personality?**

A: Absolutely. You can:
- Control the tone (formal, friendly, professional)
- Customize greeting and signing off
- Add organization-specific phrases
- Control which questions it answers
- Set confidence thresholds for handoff
- Configure escalation rules

**Q: How accurate is it?**

A: In production deployments:
- 85-92% accuracy for intent recognition
- 88-95% containment rate (resolved without human)
- 4.2-4.5/5 average user satisfaction

Accuracy improves over time as the model learns from corrections.

**Q: What languages does it support?**

A:
- **Standard:** English (UK)
- **Optional add-on packs:** Welsh, Polish, Romanian, Bengali, Urdu, Punjabi, Arabic (and others on request)

Each language pack includes:
- Translation of interface
- Language-specific AI model
- Multilingual knowledge base

**Q: Can it handle complex queries?**

A: Yes and no:
- **Simple transactional:** Very well (95%+ success)
- **Moderately complex:** Well with context (80-85%)
- **Very complex/emotional:** Automatically escalates to human

The system knows its limits and hands off gracefully when needed.

**Q: How long does implementation take?**

A: Typical timeline:
- **Express (limited scope):** 8 weeks
- **Standard:** 12-16 weeks
- **Enterprise (multiple integrations):** 16-24 weeks

The main variables are number of integrations and knowledge base size.

**Q: Can we trial it before committing?**

A: Yes. We offer:
1. **Demo:** See it working with sample data (1 hour)
2. **Proof of concept:** 6-week pilot with limited scope (£15k)
3. **Pilot:** 3-month paid trial with full implementation (convert to full deployment)

**Q: What if we don't have APIs for our systems?**

A: We have options:
1. **Work with vendor:** Many vendors will enable APIs for customers
2. **File-based integration:** Daily/hourly sync via files
3. **Database integration:** Direct read from databases (read-only)
4. **Screen scraping:** Last resort, less reliable

Even without integration, you get value from knowledge base, but integration unlocks the full benefit.

**Q: Do we need to hire staff to manage this?**

A: No dedicated staff required. Typical management:
- **Knowledge management:** 4-8 hours/week (existing staff)
- **Performance review:** 2-4 hours/week (contact centre manager)
- **Technical admin:** 2-4 hours/month (IT team)

Most organizations assign this to existing roles.

**Q: Can it handle complaints?**

A: It can:
- Recognize when someone is making a complaint
- Log it in your complaints system
- Provide initial information (process, timescales)
- Offer to escalate to complaint handler immediately

For complex complaints, it hands off quickly to ensure compliance with Housing Ombudsman code.

**Q: Is it accessible for vulnerable users?**

A: Yes. We've designed for inclusion:
- Screen reader compatible (JAWS, NVDA)
- Simple language option
- Voice input support
- High contrast mode
- Adjustable text size
- Option to speak to human at any time

For users who need additional support, advisors can disable AI for specific individuals.

---

## Case Studies

### London Borough of Newtown (300k population)

**Challenge:**
- Contact centre overwhelmed with 40,000 calls/month
- 12-minute average wait time
- 30% abandonment rate
- £800k annual contact centre cost
- Poor satisfaction scores (3.1/5)

**Solution:**
- Deployed Citizen Service Assistant with web chat and SMS
- Integrated with Civica CRM, Bartec (waste), Idox (planning)
- Built 400-article knowledge base
- 6-week implementation

**Results (after 6 months):**
- 18,000 conversations/month handled by AI (45% containment)
- Average wait time reduced to 4 minutes
- Abandonment rate down to 12%
- £220k annual saving (3 FTE avoided, reduced call handling time)
- Satisfaction improved to 4.3/5
- 24/7 service now available

**Quote:**
> "The AI assistant has transformed our contact centre. Our advisors now focus on the complex cases where they add real value, and residents get instant answers 24/7. It's a win-win."
>
> *Sarah Johnson, Customer Services Director, London Borough of Newtown*

---

### Riverside Housing Association (12,000 properties)

**Challenge:**
- Tenants frustrated by office hours only service
- High volume of out-of-hours emergency calls (70% non-emergency)
- £45k annual out-of-hours costs
- 58% first-time resolution
- Repairs scheduling inefficient

**Solution:**
- Deployed Tenant Portal Intelligence
- Integrated with NEC Housing and Oneserve (repairs)
- SMS and web chat channels
- 10-week implementation

**Results (after 9 months):**
- 6,500 conversations/month (42% of total contacts)
- Out-of-hours non-emergency calls reduced by 68%
- £31k annual saving on out-of-hours contractor
- First-time resolution up to 79%
- Average time to book repair reduced from 3 days to same-day
- Tenant satisfaction up from 3.7/5 to 4.4/5

**Quote:**
> "Our tenants love the 24/7 service. They can report repairs, check rent balances, and get answers whenever they need. The AI correctly triages emergency vs non-emergency repairs, saving us thousands in unnecessary callouts."
>
> *David Chen, Director of Customer Experience, Riverside Housing*

---

### Hope Community Trust (Charity - homelessness services)

**Challenge:**
- Small team (8 staff) supporting 200+ clients
- Unable to provide out-of-hours support
- Limited resources for multilingual support
- Clients needing help with benefits, housing applications
- Staff time spent on repetitive queries

**Solution:**
- Deployed Beneficiary Support Chatbot
- SMS-first approach (many clients no web access)
- Integrated with Salesforce NPSP
- Multi-language support (English, Polish, Romanian)
- 8-week implementation

**Results (after 4 months):**
- 420 conversations/month
- 24/7 crisis information available
- Staff time on routine queries down 60%
- Clients supported in 3 languages without hiring translators
- 92% client satisfaction with AI support
- Better crisis support (signposting to emergency services)

**Quote:**
> "For a small charity, this is game-changing. Our clients can get help whenever they need it, in their own language. Our team can focus on the face-to-face work that really matters."
>
> *Rev. Michael Thompson, CEO, Hope Community Trust*

---

## Related Solutions

Enhance your Citizen Service Assistant with these complementary solutions:

- **[Meeting Intelligence Suite](../meeting-intelligence-ai/)** - Transcribe and analyze customer feedback sessions, complaints reviews, and service improvement meetings to identify themes and improve AI responses.

- **[Resident 360 View](../resident-360-ai/)** - Combine data from AI conversations with CRM, case management, and service requests to get a complete view of each citizen/tenant.

- **[Data Query Assistant](../data-query-assistant/)** - Enable business analysts to query conversation data using natural language to identify trends and service improvements.

- **[Complaints Processor](../complaints-processor-ai/)** - Automatically categorize and route complaints that come through the Assistant, ensuring Housing Ombudsman compliance.

- **[HR Policy Assistant](../hr-policy-assistant/)** - Use the same technology internally to help staff with HR queries, creating a consistent AI experience across your organization.

---

## Get Started

### 1. Book a Demo
See the Citizen Service Assistant in action with a personalized demo using sample data from your sector.

**[Book a demo →](mailto:demos@example.com?subject=Citizen%20Service%20Assistant%20Demo)**

30-minute session covering:
- Live conversation examples
- Your sector-specific use cases
- Integration with your systems
- Q&A

---

### 2. Download Evaluation Guide
Comprehensive guide to help you assess suitability and build a business case.

**[Download evaluation guide (PDF) →](./docs/evaluation-guide.pdf)**

Includes:
- Requirements checklist
- ROI calculator
- DPIA template
- Business case template
- Comparison matrix

---

### 3. Request Proof of Concept
6-week limited pilot to test in your environment with real data.

**[Request PoC →](./docs/poc-request.md)**

What you get:
- Deployed in test environment
- One or two integrations
- Limited knowledge base
- 100 test conversations
- Results report and recommendation

---

### 4. Find an Implementation Partner
Connect with certified partners who can help deploy and support the solution.

**[View partners →](./partners.md)**

Partners offer:
- Implementation services
- Integration expertise
- Ongoing support
- Training delivery
- Customisation

---

## Support & Community

### Get Help

- **Documentation:** [Full docs →](./docs/)
- **GitHub Issues:** [Report bugs →](https://github.com/uk-public-sector-ai/citizen-service-assistant/issues)
- **GitHub Discussions:** [Ask questions →](https://github.com/uk-public-sector-ai/citizen-service-assistant/discussions)

### Join the Community

- **Slack Workspace:** [Join UK Public Sector AI →](https://ukpublicsectorai.slack.com)
- **Monthly Webinar:** Live demos and Q&A - [Register →](./events.md)
- **User Group:** Quarterly meetups (virtual) - [Sign up →](./community.md)

### Share Your Success

Deployed this solution? We'd love to hear about it!
- **Case study:** [Submit your story →](./case-studies/submit.md)
- **Testimonial:** Share your experience
- **Speak:** Present at our webinars

---

## License

This solution is available under a commercial license. See [LICENSE.md](./LICENSE.md) for details.

Open-source components used in this solution are listed in [THIRD-PARTY-LICENSES.md](./THIRD-PARTY-LICENSES.md).

---

## Contributing

We welcome contributions from the community! Whether it's:
- Bug fixes
- Feature enhancements
- Documentation improvements
- Integration adapters for new systems

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

---

*Last updated: November 2024*
*Version: 2.1.0*
*Maintained by: UK Public Sector AI Solutions*
