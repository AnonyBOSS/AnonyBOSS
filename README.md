<div align="center">

<h1>Ahmed Hossam Abdallah Ibrahim</h1>
<h3>AI & LLM Engineering &nbsp;·&nbsp; Full-Stack & Mobile Development</h3>

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

I build **LLM serving infrastructure**, **on-device AI**, and the **products** on top of them.

- 🤖 **Now building:** the perception stack for a **Siemens-sponsored humanoid robot** (graduation project, Team A: Perception)
- ⚙️ **Flagship infra:** a distributed LLM serving stack that **survives a worker crash mid-run without losing a request**
- 🎓 **Education:** dual degree, graduating 2027 — B.Sc. Computer & AI Engineering (**Ain Shams University**, GPA 3.09) + B.Sc. Computer Science (**University of East London**)
- 💼 **Open to** AI/ML engineering, full-stack and mobile internships

---

## Featured Work

### 🤖 Humanoid Agent — Emotionally-Aware Workplace Robot
*Siemens-sponsored graduation project · 2026 – 2027 · in progress*

An edge-first humanoid support robot built by three teams (Perception, Cognitive Brain, Expression & HMI). I'm on **Team A — Perception**, which owns everything the robot senses:

- On-device **Whisper speech-to-text** (TensorRT INT8, Arabic/English), **speech + facial emotion recognition** and speaker binding on an **NVIDIA Jetson Orin NX**
- A **multimodal fusion node** publishing the `/interaction_state` and `/gaze_target` **ROS 2** contracts to the reasoning and neck-control teams
- **VAD + neural end-of-utterance detection** tuned for Egyptian-Arabic pauses, as part of an **800 ms time-to-first-audio** target
- Privacy by construction: raw audio and video never leave the robot's head

`ROS 2` `NVIDIA Jetson` `TensorRT` `Whisper` `PyTorch` `Python`

### ⚙️ [Distributed GPU Load Balancer for LLMs](https://github.com/AnonyBOSS/llm-distributed-gpu-load-balancer)
*Distributed LLM serving: NGINX → load balancer → 2 masters → 4 inference workers (7 FastAPI services, 10 Docker containers)*

- **Crash-tested:** SIGKILL a worker mid-run and its in-flight requests fail over to healthy workers — **250 of 250 served**
- **1,000 simultaneous requests** (simulated inference): **0 failed** under all 4 routing strategies (round-robin, least-connections, load-aware, power-of-two), p99 ≈ 4 s
- **Real Qwen2.5-0.5B inference** on 2 GPU + 2 CPU workers (one laptop RTX 3060), with load shedding when the cluster is full
- **RAG** with FAISS, **Prometheus + Grafana** latency dashboards, lint + pytest CI

`Python` `FastAPI` `Hugging Face Transformers` `FAISS` `Docker` `NGINX` `Prometheus` `Grafana`

### 🩺 [Clinify — Healthcare Booking Platform (Web + Mobile)](https://github.com/AnonyBOSS/Clinic-Web-App)
*Patient–doctor platform: one Next.js + MongoDB backend serving a web app and a React Native mobile app*

- **Race-safe booking:** atomic MongoDB updates prevent double-booking
- **AI symptom checker & assistant** (Llama 3.3 70B via Groq) that suggests which specialist to see
- Doctor search, auto-generated schedules, chat, ratings, role-based dashboards, **English/Arabic with RTL**

`Next.js` `React Native` `Expo` `TypeScript` `MongoDB` `Groq` `Tailwind CSS`

[Live Demo](https://clinic-web-app-two.vercel.app/) · [Web Repo](https://github.com/AnonyBOSS/Clinic-Web-App) · [Mobile Repo](https://github.com/AnonyBOSS/Clinify-mobile-app)

---

## More Projects

| Project | What it is | Stack |
|---|---|---|
| [FeatherLens](https://github.com/AnonyBOSS/featherlens-pixels-to-language) | Team project: fine-grained bird classification on CUB-200-2011 — ConvNeXt ensemble at **90.3% top-1 on the official test set**, with Grad-CAM | PyTorch |
| [UniManage](https://github.com/AnonyBOSS/University-Management-System-MVP) · [demo](https://university-management-system-mvp.vercel.app/) | Role-based university platform: Row-Level Security on all 10 tables, a Postgres trigger against double-booking, real-time messaging | Next.js 16, Supabase, PostgreSQL |
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
| **Languages** | Python · TypeScript · JavaScript · Dart · C++ · C# · Java · VHDL |
| **AI / ML** | PyTorch · TensorFlow / Keras · scikit-learn · Hugging Face Transformers · LangChain · FAISS |
| **Backend & Infra** | FastAPI · Node.js / Express · Docker · NGINX · Prometheus · Grafana · GitHub Actions · Linux · Vercel |
| **Mobile & Web** | Flutter · Riverpod · React Native / Expo · Next.js · React · Tailwind CSS |
| **Data** | PostgreSQL / Supabase · MongoDB · SQLite / Drift |

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
  <b>Open to AI/ML engineering, full-stack and mobile internships</b> — reach me by <a href="mailto:ahmadhossam82004@gmail.com">email</a> or on <a href="https://www.linkedin.com/in/ahmed-hossam-abdallah-673392309">LinkedIn</a>.
</div>
