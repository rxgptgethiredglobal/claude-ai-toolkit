# External Tools Directory 🛠️

**20 curated open-source projects** for integrating with Claude, your agents, and projects.

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
**"Everything is a Plugin"** — Universal LLM framework

- **Use**: Add LLM to any codebase instantly
- **GitHub**: [deepseek-ai/deepseek-harness](https://github.com/deepseek-ai/deepseek-harness)
- **201K stars, 23.1K forks**

---

## 🛠 Agent & Workflow Builders

### 17. **Langflow** ⭐ FOR VISUAL AGENT DESIGN
**Build AI agents & RAG workflows visually** — Drag-and-drop, deploy as APIs/MCP

- **What**: Visual builder for agents and flows
- **Use**: Hemraj agents, DIGIX SDR, LeadVault pipelines (no code)
- **Deploy**: Web UI, API generation, MCP servers
- **GitHub**: [langflow-ai/langflow](https://github.com/langflow-ai/langflow)
- **153K stars**

```bash
docker run -it -p 7860:7860 langflowai/langflow
# Build complex flows visually, export as Python/FastAPI
```

---

### 18. **OpenHands** ⭐ AUTONOMOUS CODING AGENT
**Self-hosted coding agent** — Write code, run tests, debug, autonomous development

- **What**: Autonomous agent that can code (like Claude but self-hosted)
- **Use**: Hemraj agent code generation, testing, debugging
- **Deploy**: Docker, local or cloud
- **GitHub**: [All-Hands-AI/OpenHands](https://github.com/All-Hands-AI/OpenHands)
- **84K stars**

```bash
# Run agent to complete dev tasks
openagents execute "Add tests for pricing agent"
```

---

## 🔍 Data & Web Integration

### 19. **Scraping** ⭐ WEB SCRAPING FRAMEWORK
**Adaptive web scraping** — Anti-bot bypass, Cloudflare handling, proxy rotation

- **What**: Enterprise web scraping (handles modern sites)
- **Use**: LeadVault data harvesting, market research, competitor monitoring
- **Features**: Learns from site changes, auto-relocates selectors
- **GitHub**: [D4Vinci/Scraping](https://github.com/D4Vinci/Scraping)
- **73.6K stars**

```bash
pip install scraping-ai
scraping-ai --url https://example.com --extract "pricing, features"
```

---

### 20. **Free-for-dev** ⭐ DEVELOPER TOOLS DIRECTORY
**132K collection of developer tools with free/permanent tiers**

- **What**: Massive directory of free dev services (hosting, databases, APIs, etc.)
- **Use**: Find free alternatives for all projects (Hemraj, LeadVault, etc.)
- **Categories**: Hosting, DBs, APIs, monitoring, design, analytics
- **GitHub**: [ripienaar/free-for-dev](https://github.com/ripienaar/free-for-dev)
- **132K stars**

---

## 🎨 Design Automation

### 21. **Open Design** ⭐ OPEN-SOURCE CLAUDE DESIGN
**Claude Design alternative** — AI-powered design workflows open-source

- **What**: Design system automation (turn Claude Design into a workflow)
- **Use**: DIGIX frontend design, Penpot integration
- **Deploy**: Self-hosted design agent
- **GitHub**: [nexu-io/open-design](https://github.com/nexu-io/open-design)
- **85K stars**

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

## 🌐 Modern AI Ecosystem (Complete Stack)

### LLMs & Foundation Models
- **Claude** (Anthropic) — 200K context, multimodal, strong reasoning
- **GPT-4o** (OpenAI) — Vision, fast, production-ready
- **Gemini** (Google) — Multimodal, long context
- **Llama 3** (Meta) — Open-source, efficient
- **Mistral** — Sparse experts, efficient
- **DeepSeek** — Cost-effective reasoning
- **Phi-3** (Microsoft) — Lightweight, edge

### RAG & Retrieval
- **LangChain** — Orchestration, chains, memory
- **LlamaIndex** — Document indexing, retrieval
- **Haystack** — Production pipelines
- **RAGFlow** — Open-source orchestration
- **GraphRAG** — Knowledge graph + retrieval

### Vector Databases (Embeddings)
- **Pinecone** — Managed, serverless
- **Weaviate** — Open-source, GraphQL
- **Qdrant** — High-performance
- **Milvus** — Scalable
- **Chroma** — Lightweight
- **Redis** — Vector + caching
- **Elasticsearch** — Full-text + vector

### Data Ingestion
- **Unstructured** — Parse PDFs, images, docs
- **FireCrawl** — Website to LLM-ready data
- **Docling** — Document understanding
- **Beautiful Soup** — HTML/XML parsing

### AI Security & Guardrails
- **NVIDIA NeMo Guardrails** — Conversation safety
- **Guardrails AI** — Input/output validation
- **Microsoft Presidio** — PII detection
- **Lakera** — Prompt injection detection
- **ProtectAI** — ML security

### Observability & Monitoring
- **LangSmith** — Debug & test LLM apps
- **Langfuse** — Open-source analytics
- **TruLens** — RAG evaluation
- **Ragas** — RAG assessment
- **Promptfoo** — Eval harness
- **Weights & Biases** — Experiment tracking
- **OpenTelemetry** — Standard observability

### Memory & State
- **Mem0** — Persistent agent memory
- **Zep** — Long-term memory layer
- **Redis** — Distributed state
- **PostgreSQL** — Relational storage

### AI Agents & Orchestration
- **LangGraph** — Agent state machines
- **PydanticAI** — Type-safe agents
- **Semantic Kernel** — Multi-model reasoning
- **AWS Bedrock Agents** — Managed agents
- **Azure AI Foundry** — Enterprise agents

### Deployment & Infrastructure
- **AWS** — SageMaker, Bedrock, Lambda
- **Google Cloud** — Vertex AI, Cloud Run
- **Azure** — Azure AI, Machine Learning
- **Vercel** — Edge inference
- **Docker** — Containerization
- **Kubernetes** — Orchestration at scale

### Evaluation & Testing
- **Ragas** — RAG evaluation
- **DeepEval** — LLM testing
- **Giskard** — Model testing
- **UpTrain** — Quality assurance

### Prompt Engineering
- **PromptHub** — Prompt marketplace
- **PromptPerfect** — Optimization
- **HumanLoop** — RLHF platform
- **TextGrad** — Gradient-based tuning

---

## ⚙️ Harness Engineering (Model + Harness = Agent)

**The Equation**: `Model + Harness = Coding Agent`

The **model** is one term (Claude, GPT-4, Llama). The **harness** is everything else:

### Harness Components
- **Loop** — Feedback iteration (plan → act → evaluate → improve)
- **Tools** — Functions the agent can call (APIs, databases, GitHub, etc.)
- **Gate** — Safety guardrails (input validation, policy checks, output screening)
- **Context** — Persistent state (project files, memory, history)
- **Checkpoints** (ckpt) — Save/restore agent state mid-task
- **Sub-agents** — Delegate to specialized workers (retrieval agent, code agent, etc.)

### Why It Matters
- Model alone = not an agent (it's just prediction)
- Harness = makes it autonomous, reliable, safe
- Your projects: Hemraj harness orchestrates 13 agents; each agent has its harness

---

## 🎯 Agent Governance & Evals 2.0 (Microsoft Foundry Pattern)

### Retrieval as a Subagent (Self-Healing)
1. **Plan** — Understand what info is needed
2. **Query Sources** — Search docs, wiki, blob storage
3. **Evaluate Good?** — If yes → grounded answer; if no → marked "I don't know"
4. **Iterate** — Retry if sources exhausted
5. **Output** — Answer with citations or structured "I don't know"

**Your use**: LeadVault knowledge base, Hemraj market data retrieval

### Eval & Optimizer Loop (Production-Grade Testing)
1. **Run Rubrics** — Evaluate agent response against 5+ dimensions
2. **Pass All?** — If YES → ship agent; if NO → optimize
3. **Agent Optimizer** — Generate & test candidate fixes:
   - Rewrite prompt
   - Adjust tool use
   - Swap model
   - Re-rank sources
   - Tune skills
4. **Score Candidates** — Pick best performing fix
5. **Promote Best** — Move to production

**Your use**: Test Hemraj pricing agent before live deployment; validate DIGIX SDR scoring

---

## 🎯 AI Engineer's Stack (8 Core Areas)

### 1. LLMs (Foundation)
- Claude, GPT-4o, Gemini, Llama, Mistral
- **Cost**: varies; Claude token-based
- **Use**: Core reasoning for all agents

### 2. Frameworks (Orchestration)
- LangChain, LlamaIndex, Semantic Kernel, LangGraph
- **Purpose**: Chain LLM calls, manage memory, routing
- **Critical for**: Hemraj 13 agents, LeadVault pipelines

### 3. Vector Databases (Knowledge)
- Pinecone, Weaviate, Qdrant, Milvus
- **Purpose**: Store embeddings, fast retrieval
- **Critical for**: RAG in all projects

### 4. Data Ingestion (Input)
- FireCrawl, Unstructured, Docling
- **Purpose**: Convert docs → LLM-ready format
- **Critical for**: LeadVault data mining

### 5. Observability & Monitoring (Visibility)
- LangSmith, Langfuse, Ragas, TruLens
- **Purpose**: Debug, evaluate, monitor pipelines
- **Critical for**: Hemraj agent optimization

### 6. Deployment & Infrastructure (Production)
- AWS (Bedrock, SageMaker), GCP (Vertex, Cloud Run), Kubernetes
- **Purpose**: Scale agents globally
- **Critical for**: RxGPT HIPAA compliance

### 7. Evaluation & Testing (Quality)
- Ragas, DeepEval, Promptfoo, Giskard
- **Purpose**: Test inputs → verify outputs
- **Critical for**: Agent safety, reliability

### 8. Prompt Engineering (Fine-Tuning)
- Prompt optimization, in-context learning, few-shot patterns
- **Purpose**: Maximize LLM performance
- **Critical for**: All agent instruction design

---

## 🚀 Complete AI Agent Development Stack (All Layers)

### Layer 1: Foundations
- **Python** — Backend language for agents (FastAPI, Django)
- **JavaScript** — Frontend + Node.js backend
- **Git** — Version control for agent code

### Layer 2: LLMs (Core Models)
- **OpenAI GPT** — Industry standard
- **Claude** (Anthropic) — Strong reasoning
- **Gemini** (Google) — Multimodal
- **Llama** (Meta) — Open-source

### Layer 3: AI Frameworks (Orchestration)
- **LangChain** — Chain LLM calls, memory, agents
- **LangGraph** — State machines for multi-step workflows
- **LlamaIndex** — Document indexing + retrieval

### Layer 4: Agent Skills (Capabilities)
- **Prompt Engineering** — Optimize instructions
- **Tool Calling** — Call external functions
- **Function Calling** — Structured outputs
- **RAG** — Retrieve external knowledge
- **Memory** — Persistent state (short/long-term)
- **Multi-Agent Systems** — Coordinate multiple agents

### Layer 5: Databases (State Storage)
- **Vector DB** (Pinecone, Qdrant, Chroma) — Embeddings storage
- **ChromaDB** — Lightweight embeddings
- **FAISS** — Facebook vector search
- **PostgreSQL** — Relational data

### Layer 6: APIs (Connectivity)
- **REST API** — Stateless HTTP endpoints
- **GraphQL** — Query language for APIs
- **MCP** (Model Context Protocol) — Standard tool layer

### Layer 7: Deployment & Infrastructure
- **Docker** — Containerization
- **FastAPI** — Fast Python API framework
- **Vercel** — Edge deployment

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

**Last Updated**: 2026-08-29  
**Total Tools**: 20  
**Combined Stars**: 1.5M+  
**Total Cost to Deploy**: $0 (all open-source)
