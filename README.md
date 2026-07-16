Hi there! 👋

I'm **Chengzha (Eric) Zhou**, a Master's student in **Electrical and Computer Engineering (ECE)** at **Johns Hopkins University**. I focus on **backend engineering, AI agents, RAG systems, and database-backed applications**, and I'm currently seeking **Software Development Engineer (SDE)** internship and new graduate full-time opportunities.

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

- Prevented cache breakdown for hot Redis keys with logical expiration and distributed locking, while using Bloom filters and cached-null entries to protect against cache penetration.
- Built a two-level cache with Caffeine and Redis that automatically promotes hot data into local memory, achieving a **local-cache hit rate above 99%** and substantially reducing Redis load.
- Maintained cache consistency by invalidating cached data after updates, retrying failed invalidations through a message queue, and using TTL as a fallback.
- Implemented dynamic hotspot detection with Redis sliding windows, sampling statistics, and Lua scripts, improving hotspot-query throughput by **5–10x**.
- Built a Redis- and Lua-based flash-sale workflow that validates purchase eligibility, prevents overselling and duplicate orders, and asynchronously processes inventory deduction and order creation through message-queue consumers.
- Reduced flash-sale response time by **65.2%** while preventing overselling and duplicate purchases.
- Scheduled automatic cancellation of unpaid orders with Spring Task and used optimistic locking to coordinate concurrent payment and order-closing operations.

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
