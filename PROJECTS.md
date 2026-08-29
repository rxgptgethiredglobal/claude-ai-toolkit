# Project Integration Map 🗺️

**Your 6 active projects** with recommended skills, tools, and MCP servers.

---

## 1. Hemraj Group AI Agents 🌾

**13 AI agents** for agro-industrial operations: demand forecasting, pricing, procurement, sales, logistics, quality, market intelligence.

### Recommended Skills
```
/code-review /data:analyze /data:sql-queries /data:statistical-analysis
/sales:account-research /operations:process-optimization /engineering:system-design
/marketing:competitive-brief /data:build-dashboard /engineering:deploy-checklist
/finance:audit-support /product-management:metrics-review
```

### Essential Tools
- **Semantica** ⭐ — Trace every pricing/procurement decision
- **Decision Tracing** ⭐ — Audit trail for compliance
- **context-mode** — Keep 13 agents focused
- **Ollama** — Local LLM inference for cost reduction
- **public-apis** — Weather, commodity prices, market data
- **AppFlowy** — Agent operation logs & dashboards
- **Plausible** — Farm/supply analytics

### MCP Servers
```
- BigQuery (forecast results)
- Google Sheets (pricing tables)
- Slack (agent alerts)
- GitHub (agent code)
- PostgreSQL (operational DB)
```

### Directory Structure
```
CLAUDE.md (updated with toolkit links)
├── integrations/hemraj/
│   ├── demand-forecast-agent.md
│   ├── pricing-optimization-agent.md
│   ├── procurement-agent.md
│   └── semantica-config.yml
└── setup-guides/
    └── hemraj-gcp-setup.md
```

---

## 2. HEMRAJ Finance GCP Deployment 💰

**Debtor Reporting Agent system** (7 agents) deploying to GCP: Cloud Run, Cloud SQL, Artifact Registry.

### Recommended Skills
```
/finance:audit-support /finance:close-management /finance:reconciliation
/finance:financial-statements /data:build-dashboard /engineering:deploy-checklist
/engineering:architecture /operations:compliance-tracking
```

### Essential Tools
- **Semantica** — Decision audit for financial transactions
- **context-mode** — GCP-optimized prompts
- **AppFlowy** — Finance dashboards
- **Plausible** — Debtor portal analytics

### MCP Servers
```
- Google Cloud (Cloud Run, Cloud SQL)
- BigQuery (financial reporting)
- GitHub (CI/CD)
- Slack (deployment alerts)
```

### CLAUDE.md Updates
```markdown
## Finance Platform Integration

### Skills
/finance:audit-support /finance:close-management /finance:reconciliation

### Tools
- Semantica (decision tracing)
- Cloud Run/SQL (GCP)
- BigQuery (reporting)

### Reference
See ../claude-ai-toolkit/PROJECTS.md
```

---

## 3. LeadVaultAI 🎯

**Standalone lead-mining app** with client ICP upload, mining brain generation, classification, export.

### Recommended Skills
```
/sales:draft-outreach /sales:account-research /data:explore-data
/product-management:brainstorm /searchfit-seo:keyword-clustering
/marketing:content-creation /data:analyze /sales:call-prep
```

### Essential Tools
- **semantica** ⭐ — Why did classifier score this lead 0.87?
- **claude-ads** — Lead nurture campaign automation
- **Fooocus** — LinkedIn profile picture generation
- **public-apis** — Company/person data enrichment
- **AppFlowy** — Lead research notes
- **Plausible** — User funnel analytics

### MCP Servers
```
- PostgreSQL (lead database)
- GitHub (classifier code)
- Slack (lead alerts)
- Gmail (outreach tracking)
```

### Key Workflows
1. **Mining**: Pull raw leads via APIs
2. **Enrichment**: 1400+ public APIs for data
3. **Classification**: ML classifier (trace with Semantica)
4. **Nurture**: claude-ads multi-platform campaigns
5. **Export**: Bulk leads to sales CRM

### CLAUDE.md Updates
```markdown
## LeadVault AI Integration

### Decision Tracing
All lead classification decisions logged in Semantica:
`semantica trace --query "Why was this lead scored 0.87?"`

### Tools
- Semantica (classifier auditing)
- claude-ads (campaign automation)
- Fooocus (profile generation)

### Reference
../claude-ai-toolkit/PROJECTS.md
```

---

## 4. DIGIX AI Operating System 🤖

**AI revenue OS** with SDR console, Gmail integration, Instagram analytics, campaign management.

### Recommended Skills
```
/sales:call-prep /sales:daily-briefing /marketing:campaign-plan
/adspirer-ads-agent:performance-review /design:design-critique
/marketing:content-creation /brand-voice:enforce-voice
/engineering:deploy-checklist /product-management:metrics-review
```

### Essential Tools
- **claude-ads** ⭐ — 12-platform campaign management
- **Whisper** ⭐ — Call transcription for SDR console
- **Fooocus** — Ad creative generation
- **Penpot** — SDR UI/UX design
- **AppFlowy** — SDR playbooks & docs
- **Plausible** — Campaign analytics
- **Semantica** — SDR decision logging

### MCP Servers
```
- Gmail (email integration)
- Instagram (analytics)
- GitHub (SDR code)
- Slack (team updates)
- Linear (task tracking)
```

### Key Workflows
1. **SDR Console**: Daily lead list + call script
2. **Multi-Platform Ads**: Google, Meta, LinkedIn, TikTok
3. **Call Transcription**: Whisper → email summary
4. **Campaign Analytics**: Plausible dashboards
5. **Creative Generation**: Fooocus for ad variants

---

## 5. RxGPT Healthcare Platform 🏥

**Healthcare AI platform** with Docker Compose, PostgreSQL, FastAPI backend, Node.js frontend.

### Recommended Skills
```
/operations:compliance-tracking /data:build-dashboard /design:user-research
/product-management:metrics-review /sales:call-summary
/engineering:deploy-checklist /engineering:testing-strategy
```

### Essential Tools
- **Whisper** ⭐ — Patient call transcription (HIPAA-safe local)
- **Ollama** — Local LLM for patient data (no cloud exposure)
- **Semantica** — Clinical decision logging
- **AppFlowy** — Medical workflows
- **Plausible** — GDPR-compliant patient portal analytics

### MCP Servers
```
- PostgreSQL (patient DB)
- GitHub (code)
- Slack (clinical alerts)
```

### HIPAA Considerations
- Use Ollama for local inference (no cloud data)
- Whisper runs locally (no audio to cloud)
- Plausible (privacy-first, no cookies)
- Semantica (audit trail required)

---

## 6. Fractional CMO Tools 📊

**Interactive HTML diagnostic** for consulting discovery, client engagement, friction assessment.

### Recommended Skills
```
/brand-voice:generate-guidelines /brand-voice:discover-brand
/marketing:campaign-plan /searchfit-seo:content-strategy
/design:design-system /marketing:content-creation
/product-management:brainstorm
```

### Essential Tools
- **Penpot** — Visual identity creation
- **AppFlowy** — Client research notes
- **Fooocus** — Brand asset generation
- **claude-ads** — Campaign templates
- **Plausible** — Tool analytics (who uses it)

### Tool Usage
```markdown
## Fractional CMO Integration

Diagnostic Tool Features:
- Brand Discovery Quiz → /brand-voice:discover-brand
- Content Gap Analysis → /searchfit-seo:content-strategy
- Asset Generator → Fooocus integration
- Design System → Penpot export

Reference: ../claude-ai-toolkit/PROJECTS.md
```

---

## 📊 Skills by Project

| Skill | Hemraj | HEMRAJ Finance | LeadVault | DIGIX | RxGPT | fractional-cmo |
|-------|--------|---|-----------|-------|-------|---|
| code-review | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| data:analyze | ✅ | ✅ | ✅ | ⚠️ | ✅ | ⚠️ |
| sales:draft-outreach | ⚠️ | ⚠️ | ✅ | ✅ | ⚠️ | ⚠️ |
| finance:* | ⚠️ | ✅ | ⚠️ | ⚠️ | ⚠️ | ⚠️ |
| marketing:* | ✅ | ⚠️ | ✅ | ✅ | ⚠️ | ✅ |
| design:* | ⚠️ | ⚠️ | ⚠️ | ✅ | ⚠️ | ✅ |
| operations:* | ✅ | ✅ | ⚠️ | ✅ | ✅ | ⚠️ |
| brand-voice:* | ⚠️ | ⚠️ | ⚠️ | ✅ | ⚠️ | ✅ |

Legend: ✅ = Core, ⚠️ = Useful, ⚪ = Optional

---

## 🔧 Tools by Project

| Tool | Hemraj | HEMRAJ Finance | LeadVault | DIGIX | RxGPT | fractional-cmo |
|------|--------|---|-----------|-------|-------|---|
| Semantica | ⭐⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐ | ⚪ |
| Decision Tracing | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐ | ⚪ |
| context-mode | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Ollama | ⭐⭐ | ⚪ | ⚪ | ⚪ | ⭐⭐⭐ | ⚪ |
| Whisper | ⭐⭐ | ⚪ | ⚪ | ⭐⭐⭐ | ⭐⭐⭐ | ⚪ |
| claude-ads | ⚪ | ⚪ | ⭐⭐⭐ | ⭐⭐⭐ | ⚪ | ⭐⭐⭐ |
| Fooocus | ⭐ | ⚪ | ⭐⭐ | ⭐⭐⭐ | ⚪ | ⭐⭐⭐ |
| AppFlowy | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Penpot | ⚪ | ⚪ | ⚪ | ⭐⭐⭐ | ⚪ | ⭐⭐⭐ |
| Plausible | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |

Legend: ⭐⭐⭐ = Critical, ✅ = Essential, ⚪ = Optional

---

## 📍 Quick Navigation

### By Project
- [Hemraj Group AI Agents](#1-hemraj-group-ai-agents-)
- [HEMRAJ Finance GCP](#2-hemraj-finance-gcp-deployment-)
- [LeadVaultAI](#3-leadvaultai-)
- [DIGIX AI OS](#4-digix-ai-operating-system-)
- [RxGPT Healthcare](#5-rxgpt-healthcare-platform-)
- [Fractional CMO](#6-fractional-cmo-tools-)

### By Tool Category
- [AI Infrastructure](#-ai-agent-infrastructure)
- [LLM Models](#-llm--model-infrastructure)
- [Advertising](#-multi-platform-advertising)
- [Media Generation](#-media-generation)
- [Design Tools](#%EF%B8%8F-design--workspace-tools)

---

## 🚀 Next Steps

1. **Read**: `SKILLS_REGISTRY.md` — All 100+ skills
2. **Read**: `EXTERNAL_TOOLS.md` — Tool setup guides
3. **Do**: Update each project's CLAUDE.md (see examples above)
4. **Do**: Run Docker Compose to deploy core tools
5. **Do**: Wire up MCP servers for your stack

**Total implementation time**: ~2 weeks (phased)

---

**Last Updated**: 2026-08-28  
**Maintainer**: [@saileshpattnaik357](https://github.com/saileshpattnaik357)
