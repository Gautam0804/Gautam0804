<p align="center">
  <img src="./banner.svg" width="100%" alt="Gautam Kumar Yadav Banner">
</p>

<h1 align="center">Hi, I'm Gautam Kumar Yadav 👋</h1>

<h3 align="center">
  Software Engineer · Full Stack Developer · AI/ML Engineer
</h3>

<p align="center">
  I build production-oriented full-stack, backend, and AI-powered systems —<br>
  from secure REST APIs to RAG pipelines and ML inference services.
</p>

<p align="center">
  <a href="https://gautam-portfolio-self.vercel.app/">
    <img src="https://img.shields.io/badge/PORTFOLIO-ff4db8?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio">
  </a>
  <a href="https://www.linkedin.com/in/gautam-yadav-10922726b/">
    <img src="https://img.shields.io/badge/LINKEDIN-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:gautamcodesin@gmail.com">
    <img src="https://img.shields.io/badge/EMAIL-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
  <a href="https://leetcode.com/u/Gautam_Yadav8/">
    <img src="https://img.shields.io/badge/LEETCODE-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode">
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Gautam0804&label=PROFILE%20VIEWS&color=ff4db8&style=flat-square" alt="Profile Views">
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1200&color=FF4DB8&center=true&vCenter=true&width=720&lines=Full+Stack+Developer;Backend+%26+REST+API+Engineer;AI%2FML+%26+RAG+Systems;300%2B+DSA+Problems+Solved" alt="Typing animation">
</p>

<p align="center">
  <a href="#-recruiter-quick-glance">Quick Glance</a> ·
  <a href="#-featured-projects">Projects</a> ·
  <a href="#-tech-stack">Tech Stack</a> ·
  <a href="#-achievements">Achievements</a> ·
  <a href="#-github--coding-activity">Activity</a> ·
  <a href="#-lets-work-together">Contact</a>
</p>

---

## 🎯 Recruiter Quick Glance

| | |
|---|---|
| **🟢 Open to** | Software Engineering · Full Stack · Backend · AI/ML roles |
| **💪 Strongest at** | Backend APIs (Node.js / FastAPI), RAG & vector search, ML model integration, secure auth (JWT + RBAC) |
| **🛠️ Core languages** | Java · Python · JavaScript / TypeScript |
| **🏆 Proof of work** | 300+ DSA problems · Google Solution Challenge 2025 · HackIndia 2025 · Adobe University Hackathon 2026 |
| **🚀 Flagship project** | [Nexora AI](https://github.com/Gautam0804/Nexora-AI) — private-document RAG platform with page-level citations |
| **📬 Fastest way to reach me** | [gautamcodesin@gmail.com](mailto:gautamcodesin@gmail.com) |

---

## 🚀 Featured Projects

<table>
<tr>

<td width="50%" valign="top">

### 📚 Nexora AI
**AI Document Intelligence & Semantic Search**

Upload private PDFs, search them semantically, and get **RAG answers with document + page-level citations**.

**Highlights**
- 384-D BGE embeddings + **pgvector** similarity search
- Page-level extraction with overlapping chunking
- Private storage with **signed URLs**, JWT auth, bcrypt, user-level authorization
- Local LLM inference via **Ollama (Qwen 2.5 3B)**

**Stack:** `Next.js` `TypeScript` `Tailwind` `Node.js` `Express` `PostgreSQL` `pgvector` `FastAPI` `Sentence Transformers` `Supabase`

<a href="https://github.com/Gautam0804/Nexora-AI">
<img src="https://img.shields.io/badge/VIEW%20PROJECT-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="Nexora AI">
</a>

</td>

<td width="50%" valign="top">

### 🛡️ RiskForge
**Real-Time AI Fraud Detection & Risk Intelligence**

Scores transactions in real time by combining **rule-based signals, anomaly analysis, and an XGBoost model**.

**Highlights**
- FastAPI ML inference service decoupled from the main API
- Redis caching for low-latency risk lookups
- PostgreSQL persistence for transactions, risk scores, and alerts
- Risk & alert workflows for flagged activity

**Stack:** `React` `Node.js` `Express` `PostgreSQL` `Redis` `FastAPI` `XGBoost`

<a href="https://github.com/Gautam0804/RiskForge">
<img src="https://img.shields.io/badge/VIEW%20PROJECT-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="RiskForge">
</a>

</td>

</tr>
<tr>

<td width="50%" valign="top">

### 🚚 RouteX
**Full-Stack Fleet Operations Platform**

Manage vehicles, drivers, shipments, assignments, tracking, and alerts from one dashboard.

**Highlights**
- JWT authentication with **role-based access control**
- Authorization middleware protecting every sensitive route
- Clean RESTful API architecture
- Shipment ↔ driver ↔ vehicle assignment workflows

**Stack:** `React` `Node.js` `Express` `MySQL` `JWT` `REST`

<a href="https://github.com/Gautam0804/route-x">
<img src="https://img.shields.io/badge/VIEW%20PROJECT-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="RouteX">
</a>

</td>

<td width="50%" valign="top">

### 🤖 PredictX
**AI Predictive Maintenance Platform**

Analyzes industrial sensor data (temperature, vibration) to predict **equipment health and failure risk**.

**Highlights**
- Random Forest model for failure-probability prediction
- FastAPI inference service consumed by the Node backend
- Health & risk assessment with maintenance recommendations
- MongoDB storage for sensor readings and predictions

**Stack:** `React` `Node.js` `Express` `MongoDB` `FastAPI` `Scikit-learn`

<a href="https://github.com/Gautam0804/PredictX">
<img src="https://img.shields.io/badge/VIEW%20PROJECT-GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="PredictX">
</a>

</td>

</tr>
</table>

### 🧠 Under the hood: Nexora AI's RAG pipeline

```mermaid
flowchart LR
    subgraph Ingestion
        A[PDF Upload] --> B[Page-level Extraction] --> C[Overlapping Chunking] --> D[BGE Embeddings · 384D]
    end
    D --> E[(PostgreSQL + pgvector)]
    subgraph Query
        Q[User Question] --> F[Query Embedding] --> G[Similarity Search] --> H[Context Assembly] --> I[Qwen 2.5 3B · Ollama] --> J[Cited Answer]
    end
    E --> G
```

---

## 🧰 Tech Stack

<div align="center">

<h3>💻 Languages</h3>
<img src="https://skillicons.dev/icons?i=java,python,c,js,ts,html,css" alt="Languages">

<br><br>

<h3>🌐 Frontend & Backend</h3>
<img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,express,fastapi,tailwind" alt="Frontend and Backend">

<br><br>

<h3>🗄️ Databases & Tools</h3>
<img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb,redis,supabase,docker,git,github,vscode" alt="Databases and Tools">

<br><br>

<h3>🤖 AI / ML</h3>
<img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
<img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="Scikit-Learn">
<img src="https://img.shields.io/badge/XGBoost-1F425F?style=for-the-badge" alt="XGBoost">
<br>
<img src="https://img.shields.io/badge/RAG-6C5CE7?style=for-the-badge" alt="RAG">
<img src="https://img.shields.io/badge/pgvector-336791?style=for-the-badge" alt="pgvector">
<img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge" alt="Ollama">

<br><br>

<h3>🔐 Concepts</h3>
<img src="https://img.shields.io/badge/REST%20API-ff4db8?style=for-the-badge" alt="REST API">
<img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge" alt="JWT">
<img src="https://img.shields.io/badge/RBAC-6C5CE7?style=for-the-badge" alt="RBAC">
<br>
<img src="https://img.shields.io/badge/System%20Design-4B5563?style=for-the-badge" alt="System Design">
<img src="https://img.shields.io/badge/DSA-8b5cf6?style=for-the-badge" alt="DSA">

</div>

---

## 🏆 Achievements

<p>
  <img src="https://img.shields.io/badge/DSA-300%2B%20Problems-ff4db8?style=for-the-badge" alt="DSA">
  <img src="https://img.shields.io/badge/Google%20Solution%20Challenge-2025-6C5CE7?style=for-the-badge" alt="Google Solution Challenge 2025">
  <img src="https://img.shields.io/badge/HackIndia-2025-181717?style=for-the-badge" alt="HackIndia 2025">
  <img src="https://img.shields.io/badge/Adobe%20University%20Hackathon-2026-FF0000?style=for-the-badge" alt="Adobe University Hackathon 2026">
  <img src="https://img.shields.io/badge/Google-Generative%20AI-4285F4?style=for-the-badge" alt="Google Generative AI">
</p>

---

## 📊 GitHub & Coding Activity

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Gautam0804&theme=tokyonight" alt="GitHub Statistics" width="100%" />
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Gautam0804&theme=tokyonight" alt="Repos per Language" width="49%" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Gautam0804&theme=tokyonight" alt="Most Used Languages" width="49%" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Gautam0804&theme=tokyonight&hide_border=true&border_radius=5&card_width=600" alt="GitHub Streak" width="75%" />
</p>

### 🐍 Contribution Snake

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Gautam0804/Gautam0804/output/github-contribution-grid-snake-dark.svg?v=2">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Gautam0804/Gautam0804/output/github-contribution-grid-snake.svg?v=2">
    <img src="https://raw.githubusercontent.com/Gautam0804/Gautam0804/output/github-contribution-grid-snake.svg?v=2" alt="GitHub Contribution Snake" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/Gautam0804/Gautam0804/actions/workflows/snake.yml">
    <img src="https://img.shields.io/badge/Contribution%20Snake-GitHub%20Actions-ff4db8?style=for-the-badge&logo=github&logoColor=white" alt="Contribution Snake Workflow">
  </a>
</p>

<p align="center">
  <a href="https://leetcode.com/u/Gautam_Yadav8/">
    <img src="https://leetcard.jacoblin.cool/Gautam_Yadav8?theme=dark&font=Baloo&ext=heatmap" alt="LeetCode Statistics and Heatmap" width="75%" />
  </a>
</p>

**Competitive programming & practice profiles**

<p>
  <a href="https://leetcode.com/u/Gautam_Yadav8/"><img src="https://img.shields.io/badge/LeetCode-Gautam__Yadav8-FFA116?style=flat-square&logo=leetcode&logoColor=black" alt="LeetCode"></a>
  <a href="https://codeforces.com/profile/Gautam0804"><img src="https://img.shields.io/badge/Codeforces-Gautam0804-1F8ACB?style=flat-square&logo=codeforces&logoColor=white" alt="Codeforces"></a>
  <a href="https://www.geeksforgeeks.org/profile/gautamcrn2z"><img src="https://img.shields.io/badge/GeeksforGeeks-Gautam-0F9D58?style=flat-square&logo=geeksforgeeks&logoColor=white" alt="GeeksforGeeks"></a>
  <a href="https://www.hackerrank.com/profile/gautamcodesin"><img src="https://img.shields.io/badge/HackerRank-Gautam-2EC866?style=flat-square&logo=hackerrank&logoColor=white" alt="HackerRank"></a>
  <a href="https://codolio.com/profile/Gautam0804"><img src="https://img.shields.io/badge/Codolio-Gautam0804-6C5CE7?style=flat-square" alt="Codolio"></a>
</p>

---

## 🌱 Currently

- 🔨 Building AI-powered, production-oriented applications with RAG, vector search, and ML inference
- 🏗️ Strengthening **system design** and backend architecture
- 🧮 Going deeper on advanced data structures and competitive programming

---

## 🤝 Let's Work Together

I'm looking for **Software Engineering, Full Stack, Backend, and AI/ML** opportunities where I can ship real features and keep learning fast.

<p align="center">
  <a href="mailto:gautamcodesin@gmail.com">
    <img src="https://img.shields.io/badge/gautamcodesin%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
  <a href="https://www.linkedin.com/in/gautam-yadav-10922726b/">
    <img src="https://img.shields.io/badge/Connect%20on-LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
</p>

<p align="center">
  <code>~$ build • solve • learn • improve</code>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" alt="Footer">
</p>
