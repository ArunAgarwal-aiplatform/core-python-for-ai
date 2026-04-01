# Python Foundations for AI Platform Engineering ⚙️🤖

This repository contains my foundational Python projects, explicitly tailored toward building the core backend skills required for **AI Platform Engineering**. 

To build scalable AI systems, deploy Large Language Models (LLMs), and manage production MLOps pipelines, generic Python scripts are not enough. You need a flawless understanding of memory management, strict type safety, concurrency, and API integration. I am mastering these concepts by building infrastructure-adjacent CLI tools, high-throughput data pipelines, and system architecture mockups from scratch.

## 🏗️ Project Architecture (Phase 1: Core Python)

This is Phase 1 of my engineering journey. Each module tackles a specific Python fundamental required for AI operations, proven through a suite of 5 industry-relevant projects:

| # | Engineering Concept | Applied Infrastructure Projects | AI Platform Relevance |
|---|---|---|---|
| 01 | **Variables & Type Safety** | <ul><li>[Cloud API Cost Estimator](./01-variables/cloud-cost-estimator)</li><li>[LLM Token Budget Calculator](./01-variables/token-calculator)</li><li>[Environment Config Validator](./01-variables/env-config-validator)</li><li>[Hardware VRAM Simulator](./01-variables/vram-simulator)</li><li>🔥 **[Quantization Precision Analyzer](./01-variables/quantization-analyzer)**</li></ul> | Managing exact float precision for compute costs, securely loading environment variables, and simulating memory footprint differences between FP16, INT8, and 4-bit AWQ quantized local models. |
| 02 | **Control Flow & Guardrails** | <ul><li>[Basic Prompt Filter](./02-control-flow/basic-prompt-filter)</li><li>[API Rate Limit Handler](./02-control-flow/rate-limit-handler)</li><li>[Model Fallback Router](./02-control-flow/fallback-router)</li><li>[Pydantic LLM Request Validator](./02-control-flow/request-validator)</li><li>🔥 **[Semantic Prompt Injection Firewall](./02-control-flow/injection-firewall)**</li></ul> | Building complex routing trees (fast vs. smart models), gracefully handling 429 timeouts, enforcing strict data schemas, and using heuristics to deflect adversarial AI "jailbreak" attempts. |
| 03 | **Loops & Batch Processing** | <ul><li>[Log File Anomaly Scanner](./03-loops/log-scanner)</li><li>[Dataset Batch Generator](./03-loops/dataset-batcher)</li><li>[Exponential Backoff Retrier](./03-loops/backoff-retrier)</li><li>[Async Request Pipeliner Mockup](./03-loops/request-pipeliner)</li><li>🔥 **[Context-Aware RAG Chunker](./03-loops/rag-chunker)**</li></ul> | Iterating through massive datasets, managing network retry logic with `while` loops, and writing greedy algorithms with overlapping sliding windows to prepare documents for Vector Databases. |
| 04 | **Lists, Dicts & JSON** | <ul><li>[Prompt Template Engine](./04-data-structures/template-engine)</li><li>[API Response Extractor](./04-data-structures/response-extractor)</li><li>[Streaming JSON Chunk Assembler](./04-data-structures/streaming-assembler)</li><li>[Agentic Tool Call Parser](./04-data-structures/tool-call-parser)</li><li>🔥 **[In-Memory Baby Vector DB](./04-data-structures/baby-vector-db)**</li></ul> | Structuring complex JSON inputs, reconstructing broken streaming payloads from OpenAI, and building a lightweight Vector Indexer from scratch using nested arrays and cosine similarity. |
| 05 | **Functions & Pipelines** | <ul><li>[Text Cleaning Utility](./05-functions/text-cleaner)</li><li>[MLOps Metrics Calculator](./05-functions/metrics-calculator)</li><li>[Webhook Payload Builder](./05-functions/webhook-builder)</li><li>[Map-Reduce Log Aggregator](./05-functions/map-reduce-aggregator)</li><li>🔥 **[LLM Caching Decorator Library](./05-functions/caching-decorators)**</li></ul> | Writing modular, pure functions for multi-modal API requests, and engineering custom Python decorators (`@cache_llm`) to intercept identical queries, saving compute and latency. |
| 06 | **OOP & State Management** | <ul><li>[Simple Chat Logger Class](./06-oop/chat-logger)</li><li>[DB Connection Pooler](./06-oop/connection-pooler)</li><li>[Sliding-Window Memory Manager](./06-oop/sliding-window-memory)</li><li>[Pipeline Task Runner](./06-oop/task-runner)</li><li>🔥 **[Multi-Agent Delegation Framework](./06-oop/multi-agent-framework)**</li></ul> | Maintaining conversational context limits across multiple users, abstracting database connections, and using OOP inheritance to orchestrate autonomous AI agents that delegate tasks to one another. |

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
