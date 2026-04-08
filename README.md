<h1 align="center">Hi, I'm Shishir Kumar Pathak</h1>
<h3 align="center">Software Engineer focused on AI-backed systems, scalable backends, and real-world constraints</h3>

---

## About Me

I design and build **backend systems and AI-assisted pipelines** where correctness, safety, and real-world constraints matter more than hype.

My work focuses on:
- integrating LLMs into production systems without making them a single point of failure  
- combining deterministic logic with probabilistic models  
- building scalable services with clear decision boundaries and observability  

I’m particularly interested in systems where **wrong decisions are costly** — and how to design around that.

---

## Selected Work

### 🔹 Gmail Cleanup AI — Safety-First Email Decision System

A Gmail triage system designed to **avoid blindly trusting AI** for destructive actions.

#### Problem
Most AI-powered automation assumes the model is reliable enough to act.  
In email systems, a wrong decision (OTP, banking, interview, invoices) leads to a **loss of trust**.

#### Approach
Designed a multi-layer decision pipeline instead of relying on a single model:

- Rule-based classification to protect high-risk emails  
- Vector similarity (`pgvector`) to leverage historical patterns  
- LLM fallback only for low-confidence cases  
- Guardrails to prevent unsafe actions  
- Human-in-the-loop review before execution  

#### Key Trade-offs
- Chose **safety over full automation** → reduced risk but added review friction  
- Limited LLM usage → lower cost and more predictable behavior  
- Accepted partial automation instead of maximizing recall  

#### System Design
- FastAPI backend with modular service layer  
- PostgreSQL + `pgvector` for similarity search  
- Redis for caching and performance  
- Google OAuth + Gmail API integration  
- React frontend for review-first workflow  

🔗 Repo: https://github.com/ShishirPathak/gmail-cleanup-ai

---

### 🔹 QuestionBuilderAI — OCR + LLM Document Pipeline

Built an OCR + LLM pipeline to convert **unstructured handwritten or scanned content into structured question papers**.

#### Highlights
- Extracted text using OCR (Tesseract / OCR APIs)  
- Structured content using LLM prompting  
- Handled noisy inputs and layout inconsistencies  
- Generated clean, formatted outputs for downstream usage  

#### Key Insight
LLMs are effective when paired with **pre-processing and validation layers**, not used in isolation.

🔗 Repo: https://github.com/ShishirPathak/QuestionBuilderAI

---

### 🔹 Streamify — Video Platform with Behavioral Analytics

A full-stack streaming system with **user engagement analytics**.

#### Highlights
- Built scalable upload and streaming pipeline  
- Implemented engagement tracking (rewatch, drop-off)  
- Used Redis for caching and performance optimization  
- Designed backend APIs for real-time interaction data  

#### Focus
Understanding **user behavior through system-generated signals**, not just raw data.

🔗 Repo: https://github.com/ShishirPathak/Streamify

---

### 🔹 UMassD Schedule Assistant — AI-Powered Query System

AI assistant handling student scheduling queries via text and voice.

#### Highlights
- Integrated LLM for natural language queries  
- Designed API layer for structured responses  
- Handled 100+ daily queries  

#### Focus
Building **LLM-backed interfaces with controlled outputs**.

🔗 Live: https://umassd-class-clock.vercel.app

---

## 🧠 Engineering Focus

I’m particularly interested in:

- Designing systems where AI is **assisted, not blindly trusted**  
- Combining retrieval, rules, and LLMs into reliable pipelines  
- Building observable systems with clear decision boundaries  
- Trade-offs between automation, safety, and cost in AI workflows  

---

## 🧰 Tech Stack

**Languages:** C#, Python, JavaScript, TypeScript  
**Backend:** .NET, FastAPI, Node.js  
**Frontend:** React  
**Databases:** PostgreSQL, MongoDB, Redis  
**Cloud & Tools:** Azure, AWS, Docker, Kubernetes  
**AI/ML:** LLM APIs, OCR pipelines, embeddings, vector search  

---

## 📫 Connect

- LinkedIn: https://linkedin.com/in/shishirkrpathak  
- Portfolio: https://shishir-kumar-pathak.vercel.app  
- Email: pathakshishir123@gmail.com
