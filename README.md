# Python Foundations for AI & Backend Projects ⚙️🤖

I’m moving from frontend and web work into Python, backend, and eventually AI/LLM projects. This repo is my way of learning out loud. Instead of just calling an LLM API a few times and saying “I know AI,” I want to understand how these models actually fit into real products—how they connect to APIs, databases, web data, and user flows.[web:26][web:31]

To get there, I’m using Python to build small, focused projects that look like real, everyday engineering tasks: estimating costs, cleaning and chunking text, validating inputs, handling failures, and wiring components into simple pipelines. I’m also using a bit of my past SEO experience to build medium-level web data projects that could later be useful for RAG-style and search-style systems.

Right now I don’t know everything about AI systems or backend infrastructure. I’m learning it step by step. The idea is simple: pick one core idea at a time (like working with JSON, handling errors, or processing text), and build a tiny project around it that I can actually run, break, and improve.

Over time, I want these skills to stack into something bigger: REST APIs, data pipelines, LLM integrations, RAG, and agent-style workflows. This repository is **Phase 1** of that journey—using core Python to become confident enough to build real things later.

---

## 🏗️ Project Architecture (Phase 1)

I’ve organized the projects by **level**, from basic scripts up to small orchestration-style experiments.  
Each level has 5 projects: a mix of general backend-style practice plus one project that uses web/page data (where my past experience helps).

The names are intentionally simple and descriptive so anyone scanning the repo can quickly understand what each thing does.

---

### Level 1 – Core Scripting & I/O  
_Focus: functions, numbers, basic logic, clean console output_

| Project | Description |
|--------|-------------|
| [Cloud Cost Calculator](./level-1/cloud-cost-calculator) | Takes basic pricing and token usage numbers and prints a clear cost breakdown for a hypothetical API run. |
| [Token Budget Planner](./level-1/token-budget-planner) | Starts from a fixed budget and works backwards to how many tokens/operations can fit inside it. |
| [Config Sanity Checker](./level-1/config-sanity-checker) | Loads a few mock “settings” and checks for missing values or obviously wrong types. |
| [Text Hygiene Helper](./level-1/text-hygiene-helper) | Cleans messy text (extra spaces, line breaks, odd characters) to make it friendlier for later processing. |
| 📄 [Web Crawl Size Estimator](./level-1/web-crawl-size-estimator) | Uses a rough page-size estimate and page count to guess how large a simple web crawl might be in MB/GB. |

---

### Level 2 – Data Parsing & Safety Checks  
_Focus: dictionaries, JSON, basic routing, simple guard logic_

| Project | Description |
|--------|-------------|
| [Rate Limit Simulator](./level-2/rate-limit-simulator) | Pretends to call a service repeatedly and shows when and how a script should slow down. |
| [Response Field Picker](./level-2/response-field-picker) | Works with a mock JSON “API response” and extracts only the fields that matter. |
| [Webhook Payload Maker](./level-2/webhook-payload-maker) | Builds small JSON payloads that a backend or third-party service could reasonably consume. |
| [Simple Choice Switchboard](./level-2/simple-choice-switchboard) | Given a few conditions, chooses between “fast”, “safe”, or “detailed” processing modes. |
| 📄 [Page Info Reader](./level-2/page-info-reader) | Reads a tiny JSON blob representing a page (title, url, tags) and prints a human-friendly summary. |

---

### Level 3 – Batch Work & Resilience  
_Focus: loops, retries, working over lists of items_

| Project | Description |
|--------|-------------|
| [Batch Splitter](./level-3/batch-splitter) | Takes a long list of items and splits it into smaller batches that could later be processed in chunks. |
| [Stubborn Request Tamer](./level-3/stubborn-request-tamer) | Simulates failing operations and retries them with increasing delays. |
| [Shape Inspector](./level-3/shape-inspector) | Checks whether each “request” in a list has the keys and basic types it’s supposed to have. |
| [Story Chunker](./level-3/story-chunker) | Splits long text into overlapping segments so no important sentence gets completely cut off. |
| 📄 [Sitemap Link Collector](./level-3/sitemap-link-collector) | Walks through a simple sitemap-like structure and collects URLs into a clean list for later use. |

---

### Level 4 – State, Quality & Caching  
_Focus: remembering a bit of state, scoring, and reuse_

| Project | Description |
|--------|-------------|
| [Log Storyboard](./level-4/log-storyboard) | Reads a bunch of fake “log lines” and builds simple summaries like counts per type or per level. |
| [Connection Toy Pool](./level-4/connection-toy-pool) | Pretends to manage a tiny pool of reusable “connections” instead of creating a new one every time. |
| [Conversation Trimmer](./level-4/conversation-trimmer) | Keeps only the latest messages in a pretend chat history so it doesn’t grow forever. |
| [Drip-Feed Reassembler](./level-4/drip-feed-reassembler) | Simulates receiving text in small chunks and stitches it back into a single complete message. |
| 📄 [Content Signal Scorer](./level-4/content-signal-scorer) | Gives simple scores to short pieces of text (e.g., too short, too cluttered, or good enough) to decide what’s worth keeping. |

---

### Level 5 – Orchestration & Small “Agent-Like” Flows  
_Focus: basic OOP, simple orchestration, multi-step flows_

| Project | Description |
|--------|-------------|
| [Multi-Request Conductor](./level-5/multi-request-conductor) | Takes several fake “jobs” and walks them through a simple pipeline, keeping track of their status. |
| [Tool Output Interpreter](./level-5/tool-output-interpreter) | Accepts a structured “tool result” and decides what the next step in the flow should be. |
| [Mini Workflow Engine](./level-5/mini-workflow-engine) | Runs a chain of small tasks in order, passing results from one step into the next. |
| [Toy Memory Search](./level-5/toy-memory-search) | Stores short snippets and checks which ones are most similar to a simple search query. |
| 📄 [Curious Web Scout](./level-5/curious-web-scout) | Keeps track of a tiny “browsing session”: which pages were visited, which are pending, and avoids revisiting the same link. |

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
