<div align="center">

![Ronnit Chopra](https://capsule-render.vercel.app/api?type=waving&color=0:4C1D95,50:6D28D9,100:312E81&height=230&section=header&text=Ronnit%20Chopra&fontSize=54&fontColor=FFFFFF&animation=fadeIn&fontAlignY=38&desc=Software%20Engineer%20%7C%20Distributed%20Systems%20%7C%20AI%2FML&descAlignY=58&descSize=19)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=23&duration=3200&pause=900&color=A78BFA&center=true&vCenter=true&width=820&lines=Building+reliable+distributed+systems;Engineering+grounded+AI+applications;Turning+complex+workflows+into+scalable+software)](https://git.io/typing-svg)

![Michigan State University](https://img.shields.io/badge/Michigan%20State%20University-Computer%20Science-18453B?style=flat-square&logo=academia&logoColor=white)
![Class of 2026](https://img.shields.io/badge/Class%20of-2026-6D28D9?style=flat-square)
![GPA](https://img.shields.io/badge/GPA-3.8%2F4.0-7C3AED?style=flat-square)
![Dean's List](https://img.shields.io/badge/Dean's%20List-All%20Semesters-8B5CF6?style=flat-square)
![Location](https://img.shields.io/badge/East%20Lansing-Michigan-4338CA?style=flat-square&logo=googlemaps&logoColor=white)

[![Portfolio](https://img.shields.io/badge/Engineering%20Portfolio-5B21B6?style=for-the-badge&logo=vercel&logoColor=white)](https://github.com/KlutzyFella?tab=repositories)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-4338CA?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ronnit-chopra)
[![Email](https://img.shields.io/badge/Email-7C3AED?style=for-the-badge&logo=gmail&logoColor=white)](mailto:choprar3@msu.edu)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KlutzyFella)

[![Profile Views](https://komarev.com/ghpvc/?username=KlutzyFella&label=Profile%20Views&color=6D28D9&style=flat-square)](https://github.com/KlutzyFella)
[![Followers](https://img.shields.io/github/followers/KlutzyFella?label=Followers&style=flat-square&color=7C3AED)](https://github.com/KlutzyFella?tab=followers)
[![Stars](https://img.shields.io/github/stars/KlutzyFella/tadk-simulator?label=Project%20Stars&style=flat-square&color=8B5CF6)](https://github.com/KlutzyFella/tadk-simulator/stargazers)

</div>

---

## About Me

I am a software engineer and Computer Science graduate from **Michigan State University** who enjoys building systems that remain reliable under scale, concurrency, and failure. My work spans **distributed backends, AI/ML infrastructure, cloud engineering, and full-stack product development**.

I approach engineering as a product discipline: start with the user or operational constraint, design explicit service boundaries, make failure modes observable, and measure whether the system actually improves the workflow. Recent work includes a serverless lifecycle simulator validated on **100,000+ production-trace events**, a citation-grounded RAG platform, a fault-tolerant distributed task engine, and an underwriting workflow projected to save **200+ labor hours annually**.

### Open To

- Backend, platform, distributed-systems, and AI engineering roles
- Open-source collaboration involving infrastructure, developer tooling, or applied AI
- Teams that value measurable impact, strong system design, and production ownership

---

## Tech Stack

### Languages

<div align="center">

[![Languages](https://skillicons.dev/icons?i=cpp,python,go,java,js,ts,cs&theme=dark)](https://skillicons.dev)

</div>

### Frontend

<div align="center">

[![Frontend](https://skillicons.dev/icons?i=react,nextjs,angular,tailwind&theme=dark)](https://skillicons.dev)

</div>

### Backend & Databases

<div align="center">

[![Backend and Databases](https://skillicons.dev/icons?i=nodejs,express,flask,postgres,mongodb,redis,supabase&theme=dark)](https://skillicons.dev)

</div>

`gRPC` `Protobuf` `Kafka` `pgvector` `Quarkus` `FastAPI` `LangChain`

### Cloud, DevOps & Tooling

<div align="center">

[![Cloud and DevOps](https://skillicons.dev/icons?i=aws,terraform,kubernetes,docker,git,github,linux&theme=dark)](https://skillicons.dev)

</div>

`Amazon EC2` `Amazon S3` `IAM` `K3s` `Prometheus` `Grafana` `Fly.io` `Unix`

---

## AI / ML Expertise

| Domain | Proficiency | Details |
|:---|:---:|:---|
| Retrieval-Augmented Generation | Advanced applied | Designed a polyglot RAG system with asynchronous ingestion, vector retrieval, structured generation, and source-level citation validation |
| Embeddings & Vector Search | Strong working | Built MiniLM-L6-v2 embedding pipelines and HNSW cosine-similarity retrieval with PostgreSQL and pgvector |
| LLM Reliability | Strong working | Cross-validates model-generated citation IDs against retrieved chunks and removes unsupported references before response delivery |
| ML Infrastructure | Strong working | Integrated Go gateways, Python ML microservices, Kafka pipelines, gRPC contracts, and containerized data services |
| Simulation & Experimentation | Advanced applied | Replayed 100,000+ serverless production-trace events using deterministic discrete-event simulation and regression-tested baselines |

---

## Featured Projects

<details open>
<summary><b>TADK - Trigger-Aware Dynamic Keep-Alive Simulator</b></summary>
<br>

A reproducible discrete-event simulation environment for evaluating serverless container keep-alive policies against real Huawei production traces.

| Dimension | Detail |
|:---|:---|
| **Stack** | Python 3.10+, pandas, `heapq`, dataclasses, pytest |
| **Scale** | 100,000 invocation events, 180 functions, and 540 policy-function result rows |
| **Performance** | Executes 100,000-event simulations in under one second using a lock-free priority queue and virtual clock |
| **Security** | Fail-fast input validation, deterministic replay, invariant testing, and no external runtime services |
| **Impact** | Reduced idle-memory cost by **66.93%** versus the 60-second baseline while holding cold-start rate to **0.20%** |
| **Repository** | [github.com/KlutzyFella/tadk-simulator](https://github.com/KlutzyFella/tadk-simulator) |

TADK makes keep-alive timeouts responsive to invocation triggers. Timer-driven functions receive an interval-aware timeout, while API traffic uses a tighter window. The simulator exposes a pluggable policy interface, per-function breakdowns, canonical input traces, and regression tests so every headline result can be independently reproduced.

</details>

<details open>
<summary><b>Cortex - Citation-Grounded RAG Engine</b></summary>
<br>

A production-oriented RAG platform that ingests documents asynchronously and returns natural-language answers grounded in the exact passages retrieved.

| Dimension | Detail |
|:---|:---|
| **Stack** | Go, Python, Kafka/Redpanda, gRPC, Protobuf, PostgreSQL, pgvector, LangChain, Gemini |
| **Scale** | Go API gateway routing across three Python microservices with event-driven document ingestion |
| **Performance** | HNSW cosine-similarity indexing supports sub-second retrieval while Kafka keeps embedding work off the request path |
| **Security** | No hardcoded secrets; services fail fast on missing credentials; generated citations are validated against retrieved chunk IDs |
| **Impact** | Prevents unsupported references from reaching users and makes every surviving citation traceable to source context |
| **Repository** | [github.com/KlutzyFella/cortex](https://github.com/KlutzyFella/cortex) |

Cortex uses contract-first gRPC services to separate ingestion, retrieval, and generation. Documents are chunked, embedded into 384-dimensional vectors, and indexed in pgvector. Structured LLM output is then checked against the chunks supplied to the model, creating an explicit reliability layer around generated answers.

</details>

<details open>
<summary><b>Dispatch - Distributed Task Execution Engine</b></summary>
<br>

A fault-tolerant task engine that separates reliable task intake from independently scalable worker execution.

| Dimension | Detail |
|:---|:---|
| **Stack** | Go, Apache Kafka, Redis, gRPC, Protobuf, Prometheus, Grafana, Docker, Kubernetes |
| **Scale** | Kubernetes HPA scales workers from 2 to 10 replicas; Kafka decouples dispatch and execution |
| **Performance** | Long-lived bidirectional gRPC streams reduce connection overhead; independent workers enable horizontal throughput scaling |
| **Security** | Minimal containers run as a non-root user; idempotency keys and expiring distributed locks constrain duplicate execution |
| **Impact** | Converts at-least-once delivery into effectively-once execution and quarantines exhausted tasks in a dead-letter queue |
| **Repository** | [github.com/KlutzyFella/dispatch](https://github.com/KlutzyFella/dispatch) |

Dispatch commits Kafka offsets only after successful completion or dead-lettering. Redis locks prevent concurrent execution of the same task, idempotent submission protects clients from duplicate enqueues, and Prometheus instrumentation exposes throughput, errors, and P99 latency across the task lifecycle.

</details>

---

## Experience

### Software Developer - Delta Dental

**Sep 2025 - Dec 2025 | East Lansing, MI**

Built an underwriting document-generation platform designed to replace fragmented manual workflows with a traceable, full-stack process.

- Architected a Java Quarkus and AWS S3 document pipeline projected to save **200+ labor hours annually**.
- Reduced API latency by **96%** by adding a MongoDB caching layer that bypassed redundant Azure Maps calls.
- Enforced full-stack type safety and schema validation, with audit timestamps, error logging, and consistent data contracts.

![Java](https://img.shields.io/badge/Java-Quarkus-6D28D9?style=flat-square&logo=openjdk&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-S3-7C3AED?style=flat-square&logo=amazonaws&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Caching-8B5CF6?style=flat-square&logo=mongodb&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-Frontend-4338CA?style=flat-square&logo=angular&logoColor=white)

### Software Developer Intern - Sopra Steria

**Jun 2025 - Aug 2025 | Remote**

Modernized a Go service from serverless deployment to reproducible, provisioned Kubernetes infrastructure.

- Defined service boundaries and built a functional K3s cluster across two AWS EC2 instances.
- Automated EC2, IAM, and Security Group provisioning with Terraform.
- Configured Kubernetes ingress and resolved OOMKill and DNS failures to establish stable two-node routing.

![Go](https://img.shields.io/badge/Go-Services-6D28D9?style=flat-square&logo=go&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-IaC-7C3AED?style=flat-square&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-K3s-8B5CF6?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-EC2%20%7C%20IAM-4338CA?style=flat-square&logo=amazonaws&logoColor=white)

### Full-Stack Web Developer - Imagine Software Club

**Feb 2025 - Jun 2025 | East Lansing, MI**

Developed product features for Course Checker as part of a four-person agile engineering team.

- Shipped new course rating and review features with Next.js, TypeScript, Tailwind, Supabase, Docker, and Fly.io.
- Built an authentication flow with Supabase and Resend to protect user data and support future product scaling.

![Next.js](https://img.shields.io/badge/Next.js-Product-6D28D9?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-Full%20Stack-7C3AED?style=flat-square&logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-Auth%20%26%20Data-8B5CF6?style=flat-square&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Deployment-4338CA?style=flat-square&logo=docker&logoColor=white)

---

## Achievements

<div align="center">

| Recognition | Details |
|:---|:---|
| **Dean's List** | Earned in every semester at Michigan State University |
| **Academic Performance** | Graduated with a **3.8/4.0 GPA** in Computer Science |
| **Serverless Systems Research** | Demonstrated a **66.93% reduction** in idle-memory cost across 100,000 production-trace events |
| **Workflow Automation Impact** | Developed a system projected to save **200+ underwriting labor hours annually** |
| **Performance Engineering** | Reduced external API latency by **96%** through a MongoDB caching layer |

</div>

---

## Certifications

Verified certifications were not included in the source material. Provider badges are retained for the requested structure; credential names and verification links should be added only when available.

### AWS

![AWS](https://img.shields.io/badge/AWS-Credential%20details%20needed-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)

### Oracle

![Oracle](https://img.shields.io/badge/Oracle-Credential%20details%20needed-5B21B6?style=for-the-badge&logo=oracle&logoColor=white)

### NPTEL

![NPTEL](https://img.shields.io/badge/NPTEL-Credential%20details%20needed-6D28D9?style=for-the-badge)

### Cisco

![Cisco](https://img.shields.io/badge/Cisco-Credential%20details%20needed-4338CA?style=for-the-badge&logo=cisco&logoColor=white)

---

## Coding Profiles

<div align="center">

<a href="https://leetcode.com/u/KlutzyFella/"><img src="https://img.shields.io/badge/LeetCode-KlutzyFella-5B21B6?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" /></a>
<a href="https://www.geeksforgeeks.org/profile/klutzyfella"><img src="https://img.shields.io/badge/GeeksforGeeks-klutzyfella-6D28D9?style=for-the-badge&logo=geeksforgeeks&logoColor=white" alt="GeeksforGeeks" /></a>
<a href="https://www.hackerrank.com/KlutzyFella"><img src="https://img.shields.io/badge/HackerRank-KlutzyFella-7C3AED?style=for-the-badge&logo=hackerrank&logoColor=white" alt="HackerRank" /></a>
<a href="https://www.codechef.com/users/klutzyfella"><img src="https://img.shields.io/badge/CodeChef-klutzyfella-4338CA?style=for-the-badge&logo=codechef&logoColor=white" alt="CodeChef" /></a>

</div>

---

## GitHub Analytics

<div align="center">

<img width="49%" src="https://github-readme-stats.vercel.app/api?username=KlutzyFella&show_icons=true&hide_border=true&bg_color=0D1117&title_color=A78BFA&text_color=C9D1D9&icon_color=8B5CF6&rank_icon=github" alt="Ronnit's GitHub statistics" />
<img width="49%" src="https://streak-stats.demolab.com?user=KlutzyFella&hide_border=true&background=0D1117&ring=8B5CF6&fire=A78BFA&currStreakLabel=A78BFA&sideLabels=C9D1D9&dates=8B949E&currStreakNum=FFFFFF&sideNums=FFFFFF" alt="Ronnit's GitHub streak" />

<img width="56%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=KlutzyFella&layout=compact&langs_count=8&hide_border=true&bg_color=0D1117&title_color=A78BFA&text_color=C9D1D9" alt="Ronnit's top languages" />

</div>

---

## GitHub Trophies

<div align="center">

[![GitHub Trophies](https://github-profile-trophy.vercel.app/?username=KlutzyFella&theme=tokyonight&no-frame=true&no-bg=true&margin-w=10&margin-h=10&column=4)](https://github.com/ryo-ma/github-profile-trophy)

</div>

---

## Contribution Activity

<div align="center">

[![Ronnit's GitHub activity graph](https://github-readme-activity-graph.vercel.app/graph?username=KlutzyFella&bg_color=0D1117&color=C4B5FD&line=8B5CF6&point=FFFFFF&area=true&area_color=5B21B6&hide_border=true)](https://github.com/KlutzyFella)

</div>

---

## Contribution Snake

<div align="center">

![GitHub contribution snake](https://raw.githubusercontent.com/KlutzyFella/KlutzyFella/output/github-contribution-grid-snake-dark.svg)

</div>

---

## Current Focus

```yaml
learning:
  - Production-grade distributed systems
  - Reliable AI and retrieval infrastructure
building:
  - Fault-tolerant backend services
  - Grounded AI products with measurable user value
exploring:
  - Event-driven architecture
  - Kubernetes operations and observability
open_to:
  - Backend, platform, and AI engineering opportunities
  - Open-source collaboration
```

---

## Connect

<div align="center">

[![Gmail](https://img.shields.io/badge/Gmail-choprar3%40msu.edu-7C3AED?style=for-the-badge&logo=gmail&logoColor=white)](mailto:choprar3@msu.edu)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ronnit%20Chopra-4338CA?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ronnit-chopra)
[![GitHub](https://img.shields.io/badge/GitHub-KlutzyFella-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KlutzyFella)
[![Portfolio](https://img.shields.io/badge/Portfolio-Selected%20Repositories-5B21B6?style=for-the-badge&logo=vercel&logoColor=white)](https://github.com/KlutzyFella?tab=repositories)

</div>

---

<div align="center">

**Build systems that stay correct under load, failure, and change.**

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:312E81,50:6D28D9,100:4C1D95&height=120&section=footer)

</div>


<!--
**KlutzyFella/KlutzyFella** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
