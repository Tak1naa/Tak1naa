<div align="center">
  <strong>语言 / 版本：</strong>
  <strong>简体中文（当前）</strong>
  ·
  <a href="./README.md">English</a>
  ·
  <a href="./README.rnd.zh-CN.md">R&amp;D 中文版</a>
  ·
  <a href="./README.rnd.md">R&amp;D Version</a>
</div>

<br>

<div align="center">
  <h1>
    你好，我是 立立子（Takina）
  </h1>
  <h3>
    Java 后端开发 • AI 工程与安全评测 • Linux 系统工具
  </h3>
  <p>
    关注契约清晰的后端集成、可复现的 LLM 评测沙箱，以及 Linux 桌面与自托管基础设施工具
  </p>
  <p>
    <b>Java</b> • <b>Spring Boot</b> • Python • TypeScript • React • Linux • Docker / Podman • MySQL • Redis • RabbitMQ
  </p>
</div>

---

<div align="center">
  <a href="#profile">个人简介</a> ·
  <a href="#value">团队价值</a> ·
  <a href="#highlights">工程实践</a> ·
  <a href="#experience">教育与经历</a> ·
  <a href="#projects">代表项目</a> ·
  <a href="#stack">技术栈</a> ·
  <a href="#fit">适配方向</a>
</div>

---

<a id="profile"></a>

## 个人简介

我是**北京交通大学**计算机科学与技术（铁路信息技术）专业本科生（2024 级，预计 2028 年毕业），技术实践围绕 **Java 后端开发**、**AI 应用与评测基础设施** 以及 **Linux 系统工具** 展开。

在工程交付中，我重视“把模糊需求收敛为可验证的软件”：明确服务间接口契约、守住运行权限与资源边界，并坚持按实际测试范围报告结果，将已知限制与待验收项显式保留在文档与仓库中。

- **主攻方向：** Java / Spring Boot 业务与集成层开发、MySQL / Redis / RabbitMQ 数据流转、HTTP / WebSocket / SSE 接口联调与 Linux 部署。
- **AI 工程与评测：** RAG 检索链路、rootless Podman 隔离沙箱与配对对照评测。在 AI 辅助编程中，主要负责需求拆解、架构与技术选型、代码审查、运行验证和交付把关。
- **公开项目沉淀：** 在 GitHub 维护 10+ 公开仓库，覆盖多服务后端平台、代码智能体安全测试原型、Fedora/GTK4 与 Tauri/Rust 桌面工具及自托管网络服务。
- **独立应用方向：** 城市空间数据 / GIS 处理与骑行路书工具，作为独立应用方向维护，与 Java 后端核心证据清晰区分。

**GitHub：** [github.com/Tak1naa](https://github.com/Tak1naa)  
**仓库列表：** [github.com/Tak1naa?tab=repositories](https://github.com/Tak1naa?tab=repositories)  
**个人博客：** [tak1na.top/blog](https://tak1na.top/blog)  
**在线服务：** [tak1na.top/speedtest](https://tak1na.top/speedtest/)  
**所在城市：** 中国 · 北京

---

<a id="value"></a>

## 能为团队带来的价值

在工程团队中，我尤其适合承担以下工作：

- **Java / Spring Boot 后端集成：** 设计并维护接口契约，结合 MySQL、Redis 缓存、RabbitMQ 异步消息及 WebSocket / SSE 推进业务落地；
- **跨语言与异构系统联调：** 通过清晰的 HTTP/JSON 协议衔接 Java、C++、Python 与 TypeScript 模块，并保留规则引擎或降级路径；
- **AI 评测与检索基础设施：** 搭建带真实副作用探针、隔离容器、配对样本与结构化日志的评测脚手架，区分工程验证与模型效果；
- **Linux 服务封装与安全边界：** 基于 Docker Compose、rootless Podman、HAProxy 与 Polkit 权限分离完成服务部署与限流加固；
- **可追溯的工程交付：** 保留回归测试、运行日志、架构说明与未完成边界，避免“口头完成”或过度外推实验结论。

---

<a id="highlights"></a>

## 核心工程实践

### Java 后端与多服务集成

- **[Cafeteria-Management · 智能食堂仿真系统](https://github.com/Tak1naa/Cafeteria-Management)：** 以 Spring Boot 作为核心业务与集成层，通过 HTTP/JSON 连接 C++ 仿真引擎，通过 WebSocket/HTTP 服务 Web 前端，集成 MySQL、Redis、RabbitMQ 及可选 DeepSeek API（未启用时回退规则引擎），完成软件实训全流程联调。
- **[TiCenter · 题枢（AI 题库工作台）](https://github.com/Tak1naa/TiCenter)：** 围绕题目文件阅读、多文件工作区、选区上下文与引用回跳组织设计；采用 Spring Boot、React / TypeScript、MySQL、Redis、Qdrant 与 Python AI 服务，实现 BM25 + 向量检索 RRF 融合与 SSE 流式回答*（当前为暂停开发的进度快照，跨服务 OCR / Qdrant 迁移与真实验收待完成）*。

### AI 工程、检索与安全评测

- **[Agent-Harness · 代码智能体安全测试原型](https://github.com/Tak1naa/Agent-Harness)：** 面向大创项目的研究原型，研究在相同模型、工具与调用上限下，Bandit 告警与 AST 函数上下文对模型生成 Python 安全测试有效性的影响。集成受限 `pytest` / `Hypothesis` 测试生成、rootless Podman 隔离执行、真实副作用探针（路径穿越、命令注入、SQL 注入）、CLI / MCP stdio / 浏览器会话客户端，已完成 30 组配对样本工程验证与 216 次冻结对照试验。
- **[QAsystem · 动车检修问题理解与处理建议系统](https://github.com/Tak1naa/QAsystem)：** 面向铁路信息技术专业实践的原型系统，支持 8 类问题识别、6 类实体抽取与归一化，在纯规则、LLM 与混合模式下输出统一 JSON 路由标签（`RAG`、`KG`、`CLARIFY`、`OUT_OF_SCOPE`），LLM 不可用时自动回退规则引擎，并配套离线 `pytest` 验收。

### Linux 桌面、CLI 与自托管基础设施

- **[PackPort · Fedora 软件包安装器](https://github.com/Tak1naa/PackPort)：** 基于 Python 与 GTK4 / Libadwaita 构建的本地包拖放安装器，统一支持 RPM、DEB（经 Alien 转换并交由 DNF 检查依赖）、AppImage 与 Flatpak；普通用户运行界面，系统级安装通过受限 Polkit helper 执行固定子命令，并记录安装队列与事务日志。
- **[SpeedTest · 自建网络测速站](https://github.com/Tak1naa/SpeedTest)：** 基于 LibreSpeed / `bg6cq` 二次开发，引入 HAProxy HTTPS 入口、Redis 原子会话准入与滑动窗口限流、有界传输、传输错误检查，并关闭上游遥测与结果库，提供可主动提交与撤回的脱敏七日排行。
- **[TokenMon · 桌面端模型用量监视器](https://github.com/Tak1naa/Tokenmon)：** 使用 Tauri / Rust（调用系统原生 WebView2 / WebKit 与系统托盘）与 Web 前端打造桌面宠物式监控面板，另附 Python 诊断 CLI；支持轮询 LiteLLM、OpenRouter、DeepSeek 余额及自定义 JSON 网关，轮询本身不触发模型调用。
- **[netease-music-codex](https://github.com/Tak1naa/netease-music-codex)：** 面向 Codex 的网易云音乐 skill，封装 `ncm-cli` 并适配 Linux 桌面 `mpv` + PipeWire/PulseAudio 音频会话与播放状态校验。

### 城市空间数据 / GIS 与 Web 实践 *（独立应用方向）*

- **城市空间数据处理（实习实践）：** 参与多源人口网格、地图与建筑数据的清洗、坐标统一、空间关联、街道尺度汇总、卫星影像处理与质量检查，严格落实业务地点与原始数据脱敏规范。
- **CycleRoute · 骑行路书（本地维护工作台）：** 基于 Spring Boot、React、高德地图与 BRouter 的隐私优先路书工具，处理 WGS84 / GCJ-02 坐标边界转换与浏览器端多格式轨迹（GPX/TCX/FIT/KML/GeoJSON）导入导出，支持用户主动分享时上传临时密文。
- **[个人博客](https://github.com/Tak1naa/blog)：** 基于 Hexo 7 与 Solitude 4 搭建并持续维护，独立编写 TypeScript 动态增强层，涵盖 PJAX 生命周期管理、Howler.js 播放器、按需启用的 Live2D 看板娘、Waline + PostgreSQL 评论及减弱动画降级策略。

---

<a id="experience"></a>

## 教育与实践经历

### 北京交通大学
**计算机科学与技术（铁路信息技术） | 本科**  
*2024.09 – 2028.07（预计）*

- 系统学习 Java、C/C++、数据结构、操作系统、编译原理、机器学习及 RISC-V SoC/FPGA 综合实训（`NEMU`、`Verilator`、`Vivado`）。
- 英语能力：CET-4 575 分 · CET-6 488 分。

### 北京城建交通设计研究院有限公司
**研发实习生 | 城市空间数据与 GIS 工程**  
*2026.07 – 2026.10（协议期限）*

- 承担多源人口网格、地图与建筑数据的清洗、坐标统一、空间关联、街道尺度汇总及质量核查，输出合规 GIS 分析成果。
- 参与卫星影像处理与建筑信息融合，按保密要求完成业务地点及原始数据脱敏。

### 大学生创新项目与专业实训
**研究与工程实践**  
*2026*

- **Agent-Harness（大创项目）：** 参与研究问题拆解、Harness 架构设计、静态分析与容器沙箱整合、代码审查及配对对照试验验证。
- **Cafeteria-Management / QAsystem（实训项目）：** 负责 Spring Boot 多服务后端整合、异构通信协议联调及领域问答原型评测。

---

<a id="projects"></a>

## 代表项目总览

| 项目 | 核心工程能力证明 | 主要技术栈 | 当前状态 |
| --- | --- | --- | --- |
| [Cafeteria-Management](https://github.com/Tak1naa/Cafeteria-Management) | Spring Boot 串联 C++ 引擎、WebSocket 前端与 MySQL/Redis/MQ | Java, Spring Boot, C++, MySQL, Redis, RabbitMQ | 实训交付 |
| [TiCenter（题枢）](https://github.com/Tak1naa/TiCenter) | 文件优先工作区、混合检索（BM25+向量 RRF）、SSE 引用回跳 | Java, Spring Boot, React, TypeScript, Python, Qdrant | 进度快照（暂停） |
| [Agent-Harness](https://github.com/Tak1naa/Agent-Harness) | Bandit/AST 上下文引导、rootless Podman 隔离、配对安全评测 | Python, Bandit, AST, pytest, Hypothesis, Podman, MCP | 研究原型 |
| [PackPort](https://github.com/Tak1naa/PackPort) | Linux 桌面权限分离（Polkit helper）、多格式安装包工作流 | Python, GTK4, Libadwaita, Polkit, DNF | 桌面工具 |
| [SpeedTest](https://github.com/Tak1naa/SpeedTest) | 自托管网络服务加固、Redis 原子限流与 Docker Compose 部署 | PHP, Redis, HAProxy, Docker Compose, JS | 在线运行 |
| [TokenMon](https://github.com/Tak1naa/Tokenmon) | 原生轻量桌面监控面板与模型网关余额/Token 诊断 | Rust, Tauri, TypeScript, Python | 桌面应用 |
| [QAsystem](https://github.com/Tak1naa/QAsystem) | 领域意图/实体抽取、统一 JSON 路由与离线自动化回归测试 | Python, Streamlit, DeepSeek API, pytest | 课程原型 |
| [netease-music-codex](https://github.com/Tak1naa/netease-music-codex) | Agent Skill 封装与 Linux 桌面音频会话状态校验 | Skill, `ncm-cli`, `mpv`, PipeWire | 效率工具 |
| [blog](https://github.com/Tak1naa/blog) | 独立 TypeScript 前端增强架构与自托管评论服务 | TypeScript, Hexo, Solitude, Waline, PostgreSQL | 在线站点 |

---

<a id="stack"></a>

## 技术栈

**后端与接口集成：** Java, Spring Boot, HTTP REST, WebSocket, SSE, Flyway  
**数据库与中间件：** MySQL, PostgreSQL, Redis, RabbitMQ, Qdrant  
**AI 工程与评测：** Python, Bandit, AST 分析, pytest, Hypothesis, DeepSeek / OpenAI 兼容接口, MCP stdio, 混合检索（BM25 + 向量 / RRF）  
**前端与桌面开发：** TypeScript, React, HTML5 / CSS3, GTK4 / Libadwaita, Tauri / Rust, Streamlit  
**系统与运维：** Linux (Fedora / Debian), Docker / Docker Compose, rootless Podman, HAProxy, nginx, Polkit, Git  
**其他基础：** C / C++ (CMake), RISC-V / Verilator / NEMU（课程实训）, 城市空间数据 / GIS 处理（独立方向）

---

<a id="fit"></a>

## 适配岗位方向

- **Java 后端开发实习生：** 业务服务开发、REST / WebSocket 接口设计、MySQL / Redis / RabbitMQ 集成与工程化测试。
- **AI Infra / 大模型应用研发实习生：** 模型网关诊断与监控、RAG 检索链路、Agent 隔离沙箱与可复现评测体系。
- **全栈工具 / 平台工程实习生：** 内部工作台、跨语言服务编排、浏览器端交互与工程文档沉淀。
- **Linux 系统与开发效率工具工程师：** 桌面/CLI 工具、最小权限隔离封装与容器化自托管服务维护。

---

## 其他版本与语言

- [English (Main)](./README.md) — 英文主简历版
- [R&D 中文版](./README.rnd.zh-CN.md) — 系统画像、Mermaid 架构图谱、可折叠工程细节与完整项目矩阵
- [R&D Version (English)](./README.rnd.md) — 极客 / 研发全景英文版

> 2026 · 应子立 (Tak1naa)
