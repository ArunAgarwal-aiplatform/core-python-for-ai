# Python Foundations for AI Integration & LLM Development ⚙️🤖

I’m moving from frontend and web/SEO work into Python, backend, and eventually **AI Integration & LLM Development**, and this repo is my way of learning out loud. Instead of just calling an LLM API a few times and saying “I know AI,” I want to understand how these models actually fit into real products—how they connect to APIs, databases, web data, and user flows.[web:26][web:31]

To get there, I’m using Python to build small, focused projects that look like real, everyday engineering tasks: estimating costs, cleaning and chunking text, validating inputs, handling failures, and wiring components into simple pipelines. I’m also using a bit of my past web/SEO experience to build medium-level web data projects that could later be useful for RAG-style and search-style systems.

Right now I don’t know everything about AI systems or infrastructure. I’m learning it step by step. The idea is simple: pick one core idea at a time (like working with JSON, handling errors, or processing text), and build a tiny project around it that I can actually run, break, and improve.

Over time, I want these skills to stack into something bigger: REST APIs, data pipelines, LLM integrations, RAG, and agent-style workflows. This repository is **Phase 1** of that journey—using core Python to get ready for more serious backend and LLM work in the future.

---

---

## 🏗️ Project Architecture (Phase 1 – Core Python Mastery)

| # | Progression Level | Headline Project + Core Projects | What This Level Actually Taught Me |
|---|-------------------|-------------------------------|-----------------------------------|
| **01** | **Level 1: Math & Visible Output**<br>*(Functions, math, string ops, file IO, loops)* | <ul><li>🌟 **[Meeting Cost Ticker](./level-1/meeting-cost-ticker)** *(My recruiter showcase)*</li><li>[Loan Amortization Revealer](./level-1/loan-amortization-revealer)</li><li>[Commit Message Archaeologist](./level-1/commit-message-archaeologist)</li><li>[Benford's Law Fraud Spotter](./level-1/benfords-law-fraud-spotter)</li><li>📈 **[Keyword Cannibalization Detector](./level-1/keyword-cannibalization-detector)**</li><li>[Password Entropy Calculator](./level-1/password-entropy-calculator)</li></ul> | **I finally understood how to make math useful.** Not just calculations, but taking real numbers (salaries, loans, git commits) and turning them into formatted tables, live counters, fraud detection reports that anyone can read instantly. This is where I learned f-strings are magic and loops can do real work. |
| **02** | **Level 2: Structured Data & Decisions**<br>*(Dicts, JSON, pattern matching, routing)* | <ul><li>🌟 **[Weighted Decision Matrix Engine](./level-2/weighted-decision-matrix-engine)** *(My recruiter showcase)*</li><li>[JSON API Schema Differ](./level-2/json-api-schema-differ)</li><li>[Wordle Strategy Engine](./level-2/wordle-strategy-engine)</li><li>[Informal Expense Parser](./level-2/informal-expense-parser)</li><li>📈 **[Search Intent Classifier (Rule-Based)](./level-2/search-intent-classifier-rule-based)**</li><li>[Profile Consistency Validator](./level-2/profile-consistency-validator)</li></ul> | **This is when scripts got smart.** I learned to read messy JSON/text, understand structure through pattern matching, then route data through if/else decision trees. Suddenly my programs could "think" - classify search intent, validate profiles, make optimal Wordle moves. Dicts became my best friend. |
| **03** | **Level 3: Batch Resilience**<br>*(Generators, retry logic, checkpointing, bulk ops)* | <ul><li>🌟 **[Spaced Repetition Flashcard Engine](./level-3/spaced-repetition-flashcard-engine)** *(My recruiter showcase)*</li><li>[Fuzzy Duplicate Detector](./level-3/fuzzy-duplicate-detector)</li><li>[Line-by-Line Text Diff Engine](./level-3/line-by-line-text-diff-engine)</li><li>[Bulk File Time Machine](./level-3/bulk-file-time-machine)</li><li>📈 **[Internal Link Opportunity Scanner](./level-3/internal-link-opportunity-scanner)**</li><li>[Deadline Scheduler Task Optimizer](./level-3/deadline-scheduler-task-optimizer)</li></ul> | **"What if it crashes at item 6,847?" became my mantra.** Generators kept memory flat, checkpoints survived crashes, retry logic handled failures. I stopped writing scripts and started building production batch jobs that process thousands of records safely. This is engineer thinking. |
| **04** | **Level 4: Living Systems**<br>*(Classes, SQLite, decorators, persistent state)* | <ul><li>🌟 **[Personal Finance Engine](./level-4/personal-finance-engine)** *(My recruiter showcase)*</li><li>[Code Complexity Auditor](./level-4/code-complexity-auditor)</li><li>[Local Full-Text Search Engine](./level-4/local-full-text-search-engine)</li><li>[Interview Prep Tracker](./level-4/interview-prep-tracker)</li><li>📈 **[SEO Rank Volatility Tracker](./level-4/seo-rank-volatility-tracker)**</li><li>[Habit Streak Engine with Analytics](./level-4/habit-streak-engine-with-analytics)</li></ul> | **I built things that actually live between runs.** Classes with SQLite persistence, decorators for metrics/logging, computed properties that update live. Restart tomorrow? They remember everything. Close laptop mid-session? Data survives. These became tools I use daily. |
| **05** | **Level 5: Senior Engineer Architecture**<br>*(OOP systems, parsers, simulations, frameworks)* | <ul><li>🌟 **[Mini Expression Language Interpreter](./level-5/mini-expression-language-interpreter)** *(My recruiter showcase)*</li><li>[Pure Python Graph Engine](./level-5/pure-python-graph-engine)</li><li>[Discrete Event Simulator](./level-5/discrete-event-simulator)</li><li>[Rule-Based Dialogue Engine](./level-5/rule-based-dialogue-engine)</li><li>📈 **[Content Cluster Architect](./level-5/content-cluster-architect)**</li><li>[Plugin Architecture Framework](./level-5/plugin-architecture-framework)</li></ul> | **Architecture that makes seniors nod in recognition.** Custom parsers, graph traversal, event simulation, plugin systems. These aren't toys - they're the exact patterns behind production systems at scale. Recruiters see Level 5 and know I can handle complex architecture. |

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
