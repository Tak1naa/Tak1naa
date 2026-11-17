<h1 align="center">Zili Ying · Takina</h1>

<p align="center">
  Java Backend Development · Linux Tooling · AI Applications
</p>

<p align="center">
  <a href="#中文">中文</a> · <a href="#english">English</a> ·
  <a href="https://github.com/Tak1naa?tab=repositories">Repositories</a> ·
  <a href="https://github.com/Tak1naa/blog">Blog Source</a>
</p>

## 中文

主要方向为 **Java 后端开发**，并围绕文档处理、桌面工具与网络服务开展项目实践。关注服务间接口、数据流、异常处理与运行验证，使用 Python 和 TypeScript 完成配套服务、自动化工具及前端交互。

### 代表项目

**[Cafeteria-Management · 智能食堂仿真系统](https://github.com/Tak1naa/Cafeteria-Management)**  
以 Spring Boot 作为业务与集成层，连接 C++ 仿真引擎与 Web 客户端；使用 MySQL 保存业务数据、Redis 提供缓存、RabbitMQ 处理异步消息，并通过 WebSocket 推送仿真状态。项目覆盖排队与就餐仿真、参数控制及调度决策，属于软件实训项目。

**[TiCenter · 题枢](https://github.com/Tak1naa/TiCenter)**  
面向题目文件阅读、上下文选择、检索与 AI 对话的文档工作台。采用 Spring Boot、React / TypeScript 与 Python AI 服务，围绕多文件工作区、选区上下文和引用回跳组织交互。当前为暂停开发的进度快照，文档检索与 OCR 迁移、跨服务验收尚未完成。

**[Agent-Harness · 代码智能体安全测试](https://github.com/Tak1naa/Agent-Harness)**  
研究程序分析信息对模型生成安全测试的影响，结合 Bandit / AST 分析、受限 pytest / Hypothesis 测试与 rootless Podman 隔离执行。以真实副作用取证、配对样本和实验记录支持结果复核；项目定位为研究原型，工程验证与模型效果分别报告。

**[PackPort · Fedora 软件包安装器](https://github.com/Tak1naa/PackPort)**  
基于 Python 与 GTK4 / Libadwaita 的桌面工具，为 RPM、DEB、AppImage 和 Flatpak 提供统一的拖放安装入口。按软件包类型处理安装流程、权限边界和错误反馈；DEB 转换后仍由 DNF 检查依赖，兼容性取决于具体软件包。

**[SpeedTest · 自托管网络测速](https://github.com/Tak1naa/SpeedTest)**  
基于 LibreSpeed / bg6cq 二次开发，保留上游测速引擎，补充双语界面、Redis 会话准入与限流、有界传输及 Docker Compose 部署配置。工程重点包括并发资源约束、异常释放、隐私处理与部署边界。

**[TokenMon · 模型用量桌面监视器](https://github.com/Tak1naa/Tokenmon)**  
使用 Tauri / Rust 与 Web 前端，将网关提供的 Token、缓存、费用和余额数据呈现在可展开的桌面面板中，并以桌面宠物作为交互入口。另提供 Python 诊断 CLI；数据轮询本身不触发模型调用。

### 其他项目与实践

- **CycleRoute · 骑行路书：** 在开发机上维护的路书工作台，使用 Spring Boot、React、高德地图与 BRouter，涉及路线规划、海拔展示、坐标转换和多格式轨迹导入导出。路书编辑在浏览器完成，用户主动分享时上传临时密文。GIS 与路线数据处理是独立的应用实践方向。
- **[netease-music-codex](https://github.com/Tak1naa/netease-music-codex)：** 基于 ncm-cli / mpv 的音乐控制 skill，处理 Linux 桌面音频会话适配与播放状态验证。
- **[个人博客](https://github.com/Tak1naa/blog)：** 基于 Hexo / Solitude 的扩展实践，包括 TypeScript 动态组件、音乐播放器、Live2D 和页面生命周期适配。

### 技术与工程实践

- **后端与数据：** Java、Spring Boot、MySQL、Redis、RabbitMQ、HTTP / WebSocket。
- **应用与工具：** Python、TypeScript、React、GTK4 / Libadwaita、Tauri / Rust。
- **运行与验证：** Linux、Git、Docker / Podman、自动化测试与浏览器回归。

方案设计优先评估成熟开源组件与项目已有能力；实现过程中关注接口约定、异常路径和资源边界。交付时保留验证记录、已知限制与待完成项，按实际测试范围描述结果。

使用 AI 辅助开展需求分析、架构选择、代码实现与审查，并通过测试、实际运行和交付物检查验证改动。

---

## English

My primary focus is **Java backend development**, with project work in document processing, desktop tooling, and network services. I work on service interfaces, data flow, error handling, and runtime verification, using Python and TypeScript for supporting services, automation, and frontend interaction.

### Selected Projects

**[Cafeteria-Management · Cafeteria Simulation System](https://github.com/Tak1naa/Cafeteria-Management)**  
A software training project with Spring Boot as the application and integration layer between a C++ simulation engine and Web clients. It uses MySQL for persistence, Redis for caching, RabbitMQ for asynchronous messaging, and WebSocket for simulation updates, covering queueing, dining, parameter control, and scheduling decisions.

**[TiCenter · AI-Assisted Question Bank Workspace](https://github.com/Tak1naa/TiCenter)**  
A document workspace for reading question files, selecting context, retrieving information, and interacting with AI. Built with Spring Boot, React / TypeScript, and Python AI services, with multi-file navigation, selection-based context, and navigation back to cited sources. Development is paused; retrieval and OCR migration and cross-service acceptance testing remain incomplete.

**[Agent-Harness · Security Testing for Code Agents](https://github.com/Tak1naa/Agent-Harness)**  
A research prototype investigating how program analysis informs model-generated security tests. It combines Bandit / AST analysis, restricted pytest / Hypothesis tests, and isolated execution with rootless Podman. Side-effect evidence, paired samples, and experiment records support review; engineering validation and model effectiveness are reported separately.

**[PackPort · Fedora Package Installer](https://github.com/Tak1naa/PackPort)**  
A Python and GTK4 / Libadwaita desktop tool providing a shared drag-and-drop entry point for RPM, DEB, AppImage, and Flatpak packages. Installation flows, privilege boundaries, and error reporting are handled by package type. Converted DEB packages still undergo DNF dependency checks, and compatibility depends on the individual package.

**[SpeedTest · Self-Hosted Network Speed Test](https://github.com/Tak1naa/SpeedTest)**  
An extension of LibreSpeed / bg6cq that retains the upstream measurement engine and adds a bilingual interface, Redis-backed session admission and rate limits, bounded transfers, and Docker Compose deployment configuration. Engineering work addresses concurrency limits, resource release on failure, privacy, and deployment boundaries.

**[TokenMon · Desktop Model Usage Monitor](https://github.com/Tak1naa/Tokenmon)**  
A Tauri / Rust application with a Web frontend, displaying gateway-provided token, cache, cost, and balance data in an expandable desktop panel with a pet-style interaction model. A Python diagnostic CLI is also available; polling usage data does not itself invoke a model.

### Additional Projects and Practice

- **CycleRoute · Cycling Routebook:** A locally maintained workspace using Spring Boot, React, AMap, and BRouter for route planning, elevation display, coordinate conversion, and multi-format track import and export. Routebook editing takes place in the browser; temporary ciphertext is uploaded only when the user chooses to share. GIS and route data processing form a separate area of application work.
- **[netease-music-codex](https://github.com/Tak1naa/netease-music-codex):** A music-control skill built on ncm-cli / mpv, covering Linux desktop audio session integration and playback-state verification.
- **[Personal Blog](https://github.com/Tak1naa/blog):** Extensions to Hexo / Solitude, including TypeScript dynamic components, a music player, Live2D, and page lifecycle integration.

### Technologies and Engineering Practice

- **Backend and data:** Java, Spring Boot, MySQL, Redis, RabbitMQ, HTTP / WebSocket.
- **Applications and tooling:** Python, TypeScript, React, GTK4 / Libadwaita, Tauri / Rust.
- **Runtime and verification:** Linux, Git, Docker / Podman, automated tests, and browser regression testing.

I evaluate established open-source components and existing project capabilities when choosing an approach. Implementation work addresses interface contracts, failure paths, and resource boundaries. Deliverables include verification records, known limitations, and outstanding work, with results described within the scope actually tested.

I use AI assistance for requirements analysis, architecture decisions, implementation, and code review, and verify changes through tests, runtime checks, and inspection of deliverables.
