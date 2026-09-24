<div align="center">

<h1>Ahmed Hossam Abdallah</h1>
<h3>AI & LLM Engineering &nbsp;·&nbsp; Full-Stack Development</h3>

<p>
  <a href="https://www.linkedin.com/in/ahmed-hossam-abdallah-673392309">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:ahmadhossam82004@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact%20Me-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://drive.google.com/file/d/1UHjeomoRIhMDI37-F7O36rL2c-_jLHMR/view?usp=drive_link">
    <img src="https://img.shields.io/badge/CV-View-00B4D8?style=for-the-badge&logo=googledrive&logoColor=white" alt="CV" />
  </a>
</p>

</div>

I build **LLM serving infrastructure** and the **AI-powered products** on top of it.

- **Flagship:** a distributed LLM serving stack that handles **1,000-request bursts** and **survives a worker crash mid-run without losing a request**
- **Education:** dual degree, graduating 2027 — B.Sc. Computer & AI Engineering (**Ain Shams University**) + B.Sc. Computer Science (**University of East London**)
- **Certified:** IBM AI Engineering Professional Certificate (2026)
- **Open to** AI/ML engineering and full-stack internships

---

## Featured Projects

### [Distributed GPU Load Balancer for LLMs](https://github.com/AnonyBOSS/llm-distributed-gpu-load-balancer)
*Distributed LLM serving: NGINX → load balancer → 2 masters → 4 inference workers (7 FastAPI services, 10 Docker containers)*

- **Crash-tested:** SIGKILL a worker mid-run and its in-flight requests fail over to healthy workers — **250 of 250 served**, none needing a client retry
- **1,000 simultaneous requests** (simulated inference): **0 failed** under all 4 routing strategies (round-robin, least-connections, load-aware, power-of-two), p99 ≈ 4 s
- **Real Qwen2.5-0.5B inference** on 2 GPU + 2 CPU workers (one laptop RTX 3060), with load shedding when the cluster is full
- **RAG** with FAISS, **Prometheus + Grafana** latency dashboards, lint + pytest CI

`Python` `FastAPI` `Hugging Face Transformers` `FAISS` `Docker` `NGINX` `Prometheus` `Grafana`

### [Clinify — Healthcare Booking Platform (Web + Mobile)](https://github.com/AnonyBOSS/Clinic-Web-App)
*Patient–doctor platform: one Next.js + MongoDB backend serving a web app and a React Native mobile app*

- **Race-safe booking:** atomic MongoDB updates prevent double-booking; rooms under maintenance can't be scheduled
- **AI symptom checker & assistant** (Llama 3.3 70B via Groq) that suggests which specialist to see
- Doctor search, auto-generated schedules, chat, ratings, role-based dashboards, **English/Arabic with RTL**

`Next.js` `React Native` `Expo` `TypeScript` `MongoDB` `Groq` `Tailwind CSS`

[Live Demo](https://clinic-web-app-two.vercel.app/) · [Web Repo](https://github.com/AnonyBOSS/Clinic-Web-App) · [Mobile Repo](https://github.com/AnonyBOSS/Clinify-mobile-app)

### [UniManage — University Management System](https://github.com/AnonyBOSS/University-Management-System-MVP)
*Role-based university platform for students, professors, and admins*

- **Security in the database:** Row-Level Security on all 10 tables; a Postgres trigger blocks classroom double-booking
- Enrollment with capacity limits, assignment submission & grading, classroom booking, announcements
- **Real-time** messaging via Supabase Realtime; all writes go through Server Actions

`Next.js 16` `TypeScript` `Supabase` `PostgreSQL` `Tailwind CSS v4`

[Live Demo](https://university-management-system-mvp.vercel.app/) · [Repo](https://github.com/AnonyBOSS/University-Management-System-MVP)

---

## More Projects

| Project | What it is | Stack |
|---|---|---|
| [LLM Customer Feedback Analyzer](https://github.com/AnonyBOSS/NVIDIA-DLI-PromptEngineering-Assessment) | NVIDIA DLI final project: LangChain pipeline that finds the products and stores behind negative feedback | LangChain, Llama 3.1 8B |
| [Detect-AI](https://github.com/AnonyBOSS/detect-AI) | Kaggle AI-vs-human image detection with transfer learning — **98th on the final leaderboard** | TensorFlow, PyTorch |
| [Reddit Clone](https://github.com/AnonyBOSS/reddit-clone) · [demo](https://reddit-clone-iota-taupe.vercel.app/login) | Team project — I built the profile page and direct messaging | React, Express, MongoDB |
| [Heart Disease Prediction](https://github.com/AnonyBOSS/heart-disease-prediction-ml) | Team of 6 comparing 6 classifiers — I built the SVM model and worked on preprocessing | scikit-learn |
| [Tiny Language Compiler](https://github.com/AnonyBOSS/Tiny-language-compiler) | Scanner and CFG-based parser with a desktop UI | C# |
| [MIPS Processor](https://github.com/AnonyBOSS/MIPS-processor) | Datapath, ALU, and controller with testbenches | VHDL |
| [Enterprise Network Design](https://github.com/AnonyBOSS/Cisco-PacketTracer-Supply-chain-enterprise-project) | Multi-site network: VLANs, OSPF, NAT, ACLs, zone-based firewall | Cisco Packet Tracer |

[All repositories →](https://github.com/AnonyBOSS?tab=repositories)

---

## Tech Stack

| Area | Tools |
|---|---|
| **Languages** | Python · TypeScript · JavaScript · C++ · C# · Java · VHDL |
| **AI / ML** | PyTorch · TensorFlow / Keras · scikit-learn · Hugging Face Transformers · LangChain · FAISS |
| **Backend & Infra** | FastAPI · Node.js / Express · Docker · NGINX · Prometheus · Grafana · GitHub Actions · Linux |
| **Web & Mobile** | Next.js · React · React Native / Expo · Tailwind CSS |
| **Data** | PostgreSQL / Supabase · MongoDB |

---

## Certifications

| Certificate | Issuer | Date |
|---|---|---|
| AI Engineering Professional Certificate | IBM & Coursera | Feb 2026 |
| Generative AI — Beginner Level | ITI & NVIDIA DLI | Sep 2025 |
| Web Development with React | ITI | Aug 2025 |
| Network Infrastructure | NTI & ITIDA | Aug 2025 |
| Huawei HCIA AI | NTI | Feb 2025 |
| Competitive Programming (C++) | Coach Academy | Aug 2024 |

---

<div align="center">
  <b>Open to AI/ML engineering and full-stack internships</b> — reach me by <a href="mailto:ahmadhossam82004@gmail.com">email</a> or on <a href="https://www.linkedin.com/in/ahmed-hossam-abdallah-673392309">LinkedIn</a>.
</div>
