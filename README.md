<div align="center">

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&pause=1000&color=38BDF8&center=true&vCenter=true&width=650&lines=M.Sc.+AI+%26+Robotics+%40+Hof+University;Building+LangGraph+multi-agent+systems;Securing+LLM+agents+against+MCP+attacks;Author+of+mcp-guardeval+on+PyPI;Two+years+of+backend+dev+before+AI" alt="Typing SVG" /></a>

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://ai-portfolio-6u12.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/jeneesh-surani-ai)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jeneeshsurani@gmail.com)
[![PyPI](https://img.shields.io/badge/PyPI-mcp--guardeval-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/mcp-guardeval/)

</div>

<br>

## About me

I'm doing my M.Sc. in AI and Robotics at Hof University. Before that I spent two years writing backend and mobile code with FastAPI, Node.js, Spring Boot, and React Native, building and shipping features that had to work beyond a demo.

That's the lens I bring to AI engineering now. My core principle: an AI system is only as good as the tests that prove it works, not the demo that shows it once. I like building systems that are measurable, testable, and safe to run.

* 📍 Plauen, Saxony, Germany
* 🟢 Open to AI Engineer, Generative AI / LLM Engineer, Working Student, and internship roles in Germany
* 🎓 M.Sc. AI & Robotics, Hof University (2026–2027)
* 🗣️ English (C1) · German (B1, improving)

<br>

## Featured projects

### 🛡️ [Safe-MCP-Agent](https://github.com/Jeneesh1014/safe-mcp-agent) · flagship

A local-first enterprise AI agent that covers the full lifecycle of securing an MCP-connected agent: build it, attack it, defend it, and prove the defense works.

Built with LangGraph and FastMCP around a local Llama 3.2 model, the agent connects to mock enterprise tools (customer DB, wiki, Slack). A **five-layer guardrail middleware** sits between the agent and tool execution: input validation, permissions and session budgets, output PII filtering, retrieved-content sanitization, and a final response filter.

The evaluation harness is published as [`mcp-guardeval`](https://pypi.org/project/mcp-guardeval/) on PyPI. It reads OpenTelemetry `gen_ai.*` spans and scores results deterministically (no LLM-as-a-judge), with a pytest plugin (`pytest --agenteval`).

`LangGraph` `MCP` `FastMCP` `Ollama` `Pydantic` `OpenTelemetry` `Pytest`

**Result:** all **7 of 7** catalogued SAFE-MCP attack techniques were deterministically blocked, regardless of model capability. In a 48-run benchmark, Llama 3.2 3B passed 100% of enterprise tasks versus 50% for the 1B model. Runs fully local at $0 API cost.

> *"Model incompetence is not a security control."* Several attacks only failed on the undefended agent because the small model fumbled its tool calls, so enforcement lives in fixed code rules, not in hoping the model isn't smart enough.

---

### 🏦 [Agentic-AML-Explainability](https://github.com/Jeneesh1014/Agentic-AML-Explainability)

Three-agent AML analysis pipeline (Investigator → Explainer → Auditor) testing whether a quantized model can maintain a strict, BaFin-style structured output format, with automatic validation and retry.

`LangGraph` `Qwen 2.5 7B` `Pydantic` `Ollama`

**Result:** 100% schema compliance at 4-bit across 20/20 test cases with €0 cloud cost.

---

### 🔎 [Intelligent Research Agent](https://github.com/Jeneesh1014/ai-agent-tools)

Research agent that decides per question whether to answer from local documents, the live web, or both, with Langfuse tracing on every node.

`LangGraph` `Groq` `ChromaDB` `Tavily` `Cohere` `Langfuse` `Docker`

**Result:** 100% routing accuracy on my evaluation set, 41 fully mocked Pytest tests, CI passing.

---

### 📄 [Ask My Docs](https://github.com/Jeneesh1014/rag-docs-assistant)

Production-style RAG system over AI/ML research papers with hybrid retrieval (BM25 + dense + Cohere rerank), Pydantic-enforced citations, and a Ragas-based CI quality gate.

`Groq` `ChromaDB` `BM25` `Dense Retrieval` `Cohere` `Ragas`

**Result:** 0.73 faithfulness, 0.81 context precision, 52 CI tests, with deploys blocked automatically below a 0.70 faithfulness threshold.

---

### 🧪 Hausmeister Eval Toolkit

Local-first LLM benchmarking framework (Ollama on Apple Silicon) that profiles cold-start vs. warm latency, quantization trade-offs, and rule-constrained reasoning, with all results reproducible from committed raw data.

`Python` `Ollama` `Pytest` `GitHub Actions`

**Finding:** cold-start time follows file size on disk, warm-call time follows model depth. The 8-bit model took about 2× longer to cold-start than the 4-bit one (5.79 s vs. 2.87 s), but the warm gap was only about 30%. *(Private repo.)*

---

### ⛳ [OpenAI Parameter Golf](https://github.com/Jeneesh1014/parameter-golf)

Teacher-student knowledge distillation under a tight parameter budget, trained on FineWeb.

`PyTorch` `AdamW`

**Result:** ~75% compression, tested against GSM8K. A learning exercise on the limits of extreme compression, not a leaderboard entry.

<br>

## Academic research

**Model Compression for Transformer-Based NLP Models** *(March 2026)*
A comparative study of Knowledge Distillation and Quantization (PTQ and QAT) across BERT-family and large-scale models, covering accuracy, size, speed, and scalability. Key takeaway: distillation suits small task-specific models, quantization suits shrinking large general models, and combining both wins at the extreme end.

**A Survey of Weighted Averaging Methods in LLM Model Merging** *(March 2026)*
Traces weight-averaging approaches from Model Soups and SWA through Task Arithmetic, TIES-Merging, DARE, and AdaMerging, plus the theory behind why merging works and where it still breaks.

<br>

## Experience

* **AI Engineer (Independent Projects)**, 03/2026 – present: building and securing LLM agents, from MCP guardrails to RAG evaluation
* **Software Developer, Pathnovo Solutions** (remote), 04/2025 – 07/2025: React Native + TypeScript apps, REST APIs, Socket.IO real-time features, AWS CI/CD with GitHub Actions
* **Software Developer (Intern), CodeLeap InfoTech**, 07/2023 – 04/2025: sole developer on 4 client projects end to end (Figma → frontend → backend → DB → AWS deployment)

<br>

## Tech stack

**AI & agent systems**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)
![FastMCP](https://img.shields.io/badge/FastMCP-4B5563?style=flat-square)
![MCP](https://img.shields.io/badge/Model_Context_Protocol-4B5563?style=flat-square)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F00?style=flat-square)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square)

**Evaluation, observability & security**

![Ragas](https://img.shields.io/badge/Ragas-6D28D9?style=flat-square)
![Langfuse](https://img.shields.io/badge/Langfuse-0EA5E9?style=flat-square)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![SAFE-MCP](https://img.shields.io/badge/SAFE--MCP-red--teaming-B91C1C?style=flat-square)

**Backend & apps**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

<br>

## Awards

* 🏆 **New India Vibrant Hackathon 2023**: Winner (SSIP Gujarat)
* 🥇 **The Maverick Effect AI Challenge 2024**: Top 15 Finalist

<br>

## Currently exploring

Agent security and guardrail design, MCP evaluation frameworks, RAG security, LLM model merging, and quantization trade-offs for edge deployment.

Outside the terminal: Blender hobbyist, learning German.

<br>

## Reach me

📧 [jeneeshsurani@gmail.com](mailto:jeneeshsurani@gmail.com) · 💼 [LinkedIn](https://linkedin.com/in/jeneesh-surani-ai) · 🌐 [Portfolio](https://ai-portfolio-6u12.vercel.app)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0f172a&height=100&section=footer" width="100%"/>
