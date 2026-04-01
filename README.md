# Python Foundations for AI Platform Engineering ⚙️🤖

This repository contains my foundational Python projects, explicitly tailored toward building the core backend skills required for **AI Platform Engineering**. 

When I started my journey into AI Platform Engineering, I quickly realized the role goes way beyond just writing basic Python scripts. It’s really about building the heavy-duty pipelines that allow LLMs to run securely, affordably, and reliably in the real world.

As someone breaking into this space, I know that to eventually handle MLOps and deploy production models, I need a rock-solid grip on the backend fundamentals—things like memory management, strict type safety, concurrency, and web-scale data ingestion.

So, rather than getting stuck in 'tutorial hell,' I’m documenting my learning process here. I'm teaching myself these core concepts by actually building things from scratch, focusing on infrastructure-adjacent CLI tools, high-throughput RAG ingestion pipelines, and system architecture mockups.

## 🏗️ Project Architecture (Phase 1: Core Python)

This is Phase 1 of my engineering journey. Each module tackles a specific Python fundamental required for AI operations, proven through a suite of 6 industry-relevant projects (including cutting-edge AI concepts and AI-driven SEO automation):

| # | Engineering Concept | Applied Infrastructure Projects | AI Platform Relevance |
|---|---|---|---|
| 01 | **Variables & Type Safety** | <ul><li>[Cloud API Cost Estimator](./01-variables/cloud-cost-estimator)</li><li>[LLM Token Budget Calculator](./01-variables/token-calculator)</li><li>[Environment Config Validator](./01-variables/env-config-validator)</li><li>[Hardware VRAM Simulator](./01-variables/vram-simulator)</li><li>📈 **[AI Crawl Budget Variable Tracker](./01-variables/crawl-budget-tracker)**</li><li>🔥 **[Quantization Precision Analyzer](./01-variables/quantization-analyzer)**</li></ul> | Managing float precision for compute costs, allocating exact crawl budgets for programmatic SEO bot traffic, and simulating memory footprint differences for local 4-bit quantized models. |
| 02 | **Control Flow & Guardrails** | <ul><li>[Basic Prompt Filter](./02-control-flow/basic-prompt-filter)</li><li>[API Rate Limit Handler](./02-control-flow/rate-limit-handler)</li><li>[Model Fallback Router](./02-control-flow/fallback-router)</li><li>[Pydantic LLM Request Validator](./02-control-flow/request-validator)</li><li>📈 **[Programmatic 301/404 Status Router](./02-control-flow/status-router)**</li><li>🔥 **[Semantic Prompt Injection Firewall](./02-control-flow/injection-firewall)**</li></ul> | Building complex routing trees, gracefully handling API timeouts, writing conditional logic for bulk SEO URL redirects, and using heuristics to deflect adversarial AI "jailbreak" attempts. |
| 03 | **Loops & Batch Processing** | <ul><li>[Log File Anomaly Scanner](./03-loops/log-scanner)</li><li>[Dataset Batch Generator](./03-loops/dataset-batcher)</li><li>[Exponential Backoff Retrier](./03-loops/backoff-retrier)</li><li>[Async Request Pipeliner Mockup](./03-loops/request-pipeliner)</li><li>📈 **[High-Throughput XML Sitemap Extractor](./03-loops/sitemap-extractor)**</li><li>🔥 **[Context-Aware RAG Chunker](./03-loops/rag-chunker)**</li></ul> | Managing network retry logic with `while` loops, looping through massive sitemaps to feed URLs into AI scrapers, and writing greedy algorithms to chunk documents for Vector Databases. |
| 04 | **Lists, Dicts & JSON** | <ul><li>[Prompt Template Engine](./04-data-structures/template-engine)</li><li>[API Response Extractor](./04-data-structures/response-extractor)</li><li>[Streaming JSON Chunk Assembler](./04-data-structures/streaming-assembler)</li><li>[Agentic Tool Call Parser](./04-data-structures/tool-call-parser)</li><li>📈 **[Dynamic JSON-LD Schema Injector](./04-data-structures/schema-injector)**</li><li>🔥 **[In-Memory Baby Vector DB](./04-data-structures/baby-vector-db)**</li></ul> | Reconstructing broken streaming payloads from OpenAI, structuring deeply nested JSON-LD dictionaries for technical SEO markup, and building a lightweight Vector Indexer using cosine similarity. |
| 05 | **Functions & Pipelines** | <ul><li>[Text Cleaning Utility](./05-functions/text-cleaner)</li><li>[MLOps Metrics Calculator](./05-functions/metrics-calculator)</li><li>[Webhook Payload Builder](./05-functions/webhook-builder)</li><li>[Map-Reduce Log Aggregator](./05-functions/map-reduce-aggregator)</li><li>📈 **[AI Meta-Tag Optimization Pipeline](./05-functions/meta-tag-pipeline)**</li><li>🔥 **[LLM Caching Decorator Library](./05-functions/caching-decorators)**</li></ul> | Writing modular functions to parse and score AI-generated meta descriptions, handling multi-modal API requests, and engineering custom Python decorators to cache identical LLM queries. |
| 06 | **OOP & State Management** | <ul><li>[Simple Chat Logger Class](./06-oop/chat-logger)</li><li>[DB Connection Pooler](./06-oop/connection-pooler)</li><li>[Sliding-Window Memory Manager](./06-oop/sliding-window-memory)</li><li>[Pipeline Task Runner](./06-oop/task-runner)</li><li>📈 **[Stateful AI Web Scraper Class](./06-oop/stateful-scraper)**</li><li>🔥 **[Multi-Agent Delegation Framework](./06-oop/multi-agent-framework)**</li></ul> | Maintaining conversational context limits, building OOP scrapers that track visited URLs and respect `robots.txt`, and orchestrating autonomous AI agents that delegate tasks to one another. |

## 🚀 Future Phases Roadmap
- **Phase 2:** Asynchronous FastAPI & WebSocket Integration (Serving models)
- **Phase 3:** High-Performance Data Manipulation (Pandas, Polars & NumPy)
- **Phase 4:** Docker, Kubernetes & Container Orchestration
- **Phase 5:** MLflow, CI/CD for ML, & MLOps Infrastructure

## 🛠️ Current Tech Stack
- Python 3.x
- Git & Version Control 

## 💡 How to Run
Each project is self-contained. Navigate to the specific project directory and read its local `README.md` for execution instructions and system design architecture.

