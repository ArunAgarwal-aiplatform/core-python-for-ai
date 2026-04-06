# Python Foundations for AI Integration & LLM Development ⚙️🤖

I’m moving from frontend and web/SEO work into Python, backend, and eventually **AI Integration & LLM Development**, and this repo is my way of learning out loud. Instead of just calling an LLM API a few times and saying “I know AI,” I want to understand how these models actually fit into real products—how they connect to APIs, databases, web data, and user flows.[web:26][web:31]

To get there, I’m using Python to build small, focused projects that look like real, everyday engineering tasks: estimating costs, cleaning and chunking text, validating inputs, handling failures, and wiring components into simple pipelines. I’m also using a bit of my past web/SEO experience to build medium-level web data projects that could later be useful for RAG-style and search-style systems.

Right now I don’t know everything about AI systems or infrastructure. I’m learning it step by step. The idea is simple: pick one core idea at a time (like working with JSON, handling errors, or processing text), and build a tiny project around it that I can actually run, break, and improve.

Over time, I want these skills to stack into something bigger: REST APIs, data pipelines, LLM integrations, RAG, and agent-style workflows. This repository is **Phase 1** of that journey—using core Python to get ready for more serious backend and LLM work in the future.

---

## 🏗️ Project Architecture (Phase 1)

I’ve organized the projects by **level**, from basic scripts up to small orchestration-style experiments.  
Each level has 5 projects: a mix of general backend-style practice plus one project that uses web/page data (where my past experience helps).

The names are intentionally simple and descriptive so anyone scanning the repo can quickly understand what each thing does.

---

### Level 1 – Core Scripting & I/O  
_Focus: functions, math, basic logic, clean console output_

| Project | Description |
|--------|-------------|
| [Cloud API Cost Estimator](./level-1/cloud-cost-estimator) | Estimates the total cost of an LLM/API run using token prices and usage, and prints a clear cost breakdown. |
| [Environment Config Validator](./level-1/env-config-validator) | Loads a few mock config values (keys, timeouts, flags) and checks for missing, empty, or wrong-type settings. |
| [LLM Token Budget Calculator](./level-1/token-calculator) | Starts from a fixed budget and calculates how many tokens or requests fit within that cost limit. |
| [Text Cleaning Utility](./level-1/text-cleaner) | Normalizes raw text by trimming whitespace, removing junk characters, and preparing it for later embedding or storage. |
| 📈 [RAG Crawler Budget Tracker](./level-1/crawl-budget-tracker) | Uses rough page-size and URL counts to estimate how large a basic document crawl will be in MB/GB for a future RAG system. |

---

### Level 2 – Data Parsing & Safety Checks  
_Focus: dictionaries, JSON, routing, simple guard logic_

| Project | Description |
|--------|-------------|
| [API Rate Limit Handler](./level-2/rate-limit-handler) | Simulates hitting a rate limit and shows how a script can pause, back off, or slow itself down. |
| [API Response Extractor](./level-2/response-extractor) | Works with a mock JSON response and pulls out only the useful fields (text, ids, usage) into a clean structure. |
| [Model Fallback Router](./level-2/fallback-router) | Given a simple condition (like error or complexity), chooses between a “fast” or “smart” model as the next step. |
| 📈 [JSON-LD Metadata Extractor](./level-2/schema-injector) | Reads small JSON-LD or page-metadata snippets and extracts titles, URLs, and entity information for later indexing. |
| 🔥 [Semantic Prompt Injection Firewall](./level-2/injection-firewall) | Scans prompts for risky patterns (like “ignore previous instructions”) and flags or blocks them before they’re sent on. |

---

### Level 3 – Batch Work & Resilience  
_Focus: loops, retry logic, bulk processing_

| Project | Description |
|--------|-------------|
| [Dataset Batch Generator](./level-3/dataset-batcher) | Takes a long list of items and splits them into batches ready for bulk processing or batched API calls. |
| [Exponential Backoff Retrier](./level-3/backoff-retrier) | Simulates failing operations and retries them with growing delays to avoid hammering a flaky service. |
| [Pydantic API Request Validator](./level-3/request-validator) | Uses Pydantic models to validate that fake requests have the right fields and types before they “hit” an API. |
| 📈 [High-Throughput Sitemap Ingestor](./level-3/sitemap-extractor) | Walks through a simple sitemap-like structure and collects URLs into batches for later crawling or indexing. |
| 🔥 [Context-Aware RAG Chunker](./level-3/rag-chunker) | Splits long documents into overlapping text chunks so they’re easier to search and feed into retrieval systems. |

---

### Level 4 – State, Quality & Caching  
_Focus: light state management, scoring, reuse and optimization_

| Project | Description |
|--------|-------------|
| [DB Connection Pooler](./level-4/connection-pooler) | Pretends to manage a small pool of reusable “connections” instead of creating a new one for every request. |
| [Sliding-Window Memory Manager](./level-4/sliding-window-memory) | Keeps only the most recent messages in a fake chat history to mimic a limited context window. |
| [Streaming JSON Chunk Assembler](./level-4/streaming-assembler) | Simulates receiving partial JSON/text chunks and rebuilds them into one complete response. |
| 📈 [RAG Source Quality Scorer](./level-4/source-quality-scorer) | Assigns simple scores to documents based on length, noise, or structure to decide which ones are worth indexing. |
| 🔥 [LLM Caching Decorator Library](./level-4/caching-decorators) | Uses decorators to cache repeated “prompt → response” calls so identical queries can be served from memory instead of re-calling a model. |

---

### Level 5 – Orchestration & Small “Agent-Like” Flows  
_Focus: basic OOP, simple orchestration, multi-step and agent-style patterns_

| Project | Description |
|--------|-------------|
| [Async Request Pipeliner Mockup](./level-5/request-pipeliner) | Simulates sending multiple fake requests and handling them in a simple, pipelined or concurrent style. |
| [Agentic Tool Call Parser](./level-5/tool-call-parser) | Accepts a structured “tool call” output (like a JSON instruction) and routes it to the right local function. |
| 📈 [Stateful Web-Research Agent](./level-5/stateful-scraper) | Tracks which pages have been “visited” in a small browsing session and records simple notes per page. |
| 🔥 [In-Memory Baby Vector DB](./level-5/baby-vector-db) | Stores text alongside small mock “vectors” and performs a toy similarity search over them. |
| 🔥 [Multi-Agent Delegation Framework](./level-5/multi-agent-framework) | Models a tiny system where two or more “agents” pass tasks and messages between each other to complete a goal. |

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
