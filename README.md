<div align="center">
  <strong>Language / Edition:</strong>
  <a href="./README.zh-CN.md">简体中文</a>
  ·
  <strong>English (current)</strong>
  ·
  <a href="./README.rnd.md">R&amp;D Version</a>
  ·
  <a href="./README.rnd.zh-CN.md">R&amp;D 中文版</a>
</div>

<br>

<div align="center">
  <h1>
    Hi, I'm Li<sup>3+</sup> (Takina)
  </h1>
  <h3>
    Java Backend Developer • AI Infra &amp; Agent Tooling • Linux Systems
  </h3>
  <p>
    Building contract-first backend services, reproducible LLM evaluation harnesses, and Linux desktop &amp; self-hosted tooling
  </p>
  <p>
    <b>Java</b> • <b>Spring Boot</b> • Python • TypeScript • React • Linux • Docker / Podman • MySQL • Redis • RabbitMQ
  </p>
</div>

---

<div align="center">
  <a href="#profile">Profile</a> ·
  <a href="#value">Value</a> ·
  <a href="#highlights">Highlights</a> ·
  <a href="#experience">Experience</a> ·
  <a href="#projects">Projects</a> ·
  <a href="#stack">Stack</a> ·
  <a href="#fit">Roles</a>
</div>

---

<a id="profile"></a>

## Short Profile

I am a Computer Science undergraduate at **Beijing Jiaotong University** (Class of 2028, Railway Information Technology track) working at the intersection of **Java backend engineering**, **AI application & evaluation infrastructure**, and **Linux systems tooling**.

My work centers on turning ambiguous requirements into verifiable software: defining clear cross-service contracts, enforcing fail-closed runtime and privilege boundaries, and keeping explicit test evidence alongside known limitations rather than overclaiming scope.

- **Primary engineering focus:** Java / Spring Boot backend integration, multi-service data pipelines (MySQL, Redis, RabbitMQ, HTTP/WebSocket), and Linux deployment.
- **AI & evaluation workflow:** RAG retrieval pipelines, bounded agent execution in rootless containers, and paired evaluation harnesses. In AI-assisted development, I focus on requirements decomposition, architecture selection, code review, runtime verification, and delivery.
- **Public track record:** 10+ repositories spanning backend platforms, AI security testing prototypes, Fedora/GTK4 and Tauri/Rust desktop utilities, and self-hosted web services.
- **Independent domain track:** Urban spatial data / GIS processing and cycling route tooling, kept distinct from core Java backend engineering evidence.

**GitHub:** [github.com/Tak1naa](https://github.com/Tak1naa)  
**Repositories:** [github.com/Tak1naa?tab=repositories](https://github.com/Tak1naa?tab=repositories)  
**Personal Blog:** [tak1na.top/blog](https://tak1na.top/blog)  
**Live Service:** [tak1na.top/speedtest](https://tak1na.top/speedtest/)  
**Location:** Beijing, China

---

<a id="value"></a>

## Value For A Team

I contribute most effectively on teams that need an engineer who can:

- design and integrate **Java / Spring Boot** services with relational databases, Redis caching, RabbitMQ messaging, and WebSocket / SSE endpoints;
- bridge heterogeneous runtimes (Java, C++, Python, TypeScript) via explicit HTTP/JSON contracts and predictable fallback behavior;
- build **AI evaluation & RAG infrastructure** with reproducible test suites, side-effect verification, and clear separation between engineering checks and model efficacy;
- package and harden **Linux services and developer tools** using Docker Compose, rootless Podman, HAProxy, Polkit privilege separation, and bounded resource limits;
- deliver honest engineering artifacts with verified runtime checks, regression tests, and transparent documentation of unfinished work or environment boundaries.

---

<a id="highlights"></a>

## Engineering Highlights

### Java Backend & Multi-Service Integration

- **[Cafeteria-Management](https://github.com/Tak1naa/Cafeteria-Management):** Built the Spring Boot business and integration layer bridging a C++ simulation engine (HTTP JSON) with a Web frontend (WebSocket/HTTP), backed by MySQL, Redis, RabbitMQ, and optional DeepSeek API integration with a rule-engine fallback.
- **[TiCenter (题枢)](https://github.com/Tak1naa/TiCenter):** Architected a file-first AI question bank and document QA workspace across Spring Boot, React/TypeScript, MySQL, Redis, Qdrant, and Python AI services, featuring multi-file tabs, selection-scoped context, hybrid BM25 + vector retrieval (RRF), SSE streaming, and citation jump-back *(currently paused progress snapshot; cross-service OCR/Qdrant migration and acceptance remain incomplete)*.

### AI Engineering, RAG & Security Evaluation

- **[Agent-Harness](https://github.com/Tak1naa/Agent-Harness):** Developing an undergraduate innovation research prototype studying how Bandit static alerts and AST function context affect LLM-generated Python security tests under fixed model/tool/call budgets. Combines restricted `pytest`/`Hypothesis` synthesis, rootless Podman execution, real side-effect probes (path traversal, command injection, SQL injection), CLI + MCP stdio + browser session client, and controlled paired trials (30 synthetic pairs verified + 216 frozen evaluation runs).
- **[QAsystem](https://github.com/Tak1naa/QAsystem):** Built an EMU train maintenance question-understanding and routing prototype classifying 8 question types and 6 entity categories into structured JSON (`RAG`, `KG`, `CLARIFY`, `OUT_OF_SCOPE`) across rule-based, LLM, and hybrid modes with automatic rule fallback and offline `pytest` evaluation.

### Linux Desktop, CLI & Self-Hosted Infrastructure

- **[PackPort](https://github.com/Tak1naa/PackPort):** Built a GTK4 / Libadwaita drag-and-drop package installer for Fedora supporting RPM, DEB (via Alien + DNF dependency checks), AppImage, and Flatpak, separating an unprivileged UI from a restricted Polkit helper executing fixed subcommands.
- **[SpeedTest](https://github.com/Tak1naa/SpeedTest):** Extended LibreSpeed / `bg6cq` into a hardened, bilingual self-hosted speed test with HAProxy HTTPS ingress, Redis atomic session admission and sliding-window rate limits, bounded transfers, disabled telemetry, and an opt-in anonymized 7-day leaderboard.
- **[TokenMon](https://github.com/Tak1naa/Tokenmon):** Created a Tauri / Rust desktop-pet monitor (native WebView2/WebKit + system tray) plus a standalone Python diagnostic CLI that polls LiteLLM, OpenRouter, DeepSeek balance, or custom JSON gateways for token, cache, cost, and balance data without invoking models.
- **[netease-music-codex](https://github.com/Tak1naa/netease-music-codex):** Built a Codex-oriented music control skill wrapping `ncm-cli` with Linux desktop `mpv` + PipeWire/PulseAudio playback adaptation and runtime state verification.

### Urban Spatial Data / GIS & Web Practice *(Independent Track)*

- **Urban Spatial Data Processing (Internship):** Completed multi-source population grid, map, and building data cleaning, coordinate unification, spatial joins, sub-district aggregation, satellite imagery processing, and quality checks under strict data desensitization requirements.
- **CycleRoute (Local Workbench):** Maintained a browser-first cycling routebook workspace using Spring Boot, React, AMap, and BRouter, handling WGS84 / GCJ-02 boundary conversion, multi-format track import/export (GPX/TCX/FIT/KML/GeoJSON), and optional client-side AES-GCM temporary sharing.
- **[Personal Blog](https://github.com/Tak1naa/blog):** Extended Hexo 7 + Solitude 4 with an independent TypeScript enhancement layer (PJAX lifecycle integration, Howler.js audio player, opt-in custom-rigged Live2D, Waline + PostgreSQL comments, and reduced-motion fallbacks).

---

<a id="experience"></a>

## Education & Experience

### Beijing Jiaotong University
**B.Eng. in Computer Science and Technology (Railway Information Technology)**  
*September 2024 – July 2028 (Expected)*

- Core coursework and systems practice spanning Java, C/C++, data structures, operating systems, compilers, machine learning, and RISC-V SoC/FPGA labs (`NEMU`, `Verilator`, `Vivado`).
- English proficiency: CET-4 (575) · CET-6 (488).

### Beijing Urban Construction Design & Development Group *(R&D Intern)*
**Urban Spatial Data & GIS Engineering**  
*July 2026 – October 2026 (Agreement Period)*

- Processed multi-source population grids, maps, and building datasets: schema cleaning, coordinate system unification, spatial joins, sub-district aggregation, and QA checks.
- Contributed to satellite imagery processing and building-attribute fusion while adhering to confidentiality and data-desensitization standards.

### Undergraduate Innovation & Engineering Practice
**Research & Software Training Projects**  
*2026*

- **Agent-Harness (Undergraduate Innovation Project):** Problem decomposition, harness architecture, static/dynamic isolation, code review, and paired experiment verification.
- **Cafeteria-Management & QAsystem (Engineering & Practice Courses):** End-to-end Spring Boot multi-service integration and domain-specific NLP/rule routing prototypes.

---

<a id="projects"></a>

## Selected Projects

| Project | What It Demonstrates | Technologies | Status |
| --- | --- | --- | --- |
| [Cafeteria-Management](https://github.com/Tak1naa/Cafeteria-Management) | Spring Boot integration across C++ engine, WebSocket UI, DB, cache, and MQ | Java, Spring Boot, C++, MySQL, Redis, RabbitMQ | Course Project |
| [TiCenter](https://github.com/Tak1naa/TiCenter) | File-first AI question workspace, hybrid RAG (BM25 + vector), SSE citations | Java, Spring Boot, React, TypeScript, Python, Qdrant | Snapshot (Paused) |
| [Agent-Harness](https://github.com/Tak1naa/Agent-Harness) | Static-guided LLM security test synthesis, rootless Podman isolation, paired eval | Python, Bandit, AST, pytest, Hypothesis, Podman, MCP | Research Prototype |
| [PackPort](https://github.com/Tak1naa/PackPort) | Privilege-separated Fedora desktop package installer with DNF/Flatpak workflows | Python, GTK4, Libadwaita, Polkit, DNF | Active Tool |
| [SpeedTest](https://github.com/Tak1naa/SpeedTest) | Hardened self-hosted web service with Redis atomic rate limits & Docker Compose | PHP, Redis, HAProxy, Docker Compose, JS | Live Service |
| [TokenMon](https://github.com/Tak1naa/Tokenmon) | Lightweight native desktop monitoring & gateway balance/token diagnostics | Rust, Tauri, TypeScript, Python | Desktop App |
| [QAsystem](https://github.com/Tak1naa/QAsystem) | Domain intent/entity extraction, structured JSON routing, offline pytest suite | Python, Streamlit, DeepSeek API, pytest | Course Prototype |
| [netease-music-codex](https://github.com/Tak1naa/netease-music-codex) | Agent skill integration with Linux desktop audio session & state checks | Markdown Skill, `ncm-cli`, `mpv`, PipeWire | Utility Skill |
| [blog](https://github.com/Tak1naa/blog) | Modular TypeScript frontend enhancements & self-hosted comment stack | TypeScript, Hexo, Solitude, Waline, PostgreSQL | Live Site |

---

<a id="stack"></a>

## Technology Stack

**Backend & Integration:** Java, Spring Boot, HTTP REST, WebSocket, SSE, Flyway  
**Databases & Messaging:** MySQL, PostgreSQL, Redis, RabbitMQ, Qdrant  
**AI, RAG & Evaluation:** Python, Bandit, AST analysis, pytest, Hypothesis, DeepSeek / OpenAI-compatible APIs, MCP stdio, hybrid retrieval (BM25 + vector / RRF)  
**Frontend & Desktop:** TypeScript, React, HTML5 / CSS3, GTK4 / Libadwaita, Tauri / Rust, Streamlit  
**Systems & Infrastructure:** Linux (Fedora / Debian), Docker / Docker Compose, rootless Podman, HAProxy, nginx, Polkit, Git  
**Additional Foundations:** C / C++ (CMake), RISC-V / Verilator / NEMU (coursework), GIS & spatial data processing (separate domain track)

---

<a id="fit"></a>

## Best-Fit Roles

- **Java Backend Engineer (Intern):** Business services, REST/WebSocket APIs, relational/cache/MQ integration, and maintainable engineering workflows.
- **AI Infra / LLM Application Engineer (Intern):** Model gateway tooling, RAG pipelines, agent execution sandboxes, and reproducible evaluation harnesses.
- **Backend / Full-Stack Tools Engineer:** Internal developer workbenches, browser clients, cross-language service orchestration, and technical documentation.
- **Linux Systems & Tooling Engineer:** Desktop/CLI utilities, privilege-isolated helpers, containerized self-hosting, and runtime diagnostics.

---

## Editions & Languages

- [简体中文 (Main)](./README.zh-CN.md) — 中文主简历版
- [R&D Version (English)](./README.rnd.md) — System profile, Mermaid architecture maps, collapsible technical breakdowns, and full project matrix
- [R&D 版本 (简体中文)](./README.rnd.zh-CN.md) — 极客 / 研发全景中文版

> 2026 · Zili Ying (Tak1naa)
