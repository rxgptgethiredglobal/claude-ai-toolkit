# CLAUDE.md Template for Projects

**Copy and customize this template** for each of your projects.

---

## Template: CLAUDE.md (Updated)

```markdown
# Project Name CLAUDE Configuration

## Quick Links
- 🛠 **Claude AI Toolkit**: [../claude-ai-toolkit](../claude-ai-toolkit)
- 📚 **Skills Registry**: [../claude-ai-toolkit/SKILLS_REGISTRY.md](../claude-ai-toolkit/SKILLS_REGISTRY.md)
- 🔧 **External Tools**: [../claude-ai-toolkit/EXTERNAL_TOOLS.md](../claude-ai-toolkit/EXTERNAL_TOOLS.md)
- 🗺️ **Project Map**: [../claude-ai-toolkit/PROJECTS.md](../claude-ai-toolkit/PROJECTS.md)

---

## 🎯 AI Skills for This Project

### Recommended Skills
Use these /commands in Claude Code for this project:

```bash
# Example for Hemraj:
/code-review              # Multi-level code analysis
/data:analyze             # Data processing
/engineering:system-design # Architecture reviews
/data:build-dashboard      # Analytics
```

👉 **Full list**: See [../claude-ai-toolkit/SKILLS_REGISTRY.md](../claude-ai-toolkit/SKILLS_REGISTRY.md)

---

## 🛠 External Tools

### Priority Tools (This Project)
- **Tool Name** — What it does ([Setup Guide](../claude-ai-toolkit/EXTERNAL_TOOLS.md#tool-name))
- **Tool Name** — What it does

### Full Directory
👉 See [../claude-ai-toolkit/EXTERNAL_TOOLS.md](../claude-ai-toolkit/EXTERNAL_TOOLS.md)

---

## 🔌 MCP Server Configs

These are already configured in `~/.claude/settings.json`:

```json
{
  "mcpServers": {
    "github": { "command": "mcp" },
    "slack": { "command": "mcp" }
  }
}
```

👉 **Full MCP setup**: See [../claude-ai-toolkit/MCP_SETUP.md](../claude-ai-toolkit/MCP_SETUP.md)

---

## 🚀 How Claude Gets Smarter

1. **Skills** — 100+ built-in AI/ML skills (via / commands)
2. **External Tools** — 15 open-source apps (Semantica, AppFlowy, etc.)
3. **MCP Servers** — Your entire stack wired to Claude (Gmail, GitHub, Slack, databases)
4. **Decision Tracing** — Every agent decision auditable (Hemraj, LeadVault, DIGIX)

---

## 📖 Documentation

See the toolkit README for comprehensive guides:
- [claude-ai-toolkit/README.md](../claude-ai-toolkit/README.md)

---

## ✅ Project-Specific Setup

[Your custom setup instructions here]

---

```

---

## Per-Project CLAUDE.md Updates

### 1. Hemraj Group AI Agents

```markdown
# CLAUDE Configuration — Hemraj Group AI Agents

## Essential Skills
```bash
/code-review              # Agent code quality
/data:analyze             # Forecast analysis
/data:build-dashboard     # Agent dashboards
/operations:runbook       # Agent procedures
/engineering:system-design # Agent architecture
```

## Critical Tools
- **Semantica** — Trace pricing/procurement decisions
- **Decision Tracing** — Full audit trail (compliance)
- **context-mode** — Keep 13 agents focused
- **Ollama** — Local LLM inference (cost reduction)
- **AppFlowy** — Operation logs & monitoring

## MCP Servers
- PostgreSQL (operational DB)
- BigQuery (forecasts)
- GitHub (agent code)
- Slack (alerts)

## Key Workflows
- Demand Forecasting Agent
- Pricing Optimization Agent
- Procurement Agent
- Logistics Agent
- Quality Control Agent
- Market Intelligence Agent

[Link to toolkit] ../claude-ai-toolkit/PROJECTS.md#1-hemraj-group-ai-agents
```

### 2. HEMRAJ Finance GCP

```markdown
# CLAUDE Configuration — HEMRAJ Finance GCP

## Essential Skills
```bash
/finance:audit-support
/finance:close-management
/finance:reconciliation
/engineering:deploy-checklist
/operations:compliance-tracking
```

## Critical Tools
- **Semantica** — Financial decision tracing
- **AppFlowy** — Finance dashboards
- **Plausible** — Debtor portal analytics

## GCP Services
- Cloud Run (debtor agents)
- Cloud SQL (transaction DB)
- Artifact Registry (agent images)
- BigQuery (reporting)

[Link to toolkit] ../claude-ai-toolkit/PROJECTS.md#2-hemraj-finance-gcp-deployment
```

### 3. LeadVaultAI

```markdown
# CLAUDE Configuration — LeadVaultAI

## Essential Skills
```bash
/sales:draft-outreach
/sales:account-research
/data:explore-data
/product-management:brainstorm
/searchfit-seo:keyword-clustering
```

## Critical Tools
- **Semantica** — Classifier decision auditing
- **claude-ads** — Multi-platform nurture campaigns
- **Fooocus** — Profile image generation
- **public-apis** — Data enrichment (1400+ APIs)
- **AppFlowy** — Research notes

## Key Workflows
1. Lead Mining (raw data)
2. Enrichment (APIs)
3. Classification (Semantica traces)
4. Nurture (claude-ads campaigns)
5. Export (bulk to CRM)

[Link to toolkit] ../claude-ai-toolkit/PROJECTS.md#3-leadvaultai
```

### 4. DIGIX AI Operating System

```markdown
# CLAUDE Configuration — DIGIX

## Essential Skills
```bash
/sales:call-prep
/sales:daily-briefing
/marketing:campaign-plan
/adspirer-ads-agent:performance-review
/design:design-critique
```

## Critical Tools
- **claude-ads** — 12-platform campaign management
- **Whisper** — Call transcription for SDR
- **Fooocus** — Ad creative generation
- **Penpot** — UI/UX design
- **Plausible** — Campaign analytics

## SDR Console Features
- Daily lead routing
- Call script generation
- Transcription & summary
- Multi-platform ads
- Performance dashboards

[Link to toolkit] ../claude-ai-toolkit/PROJECTS.md#4-digix-ai-operating-system
```

### 5. RxGPT Healthcare

```markdown
# CLAUDE Configuration — RxGPT

## Essential Skills
```bash
/operations:compliance-tracking  # HIPAA audit
/data:build-dashboard            # Patient dashboards
/design:user-research            # Patient UX
/engineering:testing-strategy    # Clinical reliability
```

## Critical Tools
- **Whisper** — Local call transcription (HIPAA)
- **Ollama** — Local inference (no cloud data)
- **Semantica** — Clinical decision logging
- **AppFlowy** — Medical workflows
- **Plausible** — GDPR-compliant analytics

## HIPAA Compliance
- All processing local (Whisper, Ollama)
- Audit trail in Semantica
- Privacy-first analytics (Plausible)
- No cloud data exposure

[Link to toolkit] ../claude-ai-toolkit/PROJECTS.md#5-rxgpt-healthcare-platform
```

### 6. Fractional CMO Tools

```markdown
# CLAUDE Configuration — Fractional CMO Tools

## Essential Skills
```bash
/brand-voice:generate-guidelines
/marketing:campaign-plan
/searchfit-seo:content-strategy
/design:design-system
/marketing:content-creation
```

## Critical Tools
- **Penpot** — Visual identity creation
- **Fooocus** — Brand asset generation
- **AppFlowy** — Client research
- **claude-ads** — Campaign templates
- **Plausible** — Tool usage analytics

## Diagnostic Features
- Brand Discovery Quiz
- Content Gap Analysis
- Asset Generator
- Design System Export

[Link to toolkit] ../claude-ai-toolkit/PROJECTS.md#6-fractional-cmo-tools
```

---

## 📋 Checklist: Update All CLAUDE.md Files

- [ ] Copy template to `digix/CLAUDE.md`
- [ ] Copy template to `leadvault/CLAUDE.md`
- [ ] Copy template to `RxGPT/frontend/CLAUDE.md`
- [ ] Copy template to `fractional-cmo-tools/CLAUDE.md`
- [ ] Create `hemraj/CLAUDE.md` with agent-specific section
- [ ] Create `hemraj/finance/CLAUDE.md` with finance section
- [ ] Commit & push all updates
- [ ] Test `/code-review` in each project

---

## Next Step

1. Customize template above for each project
2. Replace relative paths with your actual project paths
3. Add project-specific setup instructions
4. Run: `git add CLAUDE.md && git commit -m "Add Claude AI Toolkit integration"`

---
