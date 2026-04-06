# Python Foundations for AI Integration & LLM Development ⚙️🤖

I’m moving from frontend and web/SEO work into Python, backend, and eventually **AI Integration & LLM Development**, and this repo is my way of learning out loud. Instead of just calling an LLM API a few times and saying “I know AI,” I want to understand how these models actually fit into real products—how they connect to APIs, databases, web data, and user flows.[web:26][web:31]

To get there, I’m using Python to build small, focused projects that look like real, everyday engineering tasks: estimating costs, cleaning and chunking text, validating inputs, handling failures, and wiring components into simple pipelines. I’m also using a bit of my past web/SEO experience to build medium-level web data projects that could later be useful for RAG-style and search-style systems.

Right now I don’t know everything about AI systems or infrastructure. I’m learning it step by step. The idea is simple: pick one core idea at a time (like working with JSON, handling errors, or processing text), and build a tiny project around it that I can actually run, break, and improve.

Over time, I want these skills to stack into something bigger: REST APIs, data pipelines, LLM integrations, RAG, and agent-style workflows. This repository is **Phase 1** of that journey—using core Python to get ready for more serious backend and LLM work in the future.

---

## 🏗️ Project Architecture (Phase 1 – Core Python → LLM & Backend)

| # | Progression Level | Applied Projects | Why This Matters for LLM & Backend Work |
|---|-------------------|------------------|------------------------------------------|
| **01** | **Level 1: Core Scripting & I/O**<br>*(Functions, math, basic logic)* | <ul><li>[Cloud API Cost Estimator](./level-1/cloud-cost-estimator)</li><li>[Environment Config Validator](./level-1/env-config-validator)</li><li>[LLM Token Budget Calculator](./level-1/token-calculator)</li><li>[Text Cleaning Utility](./level-1/text-cleaner)</li><li>📈 **[RAG Crawler Budget Tracker](./level-1/crawl-budget-tracker)**</li></ul> | Learning to work with numbers, types, and simple functions while thinking in terms of real constraints: API cost, safe config loading, token limits, and how much data a basic crawl or ingestion job will actually produce. |
| **02** | **Level 2: Data Parsing & Safety Checks**<br>*(Dicts, JSON, routing, guard logic)* | <ul><li>[API Rate Limit Handler](./level-2/rate-limit-handler)</li><li>[API Response Extractor](./level-2/response-extractor)</li><li>[Webhook Payload Builder](./level-2/webhook-builder)</li><li>[Model Fallback Router](./level-2/fallback-router)</li><li>📈 **[JSON-LD Metadata Extractor](./level-2/schema-injector)**</li><li>🔥 **[Semantic Prompt Injection Firewall](./level-2/injection-firewall)**</li></ul> | Practicing how real services talk in JSON, how to pull out only what you need, how to route between different “modes” or models, and how to add simple safety checks so bad inputs or prompts don’t go straight into a model. |
| **03** | **Level 3: Batch Operations & Resilience**<br>*(Loops, retry logic, bulk processing)* | <ul><li>[Dataset Batch Generator](./level-3/dataset-batcher)</li><li>[Exponential Backoff Retrier](./level-3/backoff-retrier)</li><li>[Pydantic API Request Validator](./level-3/request-validator)</li><li>📈 **[High-Throughput Sitemap Ingestor](./level-3/sitemap-extractor)</li><li>📈 **[Spider-Trap Escape Guardrail](./level-3/spider-trap-guardrail)</li><li>🔥 **[Context-Aware RAG Chunker](./level-3/rag-chunker)</li></ul> | Moving from single requests to many: batching items, retrying failures without attacking a service, validating request shapes, collecting lots of URLs from simple sitemap-style data, avoiding infinite crawl loops, and chopping documents into retrieval-friendly chunks. |
| **04** | **Level 4: State Management & Optimization**<br>*(Light state, caching, aggregation)* | <ul><li>[Map-Reduce Log Aggregator](./level-4/map-reduce-aggregator)</li><li>[DB Connection Pooler](./level-4/connection-pooler)</li><li>[Sliding-Window Memory Manager](./level-4/sliding-window-memory)</li><li>[Streaming JSON Chunk Assembler](./level-4/streaming-assembler)</li><li>📈 **[RAG Source Quality Scorer](./level-4/source-quality-scorer)</li><li>🔥 **[LLM Caching Decorator Library](./level-4/caching-decorators)</li></ul> | Thinking more like someone running a system: summarizing logs, reusing connections, trimming histories to fit in context windows, rebuilding streaming responses, ranking which documents are worth indexing, and caching repeat queries so you don’t pay or wait twice. |
| **05** | **Level 5: Architecture & Orchestration**<br>*(OOP, simple async ideas, agent-like flows)* | <ul><li>[Async Request Pipeliner Mockup](./level-5/request-pipeliner)</li><li>[Agentic Tool Call Parser](./level-5/tool-call-parser)</li><li>[Pipeline Task Runner](./level-5/task-runner)</li><li>📈 **[Stateful Web-Research Agent](./level-5/stateful-scraper)</li><li>🔥 **[In-Memory Baby Vector DB](./level-5/baby-vector-db)</li><li>🔥 **[Multi-Agent Delegation Framework](./level-5/multi-agent-framework)</li></ul> | Pulling everything together into small “systems”: simulating concurrent or pipelined requests, interpreting tool-call style outputs, running multi-step flows, tracking what a tiny “research agent” has seen, prototyping a toy vector search, and exploring simple multi-agent handoff patterns. |
---

## 🧭 Bigger Roadmap (Beyond This Repo)

Phase 1 is about **core Python** and getting comfortable with scripts, data, and small flows.  
After that, my plan is roughly:

1. **Core Python** (this repo)  
2. **FastAPI & REST APIs** – turn some of these scripts into simple HTTP endpoints  
3. **Data & Storage** – use Pandas and basic SQL to store, query, and analyze the data these tools produce  
4. **LLM & AI APIs** – start calling real LLM APIs, reusing the patterns I practiced here (costs, cleaning, batching, retries)  
5. **RAG & Agent Flows** – add retrieval over my own data and experiment with small agent-like workflows  
6. **Portfolio & Jobs** – polish the best projects into clean, documented examples I can show to hiring managers and senior engineers[web:22][web:28]

---

## 🛠️ Current Stack

- Frontend & web background  
- Python 3.x  
- Git & VS Code  

## 💡 About This Repo

This is a learning-focused space. I expect the code and structure to improve as I learn more. If you’re reviewing this and see something I could do better, I’m very open to suggestions.
