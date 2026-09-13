<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:1e3a8a&height=200&section=header&text=Jeneesh%20Surani&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=AI%20Engineer%20%7C%20Agentic%20Systems%20%26%20LangGraph&descAlignY=55&descSize=18" width="100%"/>

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&pause=1000&color=38BDF8&center=true&vCenter=true&width=600&lines=M.Sc.+AI+%26+Robotics+%40+Hof+University;Building+LangGraph+multi-agent+systems;Red-teaming+my+own+MCP+agent;Two+years+of+backend+dev+before+AI" alt="Typing SVG" /></a>

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://ai-portfolio-6u12.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/jeneesh-surani-ai)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jeneeshsurani@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Jeneesh1014)

</div>

<br>

## About me

I'm doing my M.Sc. in AI and Robotics at Hof University. Before that I spent two years writing backend code for a living, FastAPI, Node.js, Spring Boot, shipping features that had to actually survive production, not just a demo.

That's the lens I bring to AI work now. I'd rather ship an agent that fails safely under a real attack than one that looks impressive for five minutes on a call.

- 📍 Plauen, Saxony, Germany
- 🟢 Open to AI Engineer, Working Student, and internship roles
- 🎓 M.Sc. AI & Robotics, Hof University (2026 to 2027)

<br>

## What I'm building right now

### 🛡️ [Safe MCP Agent](https://github.com/Jeneesh1014/safe-mcp-agent) — still in progress, scaffolding done, core build underway

MCP is quickly becoming the default way agents talk to real company tools, and that opens a new attack surface: an agent can be tricked into calling the wrong tool or leaking data through a normal message, or even through poisoned data it retrieves. So I'm building three things at once. An agent that connects to mock enterprise tools over MCP. A guardrail layer that checks every tool call across five layers before it's allowed to run. And a separate evaluation harness, `mcp-guardeval`, that reads the traces afterward and scores how many attacks actually got through, using real SAFE-MCP technique IDs rather than my own guesswork.

It asks for human approval before any destructive action and shows a live diff of what a tool call would actually change before it runs.

`LangGraph` `MCP` `Ollama` `Pydantic` `OpenTelemetry` `Pytest`
So far: 100% of tested destructive actions get blocked, and it's built against the current MCP v1.0 spec.

<br>

## Featured projects

| Project | What it does | Stack | Result |
|---|---|---|---|
| 🏦 [Agentic-AML-Explainability](https://github.com/Jeneesh1014/Agentic-AML-Explainability) | Multi-agent AML analysis pipeline testing whether a quantized model still holds a strict, audit-style output format | LangGraph, Qwen 2.5 7B, Pydantic, Ollama | 100% schema compliance at 4-bit across 20/20 test cases, €0 cloud cost |
| 🔎 [Intelligent Research Agent](https://github.com/Jeneesh1014/ai-agent-tools) | Agent that decides per question whether to search local docs, the live web, or both | LangGraph, Groq, ChromaDB, Tavily, Cohere, Langfuse | 100% routing accuracy on my eval set, 41 mocked Pytest tests, CI passing |
| 📄 [Ask My Docs](https://github.com/Jeneesh1014/rag-docs-assistant) | Production-style RAG system over AI/ML papers with cited answers | Groq, ChromaDB (BM25 + dense), Cohere rerank, Ragas | 0.73 faithfulness, 0.81 context precision, CI blocks deploys below 0.70 |
| 🧪 Hausmeister Eval Toolkit *(private repo)* | Local benchmarking of cold-start latency and quantization trade-offs on Apple Silicon | Python, Ollama, Pytest | 4 models benchmarked, full CI matrix across Python 3.11 to 3.13 |
| ⛳ [OpenAI Parameter Golf](https://github.com/Jeneesh1014/parameter-golf) | Teacher-student knowledge distillation under a tight parameter budget | PyTorch, AdamW | ~75% compression, tested against GSM8K |

<br>

## Academic research

**Model Compression for Transformer-Based NLP Models** compares Knowledge Distillation against Quantization across BERT-family and large-scale models, drawing on 18 sources.

**A Survey of Weighted Averaging Methods in LLM Model Merging** traces the line from Model Soups and SWA to Task Arithmetic, TIES-Merging, DARE, and AdaMerging.

<br>

## Tech stack

**AI & agent systems**
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square) ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6F00?style=flat-square) ![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square) ![MCP](https://img.shields.io/badge/Model_Context_Protocol-4B5563?style=flat-square)

**Evaluation & observability**
![Ragas](https://img.shields.io/badge/Ragas-6D28D9?style=flat-square) ![Langfuse](https://img.shields.io/badge/Langfuse-0EA5E9?style=flat-square) ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white) ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

**Backend & apps**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)

**Databases**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

**Cloud & DevOps**
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Languages**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

<br>

## GitHub stats

<div align="center">
<img height="165" src="https://github-readme-stats-rickstaa.vercel.app/api?username=Jeneesh1014&show_icons=true&theme=tokyonight&hide_border=true" />
<img height="165" src="https://github-readme-stats-rickstaa.vercel.app/api/top-langs/?username=Jeneesh1014&layout=compact&theme=tokyonight&hide_border=true" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Jeneesh1014&theme=tokyonight&hide_border=true" />
</div>

<br>

## Currently exploring

Agent security and guardrail design, MCP evaluation frameworks, LLM model merging, and quantization trade-offs for edge deployment.

<br>

## Reach me

📧 [jeneeshsurani@gmail.com](mailto:jeneeshsurani@gmail.com) · 💼 [LinkedIn](https://linkedin.com/in/jeneesh-surani-ai) · 🌐 [Portfolio](https://ai-portfolio-6u12.vercel.app)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0f172a&height=100&section=footer" width="100%"/>
