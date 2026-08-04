# Vaibhav Mehta

**Full-stack developer building AI-powered systems that solve real problems at scale.**

Pre-final year Computer Science undergraduate at VIT Vellore. Former Software Engineering Intern at LTIMindtree. IBM Generative AI (Watsonx) certified. Open-source contributor to LangChain.

Actively seeking placements and 6-month internships (PPO track) starting 2027.

---

## About Me

I build backend-heavy, AI-integrated software -- regulatory compliance agents, carbon-aware inference routers, browser-level security tools, and adaptive learning platforms. My work sits at the intersection of applied AI/ML and production software engineering: RAG pipelines, agentic architectures, microservice design, and real-time streaming systems.

At LTIMindtree, I architected a billing microservice with circuit breaker fault tolerance and built an autonomous compliance agent that compressed 3-6 weeks of manual regulatory review into under 10 minutes. Outside of work, I focus on systems where AI creates measurable impact -- reducing carbon emissions by 93% per AI inference request, or detecting data leaks in real-time before they leave the browser.

I write primarily in Java, Python, and TypeScript. I care about clean architecture, thorough documentation, and shipping software that works under real-world constraints.

---

## Selected Projects

### Internship Work (LTIMindtree, May-Jul 2026)

**[AgentReg](https://github.com/vaibhav585/agentreg)** -- Autonomous Regulatory Compliance Agent
- 4-stage agentic pipeline that extracts obligations from regulatory circulars, searches bank policy documents via RAG (ChromaDB + MiniLM embeddings), identifies compliance gaps, and drafts remediation amendments
- Reduced compliance review time from 3-6 weeks to under 10 minutes; extracted 37 obligations and drafted 36 policy amendments from a single RBI circular
- Python, FastAPI, LLaMA 3.1 (Groq), ChromaDB, Pydantic v2, Server-Sent Events

**[BillFlow](https://github.com/vaibhav585/BillFlow)** -- Microservice-Based Billing System
- Two-service architecture separating business logic (Billing Service) from persistence (Data Pool Service), with REST APIs for invoicing, payments, and customer management
- Circuit breaker pattern for fault-tolerant inter-service communication; BigDecimal precision for audit-grade tax calculations; client-side PDF invoice generation
- Java 17, Spring Boot, MySQL, Hibernate/JPA, Resilience4j, Swagger/OpenAPI

---

### Personal Projects

**[CodeCarbonOps](https://github.com/vaibhav585/CodeCarbonOps)** -- Carbon-Aware AI Inference Routing
- Closed-loop routing system that distributes LLM inference workloads across 15 global cloud regions using real-time grid carbon intensity telemetry from ElectricityMaps
- Thompson Sampling for adaptive server selection; Holt-Winters forecasting for carbon intensity prediction; automatic model downgrading (e.g. GPT-4o to GPT-4o-mini) when grid intensity exceeds thresholds
- Achieved up to 93% reduction in per-request CO2 emissions and 68.8% energy savings through model auto-selection
- Python, FastAPI, React, SQLite, ElectricityMaps API

**[ShadowLeak](https://github.com/vaibhav585/ShadowLeak)** -- Browser Extension for AI Data Exfiltration Prevention
- On-device browser extension that intercepts and inspects text before it is sent to AI chatbots (ChatGPT, Claude, Gemini, Perplexity), detecting secrets, credentials, and PII
- Two-layer detection: regex + Shannon entropy for structured secrets (API keys, JWTs, credit cards), and a quantized DistilBERT NER model (via transformers.js + ONNX Runtime) for unstructured PII -- all running locally with zero telemetry
- Improved combined detection recall from 0.021 (regex-only) to 1.000 (fused engine) across structured, clean PII, and adversarial PII test slices
- JavaScript, transformers.js, ONNX Runtime Web, Chrome Extensions API

**[EduEase](https://github.com/vaibhav585/EduEase-ai-adaptive-assistant)** -- Adaptive AI Learning System for Neurodivergent Students
- Attention-aware TTS reader with word/sentence-level playback, configurable pacing (50-500 WPM), and autopause via webcam distraction detection; multilingual content translation (English to Hindi/Tamil)
- Production RAG pipeline (LangChain, FAISS, BAAI/bge-reranker-base CrossEncoder) with parent-child chunking and per-session memory for context-aware Q&A grounded in uploaded course material
- Real-time attention tracking via MediaPipe FaceLandmarker (478-point landmarks, head-pose estimation, eye-closure blendshapes) feeding a teacher analytics dashboard
- React, FastAPI, LangChain, FAISS, MediaPipe, WebGazer.js

---

### Open Source

**[LangChain](https://github.com/vaibhav585/langchain)** -- Contributed a fix for 400 BadRequestErrors when passing synthetic AIMessages to the OpenAI Responses API. The issue was that LangChain's `create_text_block()` generates internal `lc_` IDs, but OpenAI strictly requires `msg_` prefixed IDs. ([PR #39113](https://github.com/langchain-ai/langchain/issues/39113))

---

## Tech Stack

**Languages:** Java, Python, JavaScript, TypeScript, C/C++, SQL

**Frameworks and Backend:** Spring Boot, FastAPI, React, Node.js, Express.js, Flask, REST APIs, Microservices

**AI/ML:** LLMs, RAG, LangChain, Prompt Engineering, HuggingFace Transformers, spaCy, FAISS, ChromaDB

**Databases and Cloud:** MySQL, MongoDB, AWS (EC2, RDS), Docker, Git, CI/CD

---

## Contact

- [LinkedIn](https://www.linkedin.com/in/vaibhavmhta/)
- [Portfolio](https://vaibhav-portfolio-lilac.vercel.app)
- [Email](mailto:mehta16vaibhav@gmail.com)
