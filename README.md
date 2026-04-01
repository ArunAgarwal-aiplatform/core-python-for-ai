# Python Foundations for AI Platform Engineering ⚙️🤖

This repository contains my foundational Python projects, explicitly tailored toward building the skills required for **AI Platform Engineering**. 

To build scalable AI systems, deploy LLMs, and manage MLOps pipelines, you first need a flawless understanding of core Python engineering, memory management, and backend logic. I am mastering these concepts by building medium-to-hard infrastructure-adjacent CLI tools, high-throughput data pipelines, and distributed system mockups from scratch.

## 🏗️ Project Architecture (Phase 1: Core Python)

This is Phase 1 of my engineering journey. Each phase tackles a specific Python fundamental required for backend and AI operations, proven through complex, industry-relevant architecture projects:

| # | Engineering Concept | Applied Infrastructure Projects | AI Platform Relevance |
|---|---|---|---|
| 01 | **Variables & Type Safety** | <ul><li>[Config-Driven API Rate Limiter](./01-variables/config-rate-limiter)</li><li>[Pydantic LLM Request Validator](./01-variables/pydantic-validator)</li><li>🔥 **[Distributed Token KV Store Mockup](./01-variables/token-kv-store)**</li><li>[Hardware VRAM Simulator](./01-variables/vram-simulator)</li></ul> | Managing global state for distributed rate limiting, enforcing strict schema validation on incoming API requests, and calculating exact hardware float precision for model loading. |
| 02 | **Control Flow & Guardrails** | <ul><li>[Semantic Request Router](./02-control-flow/semantic-router)</li><li>[Hallucination Regex Detector](./02-control-flow/hallucination-detector)</li><li>🔥 **[Heuristic Prompt Injection Firewall](./02-control-flow/injection-firewall)**</li></ul> | Building complex routing trees to send queries to different models (fast vs. smart), and intercepting malicious/jailbreak prompts before they hit the LLM layer. |
| 03 | **Loops & Batch Processing** | <ul><li>[Concurrent API Request Pipeliner](./03-loops/concurrent-pipeliner)</li><li>[Circuit Breaker & Backoff Engine](./03-loops/circuit-breaker)</li><li>🔥 **[Adaptive Token-Aware Chunker](./03-loops/adaptive-chunker)**</li></ul> | Simulating thousands of asynchronous API calls, implementing production-grade circuit breakers to stop cascading failures, and writing greedy algorithms for RAG document chunking. |
| 04 | **Lists, Dicts & JSON** | <ul><li>[Nested AST Tool Call Parser](./04-data-structures/ast-tool-parser)</li><li>[Streaming JSON Chunk Assembler](./04-data-structures/streaming-assembler)</li><li>🔥 **[In-Memory HNSW Vector Indexer](./04-data-structures/baby-vector-db)**</li><li>[Prompt Template Engine](./04-data-structures/template-engine)</li></ul> | Reconstructing broken/streaming JSON objects from OpenAI's API, and building a "baby Vector DB" from scratch using nested dictionaries and cosine similarity sorting. |
| 05 | **Functions & Pipelines** | <ul><li>[Map-Reduce Log Aggregator](./05-functions/map-reduce-aggregator)</li><li>[Event-Driven Webhook Dispatcher](./05-functions/webhook-dispatcher)</li><li>🔥 **[Decorator Library for LLM Caching](./05-functions/llm-caching-decorators)**</li></ul> | Writing higher-order functions and Python decorators to automatically cache identical LLM queries, saving compute costs and reducing latency. |
| 06 | **OOP & State Management** | <ul><li>[Sliding-Window Memory Cache](./06-oop/sliding-window-memory)</li><li>[Distributed Actor-Model Chat Manager](./06-oop/actor-chat-manager)</li><li>🔥 **[Multi-Agent Delegation Framework](./06-oop/agent-delegation-framework)**</li></ul> | Managing complex conversational state across multiple concurrent users, and using Object-Oriented patterns to orchestrate autonomous agents that assign tasks to each other. |

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
