# Claude AI Toolkit 🚀

**Central hub for AI tools, skills, agents, and MCP servers** — Purpose-built to make Claude Code smarter across all your projects (Hemraj, LeadVault, RxGPT, DIGIX, and more).

This toolkit aggregates **100+ Anthropic skills**, **13 essential open-source tools**, **MCP servers**, and **integration patterns** into one discoverable, deployable ecosystem.

---

## 📋 What's Inside

### [1. Skills Registry](./SKILLS_REGISTRY.md)
**100+ Anthropic AI/ML skills** organized by category:
- **Engineering**: code-review, debug, deploy, testing-strategy, tech-debt
- **Product Management**: brainstorm, metrics-review, roadmap, competitive-brief
- **Marketing**: campaign-plan, content-creation, seo-audit, brand-review
- **Data & Analytics**: analyze, build-dashboard, data-viz, sql-queries
- **Design**: design-critique, ux-copy, accessibility-review, design-system
- **Operations**: runbook, compliance-tracking, capacity-plan, vendor-review
- **Sales & Revenue**: account-research, call-prep, pipeline-review, forecast
- **Finance**: audit-support, reconciliation, variance-analysis, close-management
- **Healthcare** (RxGPT): patient-engagement, clinical-workflows, compliance
- **Agro-Industrial** (Hemraj): demand-forecasting, procurement, pricing, logistics
- **Lead Generation** (LeadVault): prospecting, enrichment, classification, export

➡️ **Use**: `/code-review`, `/debug`, `/brainstorm`, `/seo-audit`, etc. in Claude Code

---

### [2. External Tools Directory](./EXTERNAL_TOOLS.md)
**13 curated open-source projects** to integrate:

| Tool | Purpose | Use Case |
|------|---------|----------|
| **ollama** | Run LLMs locally | On-premise inference for Hemraj agents |
| **Whisper** | Speech-to-text (99 languages) | Call transcription, voice input for RxGPT |
| **claude-ads** | Multi-platform ad management | Meta, Google, LinkedIn, TikTok campaigns |
| **Fooocus** | Image generation (Midjourney alt) | Marketing collateral, product visuals |
| **yt-dlp** | Video downloader | Content harvesting, media processing |
| **Open-Generative-AI** | Open-source AI studio | Unrestricted image/video generation |
| **context-mode** | Context optimization | MCP + hook-based routing (17 platforms) |
| **awesome-mcp-servers** | MCP directory | 90+ servers for Claude integration |
| **awesome-llm-apps** | 100+ AI agents/RAG apps | Patterns for LeadVault, DIGIX agents |
| **public-apis** | 1400+ free APIs | Data integration, webhook sources |
| **AppFlowy** | Open-source Notion | Self-hosted workspace for all projects |
| **Penpot** | Open-source Figma | Design system for DIGIX frontend |
| **Plausible Analytics** | Privacy-first analytics | Replace Google Analytics on all apps |

➡️ **Setup**: See [EXTERNAL_TOOLS.md](./EXTERNAL_TOOLS.md) for Docker/installation guides

---

### [3. Project Integration Map](./PROJECTS.md)
**Your 6 active projects** with recommended tools & skills:

- **Hemraj Group AI Agents** — 13 agents (forecasting, pricing, procurement, logistics)
- **HEMRAJ Finance GCP** — Debtor reporting agents on Cloud Run + Cloud SQL
- **LeadVaultAI** — Lead mining, classification, ICP enrichment
- **DIGIX AI OS** — SDR console, Gmail integration, Instagram analytics
- **RxGPT Healthcare** — Patient engagement, clinical workflows, telemedicine
- **Fractional CMO Tools** — Client discovery, engagement automation

---

### [4. MCP Server Configs](./MCP_SETUP.md)
Ready-to-use Model Context Protocol configurations:
- Gmail, Google Calendar, Slack, Linear, GitHub
- Database connectors (BigQuery, PostgreSQL, MySQL)
- Data tools (Hex, Amplitude, HubSpot)
- Design tools (Figma, Adobe Creative Suite)
- Custom enterprise MCPs

---

### [5. Setup & Deployment Guides](./SETUP_GUIDES/)
- **Local Dev** — Docker Compose for all tools
- **GCP Deployment** — Cloud Run + Cloud SQL + Artifact Registry
- **GitHub Actions** — CI/CD for agents, skills, MCP servers
- **Environment Templates** — `.env.example` for each project

---

## 🎯 Quick Start

### 1. Clone This Toolkit
```bash
git clone https://github.com/saileshpattnaik357/claude-ai-toolkit.git
cd claude-ai-toolkit
```

### 2. Update Your CLAUDE.md Files
This toolkit auto-links to your projects. Update your project CLAUDE.md:

```bash
# Example: digix/CLAUDE.md
# Add this section:

## 🛠 AI Toolkit Integration
- **Skills**: See [claude-ai-toolkit/SKILLS_REGISTRY.md](../claude-ai-toolkit/SKILLS_REGISTRY.md)
- **Tools**: [External Tools](../claude-ai-toolkit/EXTERNAL_TOOLS.md)
- **MCP Servers**: [MCP_SETUP.md](../claude-ai-toolkit/MCP_SETUP.md)
- **Project Map**: [PROJECTS.md](../claude-ai-toolkit/PROJECTS.md)
```

### 3. Enable Skills in Claude Code
Each skill works instantly via `/` commands:
```
/code-review ultra          # Multi-agent code review
/brainstorm                 # Product ideation with research
/seo-audit                  # Full website SEO audit
/design-critique            # Design feedback on files
/debug                      # Interactive debugging
```

### 4. Load MCP Servers
In `~/.claude/settings.json`:
```json
{
  "mcpServers": {
    "gmail": { "command": "mcp" },
    "github": { "command": "mcp" },
    "slack": { "command": "mcp" }
  }
}
```

---

## 📁 Directory Structure

```
claude-ai-toolkit/
├── README.md                          ← You are here
├── SKILLS_REGISTRY.md                 # 100+ Anthropic skills
├── EXTERNAL_TOOLS.md                  # 13 open-source tools
├── PROJECTS.md                        # Your 6 projects + mappings
├── MCP_SETUP.md                       # Model Context Protocol configs
├── CLAUDE_INTEGRATION.md              # How to wire everything together
│
├── tools/
│   ├── llm-models/                    # ollama, Whisper, local inference
│   ├── media-ops/                     # claude-ads, Fooocus, yt-dlp
│   ├── agents/                        # awesome-llm-apps, context-mode
│   ├── design/                        # Penpot, AppFlowy
│   └── utilities/                     # public-apis, Plausible
│
├── integrations/
│   ├── hemraj/                        # Hemraj Group agent configs
│   ├── leadvault/                     # LeadVault setup & classifiers
│   ├── digix/                         # DIGIX SDR + Gmail configs
│   ├── rxgpt/                         # RxGPT clinical workflows
│   └── shared/                        # Common patterns
│
├── setup-guides/
│   ├── docker-compose.yml             # Local dev environment
│   ├── gcp-deployment.md              # Cloud Run + Cloud SQL
│   ├── github-actions.yml             # CI/CD workflows
│   └── env-templates/                 # .env.example files
│
└── CONTRIBUTE.md                      # How to add new tools
```

---

## 🔗 Quick Links

| Resource | Purpose |
|----------|---------|
| [Anthropic Skills Docs](https://github.com/anthropics/skills) | Official skill repository |
| [Claude Code Docs](https://docs.anthropic.com/claude-code) | CLI reference |
| [MCP Registry](https://modelcontextprotocol.io) | MCP server directory |
| [Your Projects](./PROJECTS.md) | All 6 projects integrated |

---

## 🚀 What You Can Do Now

✅ **Run any Anthropic skill** → `/code-review`, `/brainstorm`, `/seo-audit`  
✅ **Access 100+ MCP servers** → Gmail, GitHub, Slack, databases, design tools  
✅ **Deploy agents** → Hemraj (GCP), LeadVault, DIGIX, RxGPT  
✅ **Use open-source alternatives** → Penpot, AppFlowy, Plausible, ollama  
✅ **Integrate multi-platform tools** → claude-ads (12 ad platforms), Whisper, Fooocus  

---

## 📞 Support

- Issues? → Check [TROUBLESHOOTING.md](./TROUBLESHOOTING.md)
- Adding a tool? → See [CONTRIBUTE.md](./CONTRIBUTE.md)
- Need MCP help? → [MCP_SETUP.md](./MCP_SETUP.md)

---

**Last Updated**: 2026-08-28  
**Maintainer**: [@saileshpattnaik357](https://github.com/saileshpattnaik357)  
**License**: MIT
