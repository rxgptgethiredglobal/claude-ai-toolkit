# GenAI Concepts Applied Across Projects 🎯

**Master Framework**: 30 Core GenAI Concepts mapped to Hemraj, LeadVault, DIGIX, RxGPT, HireX, and Fractional CMO projects.

---

## Quick Reference: Concept-to-Project Matrix

| Concept | Hemraj | LeadVault | DIGIX | RxGPT | HireX | Frac CMO |
|---------|--------|-----------|-------|-------|-------|----------|
| **1. Transformer** | Agent reasoning | Retrieval | Ad reasoning | Clinical decision | Resume parsing | Content generation |
| **2. Self-Attention** | Multi-agent focus | Query attention | Campaign priority | Patient history | Candidate relevance | Post relevance |
| **3. Tokenization** | Pricing tokens | Query tokens | Ad copy tokens | Medical notes tokens | Resume tokens | Content tokens |
| **4. Embeddings** | Market data vectors | Lead vectors | Campaign vectors | Medical vectors | Resume vectors | Content vectors |
| **5. Context Window** | Prompt length (agent) | Query scope | Campaign scope | Patient history scope | Resume scope | Post length |
| **6. KV Cache** | Agent memory cache | Query cache | Ad cache | Session cache | Resume cache | Post cache |
| **7. Temperature** | Pricing variance | Retrieval strictness | Creative risk | Recommendation conservatism | Candidate rank variance | Post tone variation |
| **8. Hallucination** | Price hallucination risk | Retrieval hallucination | False ad claims | Misdiagnosis risk | Resume false info | Fake engagement claims |
| **9. Zero-shot** | Agent prompting | Query prompting | Ad copy generation | Clinical reasoning | Screening prompts | Content prompting |
| **10. Chain-of-Thought** | Pricing logic chain | Lead scoring logic | Campaign planning chain | Diagnosis reasoning chain | Resume evaluation chain | Content strategy chain |
| **11. RAG** | Market data retrieval | Lead database retrieval | Campaign asset retrieval | Medical records retrieval | Candidate DB retrieval | Content library retrieval |
| **12. Chunking Strategy** | Market data chunks | Lead segmentation | Campaign chunks | Medical record chunks | Resume segmentation | Content segmentation |
| **13. Vector Database** | Pinecone (market data) | Weaviate (leads) | Chroma (campaigns) | Qdrant (medical) | Milvus (resumes) | Redis (content) |
| **14. Cosine Similarity** | Price similarity search | Lead similarity | Campaign similarity | Symptom similarity | Resume similarity | Content similarity |
| **15. Hybrid Search** | Price + keyword search | Intent + keyword | Trend + keyword | Symptom + text | Skill + keyword | Topic + keyword |
| **16. Reranking** | Price rank refinement | Lead score refinement | Campaign priority refinement | Diagnosis refinement | Candidate rank refinement | Content priority refinement |
| **17. Agentic RAG** | Agent-driven retrieval | Dynamic retrieval | Campaign asset retrieval | Patient record retrieval | Resume retrieval | Content retrieval on demand |
| **18. AI Agent** | 13 core agents | Mining brain agent | Marketing agent | Diagnosis agent | Screening agent | Content agent |
| **19. ReAct Pattern** | Agent reasoning loop | Mining loop | Campaign loop | Clinical reasoning loop | Screening loop | Content creation loop |
| **20. Tool Calling** | Pricing tools, APIs | Query tools | Ad platforms | Hospital systems | HRIS systems | Social platforms |
| **21. Agent Memory** | Seasonal trends memory | Lead conversation history | Campaign performance memory | Patient medical history | Candidate history | Campaign performance memory |
| **22. Multi-Agent** | 13-agent orchestration | Mining brain + filters | Content + outreach | Intake + clinical + follow-up | Sourcing + screening + outreach | Content + posting + analytics |
| **23. MCP** | Tool discovery layer | Retrieval MCP | Marketing MCP | Hospital MCP | HRIS MCP | Social media MCP |
| **24. Fine-tune vs RAG** | Market forecasting (fine-tune) | Lead ranking (RAG) | Campaign templates (RAG) | Clinical decisions (fine-tune) | Resume parsing (fine-tune) | Brand guidelines (RAG) |
| **25. LoRA** | Lightweight pricing tuning | Lightweight ranking | Lightweight copy | Lightweight diagnosis | Lightweight screening | Lightweight tone tuning |
| **26. QLoRA** | Mobile price inference | Edge retrieval | Mobile ad generation | Mobile patient triage | Mobile resume screening | Mobile post generation |
| **27. RLHF** | Pricing preference alignment | Relevance preference | Engagement preference | Clinical preference | Hiring preference | Content preference |
| **28. RAGAS** | RAG retrieval quality | Lead retrieval quality | Campaign asset quality | Medical record quality | Resume retrieval quality | Content retrieval quality |
| **29. LLM-as-Judge** | Price fairness judge | Lead quality judge | Campaign quality judge | Diagnosis confidence judge | Resume quality judge | Content quality judge |
| **30. Prompt Injection** | Input validation (prices) | Input validation (queries) | Input validation (briefs) | Input validation (symptoms) | Input validation (resumes) | Input validation (content briefs) |

---

## The 30 Concepts: Applied Framework

### **FOUNDATIONS (1-10): How Modern AI Works**

**1. Transformer Architecture**
- **What**: Parallel token processing with self-attention (powers all LLMs)
- **Why it matters**: Without transformers, LLMs would be too slow
- **Your applications**:
  - **Hemraj**: Pricing agent uses transformer reasoning to evaluate market conditions in parallel
  - **LeadVault**: Lead scoring uses transformer attention to weight intent signals
  - **DIGIX**: Campaign planning agent attends to multiple strategic goals simultaneously
  - **RxGPT**: Clinical reasoning uses transformers to process patient history in parallel
  - **HireX**: Resume parser uses transformer architecture for parallel skill extraction
  - **Frac CMO**: Content generation uses transformers for multi-goal optimization

---

**2. Self-Attention Mechanism**
- **What**: Each token "attends to" (focuses on) all other tokens to understand context
- **Why it matters**: Creates long-range dependencies and contextual understanding
- **Your applications**:
  - **Hemraj**: Pricing agent attends to seasonal trends, competitor prices, and demand signals
  - **LeadVault**: Lead quality agent attends to funding, hiring, and topic signals together
  - **DIGIX**: Campaign agent attends to brand rules, platform constraints, and goals
  - **RxGPT**: Clinical agent attends to symptoms, medical history, and patient preferences
  - **HireX**: Screening agent attends to job requirements and candidate profile
  - **Frac CMO**: Content agent attends to brand voice, audience, and campaign goals

---

**3. Tokenization**
- **What**: Breaking text into tokens (~4 chars/token) for LLM processing
- **Why it matters**: Affects cost, latency, and context efficiency
- **Your applications**:
  - **Hemraj**: ~1K tokens for pricing decision (market data + logic)
  - **LeadVault**: ~500 tokens per lead (company + person data)
  - **DIGIX**: ~300 tokens per post (caption + hashtags + brand rules)
  - **RxGPT**: ~2K tokens per patient intake (symptoms + history)
  - **HireX**: ~1.5K tokens per resume (parsed skills + experience)
  - **Frac CMO**: ~400 tokens per content brief (goal + brand + platform)

---

**4. Embeddings (Vectors)**
- **What**: Converting text/data into dense numerical vectors (768-4K dimensions)
- **Why it matters**: Enables semantic search, similarity, and retrieval
- **Your applications**:
  - **Hemraj**: Market data embedded as 1536-dim vectors (OpenAI) for similarity search
  - **LeadVault**: Lead profiles embedded for intent matching
  - **DIGIX**: Campaign templates embedded for style transfer
  - **RxGPT**: Medical records embedded for pattern matching
  - **HireX**: Resumes embedded for candidate matching
  - **Frac CMO**: Content pieces embedded for brand consistency checking

---

**5. Context Window**
- **What**: Maximum tokens an LLM can see at once (Claude = 200K, GPT-4 = 128K)
- **Why it matters**: Determines what history/data you can include in a single request
- **Your applications**:
  - **Hemraj**: 100K tokens for pricing decision (full year market data + strategy)
  - **LeadVault**: 50K tokens for lead prioritization (all leads + their signals)
  - **DIGIX**: 30K tokens for campaign planning (all goals + brand rules + calendar)
  - **RxGPT**: 80K tokens for patient care (full medical history + current visit)
  - **HireX**: 60K tokens for hiring pipeline (all candidates + job reqs)
  - **Frac CMO**: 20K tokens for content calendar (all 30 days + brand guidelines)

---

**6. KV Cache (Key-Value Cache)**
- **What**: Caching attention keys/values during inference for speed
- **Why it matters**: Reduces latency during streaming/long conversations
- **Your applications**:
  - **Hemraj**: Cache pricing decisions for similar markets (don't recalculate)
  - **LeadVault**: Cache lead scoring results for repeated queries
  - **DIGIX**: Cache campaign templates for repeated use
  - **RxGPT**: Cache patient history for multi-turn conversations
  - **HireX**: Cache resume parsing for batch processing
  - **Frac CMO**: Cache content templates for repeated posts

---

**7. Temperature & Top-P**
- **What**: Sampling parameters (0=deterministic, 1=random) controlling output creativity
- **Why it matters**: Balances consistency vs. creativity
- **Your applications**:
  - **Hemraj**: Temperature=0.2 for pricing (need consistency, not creativity)
  - **LeadVault**: Temperature=0.5 for lead scoring (some variation OK)
  - **DIGIX**: Temperature=0.7 for ad copy (need creativity)
  - **RxGPT**: Temperature=0.1 for diagnosis (need consistency)
  - **HireX**: Temperature=0.3 for screening (need consistency)
  - **Frac CMO**: Temperature=0.8 for post ideas (need creativity)

---

**8. Hallucination**
- **What**: AI generating false/made-up information confidently
- **Why it matters**: Kills trust in production systems
- **Your applications**:
  - **Hemraj**: Risk: Pricing agent hallucinating competitor prices → Solution: RAG + validation
  - **LeadVault**: Risk: Lead data hallucination → Solution: Only return retrieved data
  - **DIGIX**: Risk: False engagement claims → Solution: Guardrails on metrics
  - **RxGPT**: Risk: False medical claims → Solution: Grounding + HIPAA audit
  - **HireX**: Risk: Fake candidate info → Solution: Source verification
  - **Frac CMO**: Risk: False engagement numbers → Solution: API-based metrics only

---

**9. Zero-Shot & Few-Shot Prompting**
- **What**: Prompting without examples (zero-shot) or with a few examples (few-shot)
- **Why it matters**: Determines how much example data you need to bootstrap
- **Your applications**:
  - **Hemraj**: Few-shot pricing (3 examples of similar markets + decisions)
  - **LeadVault**: Zero-shot lead scoring (scoring rules in system prompt)
  - **DIGIX**: Few-shot campaign planning (3 example calendars)
  - **RxGPT**: Few-shot clinical reasoning (3 similar patient cases)
  - **HireX**: Few-shot screening (3 example good/bad resumes)
  - **Frac CMO**: Few-shot content generation (3 brand examples)

---

**10. Chain-of-Thought**
- **What**: Prompting the LLM to show its reasoning step-by-step
- **Why it matters**: Improves accuracy on complex tasks
- **Your applications**:
  - **Hemraj**: "Show pricing logic: demand + supply + margin = price"
  - **LeadVault**: "Show scoring logic: funding + hiring + engagement = intent score"
  - **DIGIX**: "Show planning logic: goals → themes → content pieces → schedule"
  - **RxGPT**: "Show diagnosis logic: symptoms → differential → tests → conclusion"
  - **HireX**: "Show screening logic: job requirements → resume signals → score"
  - **Frac CMO**: "Show content logic: goal → audience → platform → format → copy"

---

### **RETRIEVAL & KNOWLEDGE (11-20): How AI Knows Things**

**11. RAG (Retrieval-Augmented Generation)**
- **What**: Ground AI in real data by retrieving relevant documents before generating
- **Why it matters**: Prevents hallucination, enables current data, reduces cost
- **Your applications**:
  - **Hemraj**: Retrieve market data (pricing history, competitor data, demand trends)
  - **LeadVault**: Retrieve lead database (company info, funding, hiring signals)
  - **DIGIX**: Retrieve campaign templates, brand guidelines, historical performance
  - **RxGPT**: Retrieve patient records, clinical guidelines, treatment history
  - **HireX**: Retrieve candidate profiles, job descriptions, hiring history
  - **Frac CMO**: Retrieve content library, brand guidelines, competitor content

---

**12. Chunking Strategy**
- **What**: Breaking documents into chunks (256-1K tokens) for embedding/retrieval
- **Why it matters**: Affects retrieval quality and cost
- **Your applications**:
  - **Hemraj**: Chunk by market/time period (Q1 pricing data vs Q2)
  - **LeadVault**: Chunk by company + contacts (one chunk = company + all contacts)
  - **DIGIX**: Chunk by platform + goal (Instagram content chunks vs LinkedIn)
  - **RxGPT**: Chunk by visit + date (one chunk = one patient visit)
  - **HireX**: Chunk by job + candidates (one chunk = job + 10 candidates)
  - **Frac CMO**: Chunk by platform + week (Instagram week 1, week 2, etc.)

---

**13. Vector Databases**
- **What**: Specialized databases storing embeddings for fast semantic search
- **Why it matters**: Enables retrieval at scale (100K+ documents)
- **Your applications**:
  - **Hemraj**: Pinecone (1 namespace per market, 10K+ pricing decisions)
  - **LeadVault**: Weaviate (76K leads with intent signals)
  - **DIGIX**: Chroma (in-memory for 30-day content calendar)
  - **RxGPT**: Qdrant (10K+ patient records, HIPAA-compliant)
  - **HireX**: Milvus (100K resumes, parallel search)
  - **Frac CMO**: Redis (in-memory content cache for speed)

---

**14. Cosine Similarity & ANN Search**
- **What**: Finding nearest vectors (most similar documents) using cosine distance
- **Why it matters**: The core of semantic search
- **Your applications**:
  - **Hemraj**: Find similar past pricing decisions (nearest neighbor in price space)
  - **LeadVault**: Find similar leads (companies with similar funding/hiring signals)
  - **DIGIX**: Find similar content templates (style transfer)
  - **RxGPT**: Find similar patient cases (pattern matching)
  - **HireX**: Find similar resumes (candidate matching)
  - **Frac CMO**: Find similar content (brand consistency)

---

**15. Hybrid Search**
- **What**: Combining vector search (semantic) + keyword search (exact match)
- **Why it matters**: Gets best of both worlds
- **Your applications**:
  - **Hemraj**: Vector search for similar prices + keyword search for "Q1 2026 prices"
  - **LeadVault**: Vector search for similar intent + keyword search for "funded in 2026"
  - **DIGIX**: Vector search for similar campaigns + keyword search for "Q1 posts"
  - **RxGPT**: Vector search for similar symptoms + keyword search for "diabetes"
  - **HireX**: Vector search for similar resumes + keyword search for "Python developer"
  - **Frac CMO**: Vector search for similar posts + keyword search for "brand guidelines"

---

**16. Reranking**
- **What**: Re-scoring retrieved results (LLM-based or ML model) to improve top-1 accuracy
- **Why it matters**: Search returns 10 results; reranking picks the best one
- **Your applications**:
  - **Hemraj**: Retrieve 5 similar prices, rerank by market conditions
  - **LeadVault**: Retrieve 20 leads, rerank by purchase intent confidence
  - **DIGIX**: Retrieve 10 templates, rerank by campaign goal match
  - **RxGPT**: Retrieve 5 similar cases, rerank by symptom match
  - **HireX**: Retrieve 20 resumes, rerank by job match
  - **Frac CMO**: Retrieve 10 posts, rerank by brand alignment

---

**17. Agentic RAG**
- **What**: Agent autonomously decides when/what/how to retrieve
- **Why it matters**: Mimics expert behavior (ask the right question before searching)
- **Your applications**:
  - **Hemraj**: Pricing agent decides "I need Q1 comparable prices" before retrieving
  - **LeadVault**: Mining agent decides "I need funded AI startups" before querying
  - **DIGIX**: Campaign agent decides "I need brand rules" before generating copy
  - **RxGPT**: Clinical agent decides "I need patient's medication history" before recommending
  - **HireX**: Screening agent decides "I need similar successful candidates" before ranking
  - **Frac CMO**: Content agent decides "I need brand voice examples" before writing

---

**18. AI Agent**
- **What**: Autonomous system with planning, tool use, and decision-making
- **Why it matters**: Scales your thinking (agents work 24/7)
- **Your applications**:
  - **Hemraj**: 13 core agents (Pricing, Forecasting, Procurement, Quality, Sales, Logistics, Market Intelligence)
  - **LeadVault**: Mining brain agent (discovers, scores, exports leads)
  - **DIGIX**: Marketing agent (plans calendars, writes copy, posts)
  - **RxGPT**: Intake agent + Clinical agent + Follow-up agent
  - **HireX**: Sourcing agent + Screening agent + Outreach agent + Onboarding agent
  - **Frac CMO**: Content agent + Posting agent + Analytics agent

---

**19. ReAct Pattern (Reasoning + Acting)**
- **What**: Agent alternates between thinking (reasoning) and doing (acting)
- **Why it matters**: Makes agent decisions interpretable and debuggable
- **Your applications**:
  - **Hemraj**: Reason "demand is high" → Act "increase price by 5%"
  - **LeadVault**: Reason "company just raised Series A" → Act "score 9/10"
  - **DIGIX**: Reason "brand rule is no emojis" → Act "remove emojis from post"
  - **RxGPT**: Reason "symptoms match diabetes pattern" → Act "recommend glucose test"
  - **HireX**: Reason "resume has Python + ML" → Act "match to ML engineer role"
  - **Frac CMO**: Reason "goal is awareness" → Act "write educational post"

---

**20. Tool Calling (Function Calling)**
- **What**: LLM calls external APIs/functions (Stripe, Slack, databases)
- **Why it matters**: Connects AI to real systems (can't change world with text alone)
- **Your applications**:
  - **Hemraj**: Call pricing API, inventory DB, forecast model
  - **LeadVault**: Call GraphQL (Product Hunt), REST (Crunchbase), CSV (master list)
  - **DIGIX**: Call Instagram API, LinkedIn API, Facebook API, Analytics API
  - **RxGPT**: Call hospital records API, pharmacy API, patient SMS API
  - **HireX**: Call HRIS (ATS), email API, outreach platform API
  - **Frac CMO**: Call Twitter/X API, Instagram API, LinkedIn API, Analytics API

---

### **ADVANCED PATTERNS (21-30): How AI Becomes Autonomous**

**21. Agent Memory**
- **What**: Long-term context (episodic = past events, semantic = general knowledge)
- **Why it matters**: Enables multi-turn conversations and learning
- **Your applications**:
  - **Hemraj**: Seasonal trends memory (Q1 = high demand, Q4 = low demand)
  - **LeadVault**: Lead conversation history (company A has been contacted 3x)
  - **DIGIX**: Campaign performance memory (post type X gets 20% engagement)
  - **RxGPT**: Patient medical history (diabetic since 2020, on Metformin)
  - **HireX**: Candidate history (applied for role A, rejected, offered role B)
  - **Frac CMO**: Campaign performance memory (LinkedIn posts get 2x engagement)

---

**22. Multi-Agent Orchestration**
- **What**: Coordinating multiple agents to complete complex tasks
- **Why it matters**: Breaks big problems into specialised subproblems
- **Your applications**:
  - **Hemraj**: 13 agents with handoffs (forecasting → pricing → sales → logistics)
  - **LeadVault**: Mining brain + filtering agents + export agents
  - **DIGIX**: Content agent → Posting agent → Analytics agent (handoff at each step)
  - **RxGPT**: Intake agent → Clinical agent → Follow-up agent
  - **HireX**: Sourcing agent → Screening agent → Outreach agent → Onboarding agent
  - **Frac CMO**: Content agent → Posting agent → Analytics agent

---

**23. MCP (Model Context Protocol)**
- **What**: Standard tool interface for agent-to-tool communication
- **Why it matters**: Standardizes how agents discover and use tools (like HTTP did for web)
- **Your applications**:
  - **Hemraj**: MCP for pricing tools, forecast tools, inventory tools
  - **LeadVault**: MCP for data source tools, filtering tools, export tools
  - **DIGIX**: MCP for social media APIs, scheduling tools, analytics tools
  - **RxGPT**: MCP for hospital record systems, pharmacy systems, SMS systems
  - **HireX**: MCP for HRIS, ATS, email, outreach platforms
  - **Frac CMO**: MCP for social APIs, scheduling tools, analytics

---

**24. Fine-tuning vs RAG vs Prompting**
- **What**: Three ways to adapt LLMs (fine-tune model, retrieve documents, design prompts)
- **Why it matters**: Each has different cost/accuracy/speed tradeoffs
- **Your applications**:
  - **Hemraj**: Market forecasting (fine-tune on 5 years of data) vs pricing logic (RAG + prompt)
  - **LeadVault**: Lead ranking (fine-tune on scoring history) vs retrieval (RAG)
  - **DIGIX**: Campaign templates (RAG) vs brand voice (fine-tune on examples)
  - **RxGPT**: Diagnosis (fine-tune on medical cases) vs patient records (RAG)
  - **HireX**: Resume parsing (fine-tune on labeled resumes) vs job matching (RAG)
  - **Frac CMO**: Brand voice (fine-tune on examples) vs content templates (RAG)

---

**25. LoRA (Low-Rank Adaptation)**
- **What**: Efficient fine-tuning using only 1-2% of model parameters
- **Why it matters**: 100x cheaper and faster than full fine-tuning
- **Your applications**:
  - **Hemraj**: LoRA fine-tune pricing logic for industry-specific rules
  - **LeadVault**: LoRA fine-tune lead scoring for your specific intent signals
  - **DIGIX**: LoRA fine-tune brand voice for your specific tone
  - **RxGPT**: LoRA fine-tune clinical reasoning for your specific patient population
  - **HireX**: LoRA fine-tune resume parsing for your specific fields
  - **Frac CMO**: LoRA fine-tune content generation for your specific brand

---

**26. QLoRA (Quantized LoRA)**
- **What**: LoRA with quantization (4-bit precision instead of 32-bit)
- **Why it matters**: Fine-tune on your laptop instead of GPU cloud
- **Your applications**:
  - **Hemraj**: Run pricing model locally during outages
  - **LeadVault**: Run scoring locally for privacy-critical leads
  - **DIGIX**: Run content generation locally for brand control
  - **RxGPT**: Run clinical reasoning locally for offline clinics
  - **HireX**: Run screening locally without HRIS API dependency
  - **Frac CMO**: Run content generation locally for offline work

---

**27. RLHF & DPO (Reinforcement Learning from Human Feedback)**
- **What**: Training models to match human preferences instead of training data
- **Why it matters**: Aligns model behavior to what users actually want
- **Your applications**:
  - **Hemraj**: Train pricing agent to match your preferred price ranges
  - **LeadVault**: Train scoring to match your "high quality lead" definition
  - **DIGIX**: Train copy to match your brand voice preferences
  - **RxGPT**: Train diagnosis agent to match clinician clinical judgment
  - **HireX**: Train screening to match your hiring preferences
  - **Frac CMO**: Train content to match engagement patterns you prefer

---

**28. RAGAS Metrics (RAG Assessment)**
- **What**: Metrics for evaluating RAG quality (context precision, recall, relevance)
- **Why it matters**: Tells you if your retrieval is working
- **Your applications**:
  - **Hemraj**: Context precision: does retrieved market data match pricing decision?
  - **LeadVault**: Context recall: do we retrieve all relevant leads?
  - **DIGIX**: Answer relevance: does retrieved content match campaign goal?
  - **RxGPT**: Context precision: does retrieved medical history match current symptoms?
  - **HireX**: Context recall: do we retrieve all matching candidates?
  - **Frac CMO**: Answer relevance: does retrieved content match brand?

---

**29. LLM-as-Judge**
- **What**: Using an LLM to evaluate outputs instead of manual labels
- **Why it matters**: Scales evaluation without hiring humans
- **Your applications**:
  - **Hemraj**: Judge: "Is this price fair given market conditions?"
  - **LeadVault**: Judge: "Is this lead high quality?"
  - **DIGIX**: Judge: "Does this post match brand guidelines?"
  - **RxGPT**: Judge: "Is this diagnosis confidence score justified?"
  - **HireX**: Judge: "Is this candidate ranked correctly?"
  - **Frac CMO**: Judge: "Does this content follow brand voice?"

---

**30. Prompt Injection & Guardrails**
- **What**: Attack vector (malicious user input overwrites system prompt) + defenses
- **Why it matters**: Production safety
- **Your applications**:
  - **Hemraj**: Validate pricing input (can't accept negative prices)
  - **LeadVault**: Sanitize lead data before retrieval (strip SQL injection attempts)
  - **DIGIX**: Validate brand rules aren't overridden by user input
  - **RxGPT**: Validate medical data (no fake symptoms injected)
  - **HireX**: Validate candidate data (no injected requirements)
  - **Frac CMO**: Validate brand rules in every post

---

## Applied Case Studies (STAR Format)

### Case Study 1: HireX AI — "The 90-Day Myth" College GTM Campaign

**Situation**: HireX AI needed college GTM but legacy ATS positioning was weak  
**Task**: Rebuild narrative for institutional buyers (college owners, deans, TPOs)  
**Action**: Built 30-day content calendar (LinkedIn, email, outreach kit) with "Career Readiness Audit" as wedge  
**Result**: Full campaign strategy with Day-29 lead offer, positioned as AI-native workforce vs tool

**Concepts Applied**:
- Chain-of-Thought (30-day strategy logic)
- Zero-shot (positioning without examples)
- ReAct Pattern (reason why colleges need this → act with outreach)
- Multi-Agent (content agent + outreach agent + analytics agent)
- Tool Calling (email API, LinkedIn API, analytics)

---

### Case Study 2: RxGPT Health — Investor Narrative Rebuild

**Situation**: Investor deck read like US hospital OS; actual product was India-UAE AI receptionist  
**Task**: Rebuild narrative for investor confidence  
**Action**: New 18-slide deck (navy/teal palette) + companion sales deck with ROI/compliance/market-specific tracks  
**Result**: Clear positioning for independent clinics; fixed chart corruption bug

**Concepts Applied**:
- Context Window (enough tokens to show full clinic workflow)
- Hallucination (removed false claims about hospital integration)
- RAG (retrieved clinic use cases as proof points)
- Fine-tuning (customized pitch for India vs UAE markets)
- LLM-as-Judge (validated deck clarity before launch)

---

### Case Study 3: DIGIX — 30-Day, 3-Platform Content Calendar

**Situation**: Needed coordinated multi-goal GTM across 6 Gethired businesses  
**Task**: Build 30-day calendar (LinkedIn, Instagram, Facebook) with 4 strategic goals  
**Action**: Built branded visual template + 30 pieces of content + 6-touch outreach sequences  
**Result**: Consistent 3-platform presence; enforced brand rules (no emojis, max 3 hashtags, CTA on every post)

**Concepts Applied**:
- Multi-Agent Orchestration (content agent → posting agent → analytics agent)
- Temperature (0.7 for creative posts)
- Chain-of-Thought (goal → theme → platform → format → copy)
- Tool Calling (Instagram API, LinkedIn API, scheduling API)
- Prompt Injection (guardrails: enforce brand rules on every post)

---

### Case Study 4: LeadVault AI — 76K Lead Database Consolidation

**Situation**: Multiple lead sources fragmented; no unified scoring  
**Task**: Consolidate 76K contacts + build intent scoring  
**Action**: Built Python/GraphQL pipeline (Product Hunt API) + 16-sheet master file + scoring logic  
**Result**: 76K contacts scored by intent (funding + hiring + engagement signals)

**Concepts Applied**:
- RAG (retrieve from multiple sources)
- Vector Database (Weaviate for intent matching)
- Hybrid Search (intent vector + keyword search)
- Chunking Strategy (company + contacts per chunk)
- Reranking (re-score by purchase intent confidence)
- Multi-Agent (sourcing agent + filtering agent + export agent)

---

### Case Study 5: Hemraj Group — 13-Agent Pricing Orchestration

**Situation**: Manual pricing decisions created bottlenecks  
**Task**: Automate pricing across forecasting + procurement + sales  
**Action**: Built 13-agent system (pricing → forecasting → procurement → quality → sales → logistics → market intelligence)  
**Result**: Real-time pricing decisions, continuous optimization

**Concepts Applied**:
- Transformer (parallel reasoning across 13 agents)
- Multi-Agent Orchestration (13 agents with handoffs)
- ReAct Pattern (reason pricing logic → act on market)
- Chain-of-Thought (show pricing calculation)
- Memory (seasonal trends memory across seasons)
- Tool Calling (pricing API, inventory DB, forecast model)
- Guardrails (validate prices aren't extreme)

---

## Rapid-Fire Answer Bank (30 Concepts)

| # | Concept | One-Line Answer |
|----|---------|-----------------|
| 1 | Transformer | Parallel token processing via self-attention; why LLMs are feasible at scale. |
| 2 | Self-Attention | Token focuses on all others to build context; foundation of reasoning. |
| 3 | Tokenization | Text split into ~4-char tokens; 1 token ≈ 4 chars. |
| 4 | Embeddings | Text→vector (768+ dims); enables semantic search. |
| 5 | Context Window | Max tokens model sees at once (Claude 200K, GPT-4 128K). |
| 6 | KV Cache | Caching attention to speed up inference; critical for streaming. |
| 7 | Temperature | Sampling parameter (0=consistent, 1=random); set by use case. |
| 8 | Hallucination | AI confidently making stuff up; solved with RAG + validation. |
| 9 | Zero-shot | Prompting without examples; works for simple tasks. |
| 10 | Chain-of-Thought | Prompting step-by-step reasoning; improves complex task accuracy. |
| 11 | RAG | Ground AI in retrieval + generation; prevents hallucination. |
| 12 | Chunking | Split docs into chunks (256-1K tokens); affects retrieval quality. |
| 13 | Vector DB | Embeddings stored in specialized DB; enables fast semantic search. |
| 14 | Cosine Similarity | Finding nearest vectors; core of semantic search. |
| 15 | Hybrid Search | Vector + keyword search; best of both worlds. |
| 16 | Reranking | Re-score retrieved results; improves top-1 accuracy. |
| 17 | Agentic RAG | Agent decides when/what/how to retrieve; mimics expert behavior. |
| 18 | AI Agent | Autonomous system with planning + tools + decisions; scales thinking. |
| 19 | ReAct | Reasoning + Acting loop; makes agent decisions interpretable. |
| 20 | Tool Calling | LLM calls external APIs; connects AI to real systems. |
| 21 | Agent Memory | Long-term context (episodic or semantic); enables learning. |
| 22 | Multi-Agent | Multiple agents coordinating; breaks big problems into subproblems. |
| 23 | MCP | Standard tool interface; how agents discover and use tools. |
| 24 | Fine-tune vs RAG | Three adaptation modes; different cost/accuracy/speed tradeoffs. |
| 25 | LoRA | Efficient fine-tuning (1-2% parameters); 100x cheaper. |
| 26 | QLoRA | LoRA with 4-bit quantization; fine-tune on laptop. |
| 27 | RLHF/DPO | Train to human preferences, not just training data; alignment. |
| 28 | RAGAS | Metrics for RAG quality; tells you if retrieval works. |
| 29 | LLM-as-Judge | Use LLM to evaluate outputs; scales without hiring humans. |
| 30 | Prompt Injection | Malicious input overwrites system prompt; solution is guardrails. |

---

## How to Use This Framework in Your Projects

### For Hemraj (13-Agent Pricing System)
Apply concepts: 1-4 (foundations), 11-20 (retrieval + agents), 21-30 (memory + orchestration)

**Daily Use**:
- ReAct pattern for each pricing decision (reason → act)
- Chain-of-Thought for pricing logic visualization
- Memory for seasonal trends
- Tool Calling for API integration
- Guardrails for price validation

---

### For LeadVault (76K Lead Scoring)
Apply concepts: 11-16 (retrieval), 28-29 (evaluation)

**Daily Use**:
- RAG for multi-source retrieval
- Hybrid search for intent signals
- Reranking by purchase confidence
- RAGAS for scoring quality
- LLM-as-Judge for lead quality

---

### For DIGIX (3-Platform Content Calendar)
Apply concepts: 7 (temperature), 9-10 (prompting), 19-20 (agent patterns), 30 (guardrails)

**Daily Use**:
- Temperature 0.7 for creative copy
- Few-shot examples for brand consistency
- ReAct for content planning
- Tool Calling for API posting
- Guardrails for brand rules

---

### For RxGPT (Clinical AI)
Apply concepts: All 30 (most complex system)

**Daily Use**:
- Fine-tuning for clinical reasoning
- RAG for patient records
- ReAct for diagnosis logic
- Memory for patient history
- Guardrails for safety + HIPAA
- LLM-as-Judge for diagnosis confidence

---

### For HireX (20+ Hiring Agents)
Apply concepts: 18-22 (multi-agent), 24-25 (adaptation), 30 (safety)

**Daily Use**:
- Multi-Agent for sourcing + screening + outreach
- Fine-tuning for resume parsing
- Tool Calling for HRIS/ATS APIs
- Memory for candidate history
- Guardrails for compliance

---

### For Fractional CMO (Brand-Aligned Content)
Apply concepts: 7-10 (prompting), 15 (hybrid search), 27 (RLHF for voice alignment)

**Daily Use**:
- Few-shot examples for brand voice
- Temperature for tone variation
- Hybrid search for relevant content
- Tool Calling for social APIs
- Guardrails for brand consistency

---

## Interview Prep: Common Follow-Up Questions

**Q: "You mentioned using ReAct at Hemraj. Walk me through one example."**
A: "Pricing agent reasons: 'Demand is high (40% increase), supply is low (20% decrease), margin target is 15%' → Acts: 'Calculate new price: base × (1 + demand_signal) × (1 + supply_signal) - margin' → Posts to pricing API → Records decision in memory for seasonal pattern tracking."

**Q: "How do you prevent hallucination in LeadVault?"**
A: "Only return retrieved data from vector DB. Never generate lead data. Use Weaviate with source tracking. Run RAGAS metrics weekly. LLM-as-Judge validates every score before export."

**Q: "Why use hybrid search instead of pure vector search?"**
A: "Vector search finds semantic matches (company with 'similar funding journey'). Keyword search finds exact matches ('Series A in 2026'). Together they catch both intent-based and fact-based leads."

**Q: "Multi-agent orchestration sounds complex. How do you debug?"**
A: "Each agent logs reasoning (ReAct pattern). Message passing is explicit (agent A → agent B). Use MCP for tool calls so every call is traceable. Built dashboards to visualize handoffs."

---

This framework is your competitive advantage. Every interview answer is grounded in real work.
