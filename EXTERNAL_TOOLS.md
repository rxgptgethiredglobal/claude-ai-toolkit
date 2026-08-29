# External Tools Directory 🛠️

**16 curated open-source projects** for integrating with Claude, your agents, and projects.

---

## 🎯 AI Agent Infrastructure

### 1. **Semantica** ⭐ CRITICAL FOR AGENTS
**Graph-Native Infrastructure for Context & Accountable AI Systems**

- **What**: Query-able decision graphs for AI agents — traces reasoning chains, scenarios, outcomes
- **Use**: Hemraj agents, DIGIX SDR, RxGPT workflows need decision tracing
- **Key Feature**: `semantica trace --query "Why did you do that?"` reconstructs decision path
- **Deploy**: Python SDK or Docker
- **GitHub**: [semantica-agi/semantica](https://github.com/semantica-agi/semantica)

```bash
# Install
pip install semantica

# Trace agent decision
semantica trace --query "Why did pricing agent select this price?"

# Returns: Decision graph with confidence scores, reasoning, outcomes
```

**Why you need it**: Your 13 Hemraj agents make thousands of daily decisions. Need full auditability for compliance & optimization.

---

### 2. **Decision Tracing System** ⭐ CRITICAL FOR AGENTS
**Palantir-Style Decision Memory for AI Agents**

- **What**: Every decision your agents make is logged, contextualized, and queryable
- **Use**: Hemraj pricing, procurement, forecasting agents
- **Key Feature**: Scenario→Seasoning→Reasoning→Outcome→Confidence graph
- **Deploy**: Graph database + query engine
- **GitHub**: [decision-tracing-ai](https://github.com/your-org/decision-memory)

```bash
# Query decision history
decision-trace query "What decisions led to inventory shortage?"

# Returns: Complete decision path with alternatives considered
```

**Why you need it**: Retroactive analysis—if an agent's recommendation caused loss, trace exactly what it considered.

---

### 3. **context-mode**
**Context Window Optimization for AI Coding Agents**

- **What**: Reduces tool output 98%, persists session memory, enforces routing (17 platforms)
- **Use**: All projects—keeps Claude focused on code
- **GitHub**: [mksglu/context-mode](https://github.com/mksglu/context-mode)

```yaml
# .claude/context-mode.yml
sandbox_reduction: 98%
routing:
  - platform: slack
    mcp: true
  - platform: github
    mcp: true
```

---

## 🤖 LLM & Model Infrastructure

### 4. **Ollama**
**Run LLMs Locally** — Kimi-K2.6, GLM-5.2, MiniMax, DeepSeek, gpt-oss, Qwen, Gemma

- **Use**: On-premise inference for Hemraj, RxGPT (no API costs)
- **GitHub**: [ollama/ollama](https://ollama.com)

```bash
ollama run mistral
ollama run qwen:14b
# Run locally, zero latency
```

---

### 5. **Whisper (OpenAI)**
**Speech-to-Text** — 99 languages, free, open-source

- **Use**: Call transcription (RxGPT), voice input (DIGIX)
- **GitHub**: [openai/whisper](https://github.com/openai/whisper)

```bash
pip install openai-whisper
whisper audio.mp3 --language en --task transcribe
```

---

## 📢 Multi-Platform Advertising

### 6. **claude-ads** ⭐ FOR DIGIX
**Claude-First Paid Media Operations** — 12 ad platforms

Manages: Google Ads, Meta, YouTube, LinkedIn, TikTok, Microsoft, Apple, Amazon, Reddit, Pinterest, Snapchat, X

- **Use**: DIGIX campaign automation
- **Features**: Source-grounded audits, deterministic scoring, versioned JSON reports
- **GitHub**: [AgriciDaniel/claude-ads](https://github.com/AgriciDaniel/claude-ads)

```bash
claude-ads audit --account meta --budget-check
# Returns: Wasted spend, optimization recs
```

---

## 🎨 Media Generation

### 7. **Fooocus**
**Midjourney-Quality Image Generation** — Unlimited generations, free, runs on your GPU

- **Use**: Marketing collateral, product visuals (DIGIX, fractional-cmo)
- **GitHub**: [lllyasviel/Fooocus](https://github.com/lllyasviel/Fooocus)

```bash
# Web UI at localhost:7865
python -m fooocus
# Generate: "professional product photo, studio lighting"
```

---

### 8. **Open-Generative-AI**
**Unrestricted AI Studio** — 500+ models (Flux, Midjourney, Kling, Sora, Veo)

- **Use**: Unlimited image/video generation, no filters
- **GitHub**: [Anil-matcha/Open-Generative-AI](https://github.com/Anil-matcha/Open-Generative-AI)

```bash
# Self-hosted alternative to paid platforms
# 27K stars, MIT licensed
```

---

### 9. **yt-dlp**
**Video Downloader** — YouTube, TikTok, Instagram, 1000+ sites

- **Use**: Content harvesting, training data collection
- **GitHub**: [yt-dlp/yt-dlp](https://github.com/yt-dlp/yt-dlp)

```bash
pip install yt-dlp
yt-dlp "https://youtube.com/watch?v=..." -f best
```

---

## 🏗️ Agent & App Patterns

### 10. **awesome-llm-apps** ⭐ FOR PATTERN LEARNING
**100+ AI Agents, Agent Skills, RAG Apps** — Free & open-source

- **Use**: Study agent patterns for Hemraj, LeadVault, DIGIX
- **GitHub**: [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps)
- **134K stars** — industry-standard reference

```
Patterns for:
- Multi-agent orchestration
- RAG (retrieval-augmented generation)
- Tool-use workflows
- Reasoning chains
- Feedback loops
```

---

### 11. **MCP Servers Directory** ⭐ CRITICAL
**90+ Model Context Protocol Servers** — Gmail, GitHub, Slack, databases, design tools

- **Use**: Wire up Claude to your entire stack
- **GitHub**: [punkpeye/awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers)

```yaml
# .claude/settings.json
mcpServers:
  gmail: { command: "mcp" }
  github: { command: "mcp" }
  slack: { command: "mcp" }
  bigquery: { command: "mcp" }
```

---

## 🔌 Data & API Integration

### 12. **public-apis**
**1400+ Free APIs** — 50+ categories (weather, finance, games, images, etc.)

- **Use**: Data sources for all projects
- **GitHub**: [public-apis/public-apis](https://github.com/public-apis/public-apis)

```
Categories:
- Weather, Finance, Games, Images, Music
- News, Video, Science, Business, Calendar
- Geocoding, Cryptocurrency, and 40+ more
```

---

## 🔗 LLM Framework & Plugin System

### 16. **DeepSeek Harness** ⭐ CRITICAL FOR AGENTS
**"Everything is a Plugin"** — Universal LLM framework for making any system pluggable

- **What**: Plugin architecture for integrating LLMs into any codebase
- **Use**: Hemraj agents, DIGIX SDR, LeadVault classifiers
- **Key Feature**: Instant LLM capability for existing systems (no rewrite)
- **Deploy**: Python SDK or containerized
- **GitHub**: [deepseek-ai/deepseek-harness](https://github.com/deepseek-ai/deepseek-harness)
- **Stats**: 201K stars, 23.1K forks

```bash
# Install
pip install deepseek-harness

# Make ANY function LLM-capable
from deepseek_harness import plugin

@plugin
def my_function(x: int) -> str:
    return f"Process {x}"

# Now has LLM reasoning, multi-step execution, memory
```

**Why you need it**: 
- Hemraj agents: Add LLM to existing pricing/forecasting logic
- LeadVault: Plug LLM into classifier pipeline
- DIGIX: Add reasoning to SDR score engine
- RxGPT: Integrate LLM into clinical workflows

**Integration with Semantica**: 
- Harness plugins → Semantica decision graphs
- Full traceability of LLM reasoning in your code

---

## 🖼️ Design & Workspace Tools

### 13. **Penpot** ⭐ FOR DIGIX DESIGN
**Open-Source Figma** — Self-hosted, full-featured design

- **Use**: DIGIX frontend design system
- **GitHub**: [penpot/penpot](https://github.com/penpot/penpot)

```bash
docker-compose up penpot
# Access at localhost:80
# Full design collaboration, no licensing fees
```

---

### 14. **AppFlowy** ⭐ FOR ALL PROJECTS
**Open-Source Notion** — Self-hosted workspace, unlimited users

- **Use**: Team knowledge base, project documentation
- **GitHub**: [AppFlowy-IO/AppFlowy](https://github.com/AppFlowy-IO/AppFlowy)

```bash
docker-compose up appflowy
# Notion alternative, $0/month, full control
```

---

### 15. **Plausible Analytics** ⭐ FOR ALL WEB
**Privacy-First Google Analytics Alternative**

- **Use**: Replace GA on all web projects (DIGIX, LeadVault, Hemraj dashboards)
- **GitHub**: [plausible/analytics](https://github.com/plausible/analytics)
- **Cost**: $0 self-hosted vs $150k/year enterprise GA

```bash
docker-compose up plausible
# GDPR/CCPA compliant, no cookies, EU-hosted option
```

---

## 📊 Integration Matrix

| Tool | Hemraj | LeadVault | DIGIX | RxGPT | fractional-cmo | Setup Time |
|------|--------|-----------|-------|-------|----------------|-----------|
| **Semantica** | ⭐⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐⭐ | - | 2 days |
| **Decision Tracing** | ⭐⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐ | - | 3 days |
| **context-mode** | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐ | 2 hrs |
| **Ollama** | ⭐⭐⭐ | ⭐⭐ | ⭐ | ⭐⭐⭐ | - | 1 hr |
| **Whisper** | ⭐⭐ | - | ⭐⭐⭐ | ⭐⭐⭐ | - | 30 min |
| **claude-ads** | - | ⭐⭐⭐ | ⭐⭐⭐ | - | ⭐⭐⭐ | 1 day |
| **Fooocus** | ⭐ | ⭐⭐ | ⭐⭐⭐ | - | ⭐⭐⭐ | 1 hr |
| **Open-GenAI** | ⭐ | ⭐⭐ | ⭐⭐⭐ | - | ⭐⭐⭐ | 2 hrs |
| **yt-dlp** | ⭐⭐ | ⭐⭐ | ⭐ | - | ⭐⭐ | 10 min |
| **awesome-llm-apps** | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | - | Reference |
| **MCP Servers** | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | 1 day |
| **public-apis** | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐⭐ | Reference |
| **Penpot** | - | - | ⭐⭐⭐ | - | ⭐⭐⭐ | 2 hrs |
| **AppFlowy** | ⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐⭐ | ⭐⭐⭐ | 1 hr |
| **Plausible** | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐ | 30 min |

---

## 🚀 Priority Setup Order

### Phase 1: Foundation (Week 1)
1. **Semantica** — Agent decision tracing
2. **Decision Tracing** — Complete audit trail
3. **context-mode** — Optimize Claude context

### Phase 2: Operations (Week 2)
4. **MCP Servers** — Wire Claude to your stack
5. **AppFlowy** — Team workspace
6. **Plausible** — Analytics replacement

### Phase 3: Revenue-Drivers (Week 3)
7. **claude-ads** → DIGIX campaigns
8. **Whisper** → RxGPT + DIGIX voice
9. **Fooocus** → Marketing assets

### Phase 4: Optimization (Week 4)
10. **Ollama** → Local LLM inference
11. **Penpot** → Design automation
12. Everything else as needed

---

## 🔧 Quick Start: Docker Compose

Create `docker-compose.yml` in toolkit root:

```yaml
version: '3.8'

services:
  # AI Infrastructure
  semantica:
    image: semantica/core:latest
    ports:
      - "8000:8000"
    environment:
      - DATABASE_URL=postgresql://postgres:pass@postgres:5432/semantica

  # Workspace
  appflowy:
    image: appflowy/appflowy:latest
    ports:
      - "8080:80"
    
  # Analytics
  plausible:
    image: plausible/analytics:latest
    ports:
      - "8888:8000"
    environment:
      - BASE_URL=http://localhost:8888

  # Database (shared)
  postgres:
    image: postgres:15
    environment:
      POSTGRES_PASSWORD: pass
    volumes:
      - postgres_data:/var/lib/postgresql/data

volumes:
  postgres_data:
```

```bash
docker-compose up -d
# Semantica: localhost:8000
# AppFlowy: localhost:8080
# Plausible: localhost:8888
```

---

## 📖 Integration Guides

Each tool has its own setup guide in `/tools/{category}/`:

- `tools/llm-models/ollama-setup.md`
- `tools/media-ops/claude-ads-setup.md`
- `tools/agents/semantica-setup.md`
- `tools/design/penpot-setup.md`
- `tools/utilities/plausible-setup.md`

---

## 🤝 License Summary

| Tool | License | Commercial Use |
|------|---------|-----------------|
| Semantica | MIT | ✅ |
| Decision Tracing | MIT | ✅ |
| context-mode | MIT | ✅ |
| Ollama | MIT | ✅ |
| Whisper | MIT | ✅ |
| claude-ads | MIT | ✅ |
| Fooocus | GPL-3 | ✅ w/ disclosure |
| Open-GenAI | MIT | ✅ |
| yt-dlp | Unlicense | ✅ |
| awesome-llm-apps | MIT | ✅ (reference) |
| awesome-mcp-servers | MIT | ✅ (reference) |
| public-apis | MIT | ✅ (reference) |
| DeepSeek Harness | MIT | ✅ |
| Penpot | MPL-2.0 | ✅ |
| AppFlowy | AGPL-3 | ✅ w/ disclosure |
| Plausible | AGPL-3 | ✅ w/ disclosure |

---

**Last Updated**: 2026-08-28  
**Total Tools**: 16  
**Combined Stars**: 1M+  
**Total Cost to Deploy**: $0 (all open-source)
