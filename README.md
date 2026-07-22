Hi there! 👋

I'm **Chengzha (Eric) Zhou**, a Master's student in **Electrical and Computer Engineering (ECE)** at **Johns Hopkins University**. I focus on **backend engineering, AI agents, RAG systems, and database-backed applications**, and I'm currently seeking **Software Development Engineer (SDE)** internship and new graduate full-time opportunities.

[![Resume](https://img.shields.io/badge/Resume-View%20PDF-2563EB?style=for-the-badge&logo=adobeacrobatreader&logoColor=white)](./assets/Chengzha_Zhou_Resume.pdf)

---

## 🚀 Featured Projects

### 🩺 [Medical RAG Agent](https://github.com/Ericzcz/Medical_RAG_AGENT)

A production-style medical AI assistant that combines Retrieval-Augmented Generation (RAG), ReAct reasoning, intent routing, memory systems, and structured medical record workflows.

**Highlights**

- Built a Medical RAG Agent with FastAPI, ReAct planning, intent routing, and confidence-driven decision policy, orchestrating **4 specialized skills** for local medical QA, web search, medical record insertion, and field-level medical record retrieval.
- Built a local medical RAG pipeline over **72,877 retrieval chunks** from **11,274 XML files** and **16,407 QA documents**, improving **Recall@5 by 9.4 percentage points**, **Precision@5 by 2.0 percentage points**, and **Hit@5 from 84.0% to 100.0%** with contextual query rewriting, Milvus vector search, BM25 hybrid retrieval, and reranking.
- Designed Redis-backed short-term memory with sliding-window retention and rolling LLM summarization, reducing prompt memory tokens by **61.9%** from **737 to 281 tokens** while preserving multi-turn conversational context.
- Built a long-term memory system with LLM-based memory extraction, `skip / merge / create` update decisions, Redis record storage, and Milvus semantic recall for personalized cross-session responses.
- Developed a PostgreSQL medical record module with **2 normalized tables** and **3 custom indexes**, enabling structured insertion and field-level retrieval of allergies, medications, symptoms, diagnoses, procedures, and vitals.
- Implemented async memory-aware agent endpoints, achieving **4.5x higher throughput** under **10 concurrent multi-user agent requests** in local benchmarks.

**Tech Stack**

Python • FastAPI • OpenAI API • Milvus • Redis • PostgreSQL • Celery • Docker • Prometheus/Grafana

---

### 🛒 [E-Commerce Platform](https://github.com/Ericzcz/E-Commerce-Platform)

A high-concurrency e-commerce platform providing merchant information search, flash-sale coupons, and intelligent customer service.

**Highlights**

- Built a Redis Cache-Aside pipeline with cached null values, logical expiration, Redisson distributed locks, and asynchronous cache rebuilding to prevent cache penetration and breakdown, eliminating database lookups and reducing **P99 latency by 30.9%** from **43.88 ms to 30.31 ms** across **10,000 warmed-up queries** under **100 concurrent requests**.
- Built a two-level caching layer with Caffeine and Redis, using a Redis Lua sliding window to dynamically detect hot keys and promote frequently accessed data into local memory, achieving a **100% cache hit rate**, increasing throughput by **30.4%** from **6,313.59 to 8,232.77 QPS**, and eliminating Redis lookups in a warmed-up single-hot-key benchmark.
- Developed a Redis Lua flash-sale pipeline that atomically validates purchase eligibility, reserves inventory, and enforces one order per user before asynchronously creating orders through Redis Streams, reaching **3,668.06 QPS** with **1,000 unique users**, **100 concurrent requests**, and **200 vouchers** without overselling or duplicate orders.
- Designed a reliable Redis Stream consumer workflow with consumer groups, idempotent processing, acknowledgments, pending-message recovery, retries, and dead-letter handling, reducing flash-sale API **P99 latency by 83.2%** from **408.81 ms to 68.59 ms** while processing **309.15 orders per second**.
- Implemented a Spring scheduled order lifecycle workflow to batch-close expired unpaid orders, restore inventory, and resolve payment-cancellation races through compare-and-set status transitions, producing **zero invalid order states across 100 concurrency tests** and closing expired orders within **60 seconds**.

**Tech Stack**

Redis • Caffeine • Lua • Spring Task • Bloom Filter • Message Queue

---

## 💻 Technical Skills

**Languages:** Java, Python, C/C++, SQL  
**Backend:** FastAPI, Spring Boot, REST APIs, PostgreSQL, MySQL, Redis  
**AI / LLM:** RAG, AI Agents, OpenAI API, Milvus, Prompt Engineering  
**Tools:** Docker, Git, Celery, Playwright, Prometheus, Grafana

---

## 📫 Contact

- Email: [Ericzcz2025@gmail.com](mailto:Ericzcz2025@gmail.com)
- LinkedIn: [linkedin.com/in/eric-zcz](https://linkedin.com/in/eric-zcz)
- GitHub: [github.com/Ericzcz](https://github.com/Ericzcz)
