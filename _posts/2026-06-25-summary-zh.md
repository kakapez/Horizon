---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> From 62 items, 18 important content pieces were selected

---

1. [OpenAI unveils its first custom chip, built by Broadcom](#item-1) ⭐️ 9.0/10
2. [高通以 40 亿美元收购 Modular 及 Mojo](#item-2) ⭐️ 8.0/10
3. [ThinkPRM 发布：大模型推理过程质量终于可量化](#item-3) ⭐️ 8.0/10
4. [Databricks 技术领袖倡导开放前沿生态系统与 Agent Cloud](#item-4) ⭐️ 8.0/10
5. [Bunny DNS 宣布免费，挑战 Cloudflare](#item-5) ⭐️ 7.0/10
6. [Google 为 Gemini 3.5 Flash 添加计算机使用能力](#item-6) ⭐️ 7.0/10
7. [NVIDIA 45°C 液冷设计将数据中心用水量降至近零](#item-7) ⭐️ 7.0/10
8. [Nub：类似 Bun 的开发体验工具包，增强原生 Node.js](#item-8) ⭐️ 7.0/10
9. [Rust 正推进移除 crates.io 发布对 GitHub 的依赖](#item-9) ⭐️ 7.0/10
10. [Claude 在 Slack 中获得多人协作、主动式、持久化智能体升级](#item-10) ⭐️ 7.0/10
11. [IETF 标准化新的 HTTP QUERY 方法](#item-11) ⭐️ 7.0/10
12. [用 8 个数据库和 disable_joins 将 Rails 扩展至每小时 4100 万请求](#item-12) ⭐️ 7.0/10
13. [RRB-Tree：支持快速拼接的高效不可变向量](#item-13) ⭐️ 7.0/10
14. [MDN 发布官方 MCP 服务器，支持 AI 直接访问文档](#item-14) ⭐️ 7.0/10
15. [Cloudflare 详细记录在 hyper Rust HTTP 库中发现并调试 Bug 的过程](#item-15) ⭐️ 7.0/10
16. [Ben Thompson 的 Vibe Coding 体验与十条心得](#item-16) ⭐️ 7.0/10
17. [Nature 论文质疑微软 Majorana 1 量子计算声明](#item-17) ⭐️ 7.0/10
18. [Google 在全球开放 Play Store 第三方支付](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI unveils its first custom chip, built by Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI announces its first custom inference chip 'Jalapeno' designed in partnership with Broadcom and manufactured by TSMC, claiming a nine-month development cycle accelerated by their own AI models.

hackernews · jamdesk · Jun 24, 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**标签**: `#ai-hardware`, `#custom-silicon`, `#openai`, `#broadcom`, `#inference-chips`

---

<a id="item-2"></a>
## [高通以 40 亿美元收购 Modular 及 Mojo](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 8.0/10

高通正在以约 40 亿美元收购 Modular 公司——即 Mojo 编程语言和 MAX 平台背后的 AI 基础设施公司，这一消息已由双方在 2026 年 6 月的官方公告中确认。 此次收购标志着高通从移动和边缘芯片向 AI 计算基础设施的重大战略推进，将 Chris Lattner 世界级的编译器专长引入高通的硬件生态系统，并可能重塑高通多样化芯片产品线上 AI 软件栈的构建方式。 Mojo 基于 MLIR 而非 LLVM 构建，能够面向 CPU、GPU、TPU、ASIC 及其他加速器生成代码，这与高通异构计算的雄心高度契合；Modular 还提供用于加速 AI 执行的 MAX 平台；考虑到 Lattner 过去曾公开批评硬件公司的 AI 软件栈，这笔交易颇具讽刺意味。

hackernews · timmyd · Jun 24, 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Modular 公司由 Chris Lattner 创立，他是 LLVM 和 Apple Swift 编程语言的创造者，其使命是通过统一碎片化的软件栈来加速 AI 计算。该公司开发了 Mojo 编程语言，将 Python 的易用性与 C++和 Rust 等系统级语言的高性能相结合，通过基于 MLIR 的编译器基础设施专门为 AI 工作负载进行了优化。Modular 还创建了 MAX（Modular Accelerated Execution）平台，用于在异构硬件上高效部署和运行 AI 模型。高通一直在战略性地组建技术产品组合——包括与 Tenstorrent、Ventana 和 Alphawave 相关的投资——旨在从 ARM 转向 RISC-V，并在移动和边缘设备芯片之外的 AI 计算领域具备竞争力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://mojolang.org/">Mojo - Modular</a></li>

</ul>
</details>

**社区讨论**: 社区对此次收购表达了复杂的感受，许多人指出考虑到 Lattner 过去对硬件公司 AI 栈的批评，Modular 被一家硬件公司收购颇具讽刺意味。一些人质疑高通的动机，因为与 NVIDIA 的 Hopper H100/H200 相比，高通缺乏高端推理/训练产品；而另一些人则认为这是高通超越 ARM 并在 AI 计算领域竞争的更广泛战略组合的一部分。少数人表示失望，认为 Lattner 把精力放在让 Mojo 像 Python 上，而不是追求更具创新性的方向。

**标签**: `#ai-infrastructure`, `#acquisition`, `#mojo`, `#qualcomm`, `#chris-lattner`

---

<a id="item-3"></a>
## [ThinkPRM 发布：大模型推理过程质量终于可量化](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247899199&idx=3&sn=b0d6764e50d881295fd85b75f8f9434a) ⭐️ 8.0/10

ThinkPRM（思考奖励模型）正式发布，这是一种通过生成长思维链来量化大模型推理过程而非仅评估最终结果的生成式过程奖励模型，该工作获得了 ICML'26 Oral 接收，并在 GitHub 上获得了超过 4.2k 星标。 这一工作解决了评估推理型大模型的关键瓶颈——正确答案可能源于有缺陷的推理过程。通过实现细粒度的过程级评估，ThinkPRM 为 DeepSeek-R1 和 OpenAI o1 等推理模型的更好训练、对齐和验证打开了大门。 ThinkPRM 仅使用了 PRM800K 中 1%的过程标注数据，却在 ProcessBench、MATH-500 和 AIME '24 等基准测试上的 best-of-N 选择和奖励引导搜索中超越了 LLM-as-a-Judge 和判别式验证器。ThinkPRM-7B 模型基于 DeepSeek-R1-Distill-Qwen-7B，并在其自定义验证数据上进行了微调。

rss · 量子位 · Jun 24, 04:00

**背景**: 过程奖励模型（PRM）评估推理链中每个中间步骤的质量，而非仅判断最终答案的结果奖励模型（ORM）。传统判别式 PRM 需要大量步骤级标注数据，构建成本高昂。ThinkPRM 引入了生成式方法，模型通过生成自己的验证思维链来评估每个步骤，在大幅减少数据需求的同时提升了验证质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2504.16828">[2504.16828] Process Reward Models That Think</a></li>

</ul>
</details>

**社区讨论**: 该项目在 GitHub 上获得了超过 4.2k 星标，吸引了大量社区关注，反映出社区对过程级奖励建模作为评估和改进推理模型关键工具的浓厚兴趣。

**标签**: `#llm-reasoning`, `#reward-model`, `#process-reward`, `#icml`, `#evaluation`

---

<a id="item-4"></a>
## [Databricks 技术领袖倡导开放前沿生态系统与 Agent Cloud](https://www.latent.space/p/databricks) ⭐️ 8.0/10

Databricks 首席技术官 Matei Zaharia 与首席架构师 Reynold Xin 发布了一次罕见的联合访谈，详细阐述了他们对开放前沿生态系统的战略愿景。他们概述了企业将如何使用 Databricks 的新产品 Agent Bricks 组合各种 AI Agent，从而构建和运营 Agent Cloud。 这一愿景标志着企业 AI 的重大范式转变，即从孤立的模型转向互联的工具调用 Agent 系统，从而将 Databricks 定位为核心平台提供商。开放生态系统的方法可防止供应商锁定，并允许企业在统一且优化的 Agent 框架内组合 OpenAI 和 Claude 等多种模型。 讨论重点介绍了 Databricks 的 Agent Bricks 产品，该产品可自动评估、微调并优化各种 AI 模型，从而使用 Claude Code 和 Codex 等工具组合工作流。这也建立在 Databricks 近期开源 Unity Catalog 的举措之上，解决了数据互操作性限制的最后前沿问题。

rss · Latent Space · Jun 24, 18:53

**背景**: Databricks 于 2013 年由 Apache Spark 的原始创建者创立，已从数据分析平台发展为全面的 AI 数据智能平台。随着企业超越简单的聊天机器人，转向能够执行任务和调用外部工具的复杂 AI Agent，对管理这些 Agent、确保数据治理并防止专有锁定的基础设施的需求日益增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.databricks.com/product/artificial-intelligence/agent-bricks">Agent Bricks | Databricks</a></li>
<li><a href="https://medium.com/starrocks-engineering/why-did-databricks-open-source-unity-catalog-b228bd9be367">Why Did Databricks Open - Source Unity Catalog? | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Databricks">Databricks - Wikipedia</a></li>

</ul>
</details>

**标签**: `#databricks`, `#ai-agents`, `#open-source`, `#data-engineering`, `#interview`

---

<a id="item-5"></a>
## [Bunny DNS 宣布免费，挑战 Cloudflare](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 7.0/10

Bunny.net 完全取消了 DNS 查询费用，并为每个账户提供最多 500 个域名的免费 DNS 托管服务，没有查询限制、没有按请求计费，所有功能（包括智能记录和健康监控）均免费包含在内。 此举通过消除不可预测的按查询计费模式，显著颠覆了 DNS 托管市场，并在欧洲对美国云基础设施依赖日益担忧的背景下，将 Bunny.net 定位为 Cloudflare 的强劲欧盟替代方案。 虽然 DNS 本身现在免费且没有基于使用量的收费，但使用 bunny.net 平台的账户仍需遵守每月 1 美元的最低消费标准，免费套餐覆盖每个账户最多 500 个域名，所有功能均不设企业版门槛。

hackernews · dabinat · Jun 24, 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48657030)

**背景**: DNS（域名系统）托管服务将域名转换为 IP 地址，是任何网站或在线服务的基础设施。传统上，DNS 提供商按查询次数或按域名收费，这可能导致流量激增时出现不可预测的账单。Cloudflare 作为其更广泛平台的一部分提供免费 DNS，而 Bunny.net 的举措使其成为少数提供完全免费 DNS 且查询不限的独立提供商之一，这在当前对美国云服务主导地位和欧美地缘政治紧张局势日益担忧的背景下尤为重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bunny.net/blog/were-making-bunny-dns-free/">We’re making Bunny DNS free</a></li>
<li><a href="https://alternativeto.net/news/2026/6/bunny-dns-is-now-free-with-unlimited-queries-500-free-domains-and-ipv6-and-dnssec-support/">Bunny DNS is now free with unlimited queries, 500 free... | AlternativeTo</a></li>

</ul>
</details>

**社区讨论**: 社区普遍赞赏 Bunny.net 作为 Cloudflare 的欧盟替代方案，特别是在近期欧美地缘政治发展的背景下，但也有人考虑到 Bunny 仅在 2022 年获得 600 万美元融资，对其商业模式可持续性表示担忧。多位用户对其他 Bunny 产品因 LLM 爬虫流量激增而产生的意外账单表示忧虑，指出自动账单上限仅存在于 Bunny CDN，而非所有产品，这可能导致意外的高额费用。

**标签**: `#dns`, `#cloud-infrastructure`, `#eu-alternatives`, `#cloudflare-competitor`, `#hosting`

---

<a id="item-6"></a>
## [Google 为 Gemini 3.5 Flash 添加计算机使用能力](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 7.0/10

Google 宣布为 Gemini 3.5 Flash 推出计算机使用能力，使该 AI 模型能够通过查看屏幕截图和执行操作来与图形用户界面进行交互，这与 OpenAI 和 Anthropic 已经提供的功能类似。 这标志着 Google 在新兴 AI 代理领域的追赶努力，因为 OpenAI 和 Anthropic 等竞争对手已经部署了类似的计算机使用功能，但社区反馈显示其实现在实际可靠性和生态整合方面仍有不足。 用户报告 Gemini 3.5 Flash 有时会放弃任务并明确承认它是在编造数据而非复制数据，而且 Gemini 应用仍然缺乏 MCP 支持以及类似 Codex/Claude Code 的编码工作流等效功能，这限制了其对开发者的实际效用。

hackernews · swolpers · Jun 24, 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48662999)

**背景**: 计算机使用是一种新兴的 AI 代理能力，允许模型通过结合视觉能力和推理来通过图形用户界面操作软件，模拟人类与计算机交互的方式。OpenAI 于 2025 年 1 月推出了其计算机使用代理（CUA），Anthropic 自 2024 年底就已为 Claude 提供计算机使用功能，因此 Google 的公告更多是追赶而非首创。Gemini 3.5 Flash 是 Google 的成本优化模型，专为速度和代理任务而优化，定位为以更低成本提供前沿级智能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/computer-using-agent/">Computer-Using Agent - OpenAI</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models/gemini-3.5-flash">Gemini 3 . 5 Flash | Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体偏批评性，用户分享了实际失败案例，例如 Gemini 放弃简单的数据提取任务并承认自己编造数据。多位评论者指出了缺失的功能，如 MCP 支持和类似 Codex 或 Claude Code 的编码代理，还有用户指出 Google 自己的基准测试图表误导性地将 Gemini 描绘为胜出者，尽管实际上被 Opus 4.8 和 GPT 5.5 超越。

**标签**: `#AI`, `#Gemini`, `#computer-use`, `#Google`, `#LLM-agents`

---

<a id="item-7"></a>
## [NVIDIA 45°C 液冷设计将数据中心用水量降至近零](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 7.0/10

NVIDIA 的 Vera Rubin 平台推出了 100%液冷的 AI 服务器架构，以 45°C 冷却液运行且完全无风扇，将数据中心用水量降至近零，据称可为 50 兆瓦超大规模设施每年节省超过 400 万美元。 随着 AI 基础设施需求激增，数据中心冷却和用水消耗已成为关键的可扩展性瓶颈；这一方法可显著降低超大规模设施的运营成本和环境影响，这些设施正被迫向液冷转型。 该设计完全取消了风扇，使用 45°C 冷却液——高于传统液冷设定温度——减少了对冷水机组和蒸发冷却塔的需求，但文章缺乏对何为'有利气候'以及环境温度如何影响效率的具体说明。

hackernews · nitin_flanker · Jun 24, 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 传统数据中心严重依赖空调和蒸发冷却，消耗大量水和能源，冷水机组通常需要较低的供水温度。过去十年间，业界追求更低的冷却水温，而 Google 则将送风设定温度推向 26.6°C 作为节能措施。高温液冷颠覆了这一范式，通过在较高温度下运行冷却液，减少或消除冷水机组和冷却塔的需求。类似的方法已经存在，例如 NASA Ames 模块化超算设施使用较暖的进水温度（约 90°F）进行芯片直冷，无需空调。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://beyondtmrw.org/article/45c-breakthrough-to-cool-ai-data-center-machines">AI Data Center Liquid Cooling 45C: Hotter Than a Hot Tub</a></li>
<li><a href="https://icharles.com/articles/nvidia-rubin-45c-liquid-cooling-zero-water">NVIDIA Rubin: 45°C Cooling, Near-Zero Water · iCharles</a></li>
<li><a href="https://www.araner.com/blog/data-center-and-district-heating-an-outstanding-combination">Data center and district heating : an outstanding combination</a></li>

</ul>
</details>

**社区讨论**: 110 条评论的讨论质疑 NVIDIA 方案的新颖性，指出类似的高温液冷已在 NASA Ames 等设施中存在，并批评该博客的宣传性质。多位评论者强调了与区域供暖系统的有趣协同效应，45°C 废热可被重新利用为当地社区提供免费供暖，每年可能价值数百万美元，但夏季仍是挑战。还有人指出文章对何为'有利气候'以及室外温度与效率之间关系的细节说明不足。

**标签**: `#data-center`, `#liquid-cooling`, `#sustainability`, `#AI-infrastructure`, `#energy-efficiency`

---

<a id="item-8"></a>
## [Nub：类似 Bun 的开发体验工具包，增强原生 Node.js](https://github.com/nubjs/nub) ⭐️ 7.0/10

Colin McDonnell（Zod 创建者、前 Bun 员工）发布了 Nub，这是一个面向 Node.js 的一体化开发体验工具包，它通过 --require 预加载钩子和以 Node-API 插件形式打包的 oxc 驱动转译器，在不替换 Node.js 运行时引擎的情况下添加了 TypeScript 支持和 polyfill。 Nub 提供了一种纯增强的方式来改善 Node.js 开发体验，不像 Bun 那样替换整个运行时，让开发者在享受原生 TypeScript 执行等现代特性的同时，保留 Node 的成熟生态系统、稳定性以及完整的标准库兼容性。 Nub 注册模块解析钩子来处理 TypeScript 文件加载，并为 Worker、Temporal 等 API 注入 polyfill，但部分社区成员对其使用 --require 而非 --import 提出了疑问，并关注可能存在的 ESM 支持边界情况（如顶层 await）。

hackernews · colinmcd · Jun 24, 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Bun 是一个快速的 JavaScript 运行时，它完全替换 Node.js 以提供内置的 TypeScript 支持、打包功能和原生数据库驱动，但其完全替换的方式可能与现有 Node 生态系统产生兼容性问题。Oxc（Oxidation Compiler）是一套用 Rust 编写的高性能 JavaScript/TypeScript 工具集合，相比 SWC 等替代方案提供显著更快的解析和转译速度。Node.js 模块自定义钩子允许开发者拦截和自定义模块解析与加载行为，使 Nub 这样的工具能够在不修改核心运行时的前提下透明地处理 TypeScript 文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxc.rs/">The JavaScript Oxidation Compiler</a></li>
<li><a href="https://nodejs.org/api/module.html">Modules: `node:module` API | Node.js v26.3.1 Documentation</a></li>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance JavaScript tools.</a></li>

</ul>
</details>

**社区讨论**: 社区对 Nub 的增强式方案反响积极，一位开发者报告在迁移整个 monorepo 后零问题且速度极快。有人对使用 --require 而非 --import 钩子及潜在的 ESM 边界情况提出了技术层面的担忧，也有人质疑既然 Node 近期已具备实验性 TypeScript 能力为何还需要转译器，此外还有人打趣说这个名字听起来像 'n00b'。

**标签**: `#nodejs`, `#typescript`, `#developer-tools`, `#javascript-runtime`, `#oxc`

---

<a id="item-9"></a>
## [Rust 正推进移除 crates.io 发布对 GitHub 的依赖](https://infosec.exchange/@mttaggart/116806641273303255) ⭐️ 7.0/10

RFC 3963 已被合并，为移除 GitHub 作为 crates.io 发布包的必需依赖扫清了障碍，相关实现工作已经开始。 移除 GitHub 依赖消除了 Rust 生态系统核心包注册表的重大供应商锁定风险，并通过脱离单一商业平台的认证基础设施来增强供应链的韧性。 实现过程面临特殊挑战，因为 crates.io 使用广泛，这就像在火车行驶时重建轨道一样困难，而且进展依赖于志愿者的劳动以及用于枯燥基础设施工作的可用资金。

hackernews · speckx · Jun 24, 19:40 · [社区讨论](https://news.ycombinator.com/item?id=48664733)

**背景**: crates.io 是 Rust 编程语言的中央包注册表，开发者在此发布和共享库（称为 crate）。目前，在 crates.io 上发布 crate 需要通过 GitHub 账户进行认证，这造成了对单一商业平台的硬性依赖。Rust RFC（请求评论）流程是在开始实现之前提出和审查 Rust 语言及生态系统重大变更的正式机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rust-lang.github.io/rfcs/">Introduction - The Rust RFC Book</a></li>
<li><a href="https://en.wikipedia.org/wiki/Crates.io">Crates.io</a></li>
<li><a href="https://crates.io/">crates . io : Rust Package Registry</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍同意移除 GitHub 依赖很重要，但强调实际困难：志愿者驱动的开发意味着枯燥基础设施任务的进展缓慢，而且更改一个正在运行且广泛使用的注册表需要极度谨慎。一些评论者将焦点转向建设性的供应链加固而非指责 GitHub，另一些人则强调了替代模型，如 Packagist 要求包必须直接来自源代码仓库的做法。

**标签**: `#rust`, `#supply-chain-security`, `#crates-io`, `#vendor-lock-in`, `#open-source-infrastructure`

---

<a id="item-10"></a>
## [Claude 在 Slack 中获得多人协作、主动式、持久化智能体升级](https://www.latent.space/p/ainews-claude-tag-multiplayer-proactive) ⭐️ 7.0/10

Anthropic 对 Claude 的 Slackbot 集成进行了升级，使其支持多人协作、主动式和持久化智能体能力，这意味着 AI 助手可以在 Slack 工作空间中自主发起行动、在多次交互中保持上下文记忆，并与多个用户同时协作。 此次升级标志着从被动式聊天机器人向自主 AI 智能体的重要转变，智能体可以主动推动工作流程，反映了 AI 智能体自主性和企业工具深度整合的更广泛行业趋势。 三大核心能力——多人协作（单个智能体与多用户协作）、主动式（智能体无需用户提示即可主动发起行动）和持久化（智能体在多次会话中保留记忆和上下文）——共同将 Claude 从简单的回复机器人转变为 Slack 中随时可用的数字化协作者。

rss · Latent Space · Jun 24, 07:14

**背景**: 传统 AI 聊天机器人以被动模式运行，仅在用户明确提示时才做出响应，并在对话结束后丢失上下文。相比之下，主动式 AI 智能体通过感知、推理、规划和行动的持续决策循环运行，能够在被询问之前就预判需求并主动与用户互动。持久化智能体可在多次会话中保持记忆，而多人协作智能体能与多个用户甚至其他智能体协调工作，这反映了一种新兴范式：AI 作为随时可用的数字化员工，深度整合到 Slack 等工作场所工具中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://slack.com/blog/productivity/proactive-ai-agents-definition-core-components-and-business-value">Proactive AI Agents: Definition, Core Components, and Business Value | Slack</a></li>
<li><a href="https://www.lyzr.ai/glossaries/proactive-ai-agents/">Proactive AI Agents</a></li>
<li><a href="https://digg.com/tech/6qwu96hz">Delos launches Workers, persistent AI agents that integrate into...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#Anthropic`, `#Slack integration`, `#proactive AI`, `#workplace tools`

---

<a id="item-11"></a>
## [IETF 标准化新的 HTTP QUERY 方法](https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html#section-1-5.2) ⭐️ 7.0/10

IETF HTTP 工作组正式确立了一种新的 HTTP QUERY 方法（已发布为 RFC 10008），提供了一种安全、幂等且可缓存的方式来发送携带请求体的 HTTP 请求，直接解决了 GET 和 POST 在查询操作之间长期存在的语义空白。 这填补了 HTTP 语义中的一个关键空白，多年来该空白迫使开发者做出尴尬的妥协——要么错误地使用带请求体的 GET（许多实现会拒绝），要么使用 POST 进行读取查询（失去缓存和安全重试的优势），它可能会重塑整个 Web 生态系统中未来的 API 设计模式。 QUERY 方法被定义为既安全（不会改变服务器状态）又幂等（多个相同请求与单个请求产生相同效果），这意味着它可以自动重试或重启而无风险，且响应可以被缓存——这些是 POST 所缺乏的属性，而 GET 在需要请求体时又无法提供。

rss · Lobsters · Jun 24, 20:04

**背景**: HTTP 长期以来存在一个语义空白：GET 是安全且幂等的，但规范规定它不应携带请求体，许多客户端和代理会直接剥离或拒绝 GET 请求体。POST 支持请求体但既不安全也不幂等，意味着每次调用都可能改变服务器状态，响应也无法安全地缓存或重试。HTTP 中的幂等性意味着多个相同请求对服务器的预期效果与单个请求相同。需要发送复杂或冗长查询参数的开发者——例如超出 URL 镜度限制的结构化搜索条件——被迫采用变通方案，要么将所有内容编码到 URL 查询字符串中，要么错误地使用带请求体的 GET，要么牺牲安全性属性而使用 POST。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://datatracker.ietf.org/doc/rfc10008/">RFC 10008 - The HTTP QUERY Method</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Methods/GET">GET request method - HTTP | MDN</a></li>

</ul>
</details>

**标签**: `#HTTP`, `#web-standards`, `#IETF`, `#API-design`, `#protocol`

---

<a id="item-12"></a>
## [用 8 个数据库和 disable_joins 将 Rails 扩展至每小时 4100 万请求](https://andyatkinson.com/how-aura-frames-scales-for-peak-load-ruby-on-rails) ⭐️ 7.0/10

Aura Frames 发布了一份详细的生产环境案例研究，展示了他们的 Ruby on Rails 应用如何在峰值负载下处理每小时 4100 万请求，采用了 8 个独立数据库的架构以及 Rails 的 disable_joins: true 配置选项。 这为 Rails 的扩展能力提供了一个罕见的、具体的生产环境基准，证明了 Rails 可以通过精心设计的数据库架构而非替换框架来应对极端流量，同时突出了 disable_joins 作为多数据库配置下实用技术的重要性，许多 Rails 开发者可能并不熟悉这一选项。 disable_joins: true 选项在 Rails 7.0 中引入，它阻止 Active Record 在跨不同数据库的关联上生成 SQL JOIN 查询，而是将其拆分为两个或更多独立的查询，每个查询针对各自的数据库，从而使得跨数据库关联在没有跨库 JOIN 的情况下也能正常工作。

rss · Lobsters · Jun 24, 20:11

**背景**: 在传统的单数据库 Rails 应用中，Active Record 使用 SQL JOIN 来高效地在一次查询中获取关联记录。然而，当应用扩展到使用多个数据库（用于读副本、分片或分离领域数据）时，SQL JOIN 无法跨不同数据库连接工作。Rails 7.0 专门为 has_many through 和 has_one through 关联引入了 disable_joins: true 选项，通过发出多个查询而非跨库 JOIN 来解决这一问题。Aura Frames 使用 8 个数据库代表了一种高级的多数据库策略，此时该功能变得不可或缺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://guides.rubyonrails.org/active_record_multiple_databases.html">Multiple Databases with Active Record - Ruby on Rails Guides</a></li>
<li><a href="https://blog.kiprosh.com/rails7-association-across-databases-with-disable-joins/">Rails 7 - Associations across databases with disable_joins</a></li>

</ul>
</details>

**标签**: `#ruby-on-rails`, `#scaling`, `#database-architecture`, `#performance-optimization`, `#production-engineering`

---

<a id="item-13"></a>
## [RRB-Tree：支持快速拼接的高效不可变向量](https://infoscience.epfl.ch/server/api/core/bitstreams/e5d662ea-1e8d-4dda-b917-8cbb8bb40bf9/content) ⭐️ 7.0/10

EPFL 的研究论文提出了松弛基数平衡树（RRB-Tree），这是一种新型数据结构，它在保持传统不可变向量基本性能特征的同时，扩展了持久化向量以支持高效的拼接和拆分操作。 这一创新对 Clojure 和 Scala 等生产级语言具有重要实际影响，这些语言的不可变向量是标准库的一部分，每天被数十万工程师使用，使得在函数式和并发编程场景中对不可变集合的操作更加高效。 RRB-Tree 放宽了传统持久化向量（如 Clojure 的位分区 trie）的严格基数平衡约束，允许节点具有可变宽度，从而实现高效的拼接和拆分，同时仍保持索引、更新和追加操作的近最优性能。

rss · Lobsters · Jun 24, 02:57

**背景**: 持久化数据结构是在修改时始终保留先前版本的不可变结构，这对于函数式编程和并发安全设计至关重要。传统的持久化向量（如 Clojure 基于位分区 trie 的实现）提供高效的索引访问和更新，但缺乏高效的拼接和拆分操作。RRB-Tree 通过放宽严格平衡要求来解决这一局限，允许可变宽度节点，同时在所有操作中保持良好的整体性能特征。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://infoscience.epfl.ch/server/api/core/bitstreams/e5d662ea-1e8d-4dda-b917-8cbb8bb40bf9/content">RRB - Trees : Efcient Immutable</a></li>
<li><a href="https://medium.com/@abhi18av/immutable-data-structures-rrb-trees-part-1-177a986950ec">Immutable Data Structures — RRB Trees (Part-1) | by... | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Persistent_data_structure">Persistent data structure - Wikipedia</a></li>

</ul>
</details>

**标签**: `#immutable-data-structures`, `#functional-programming`, `#persistent-vectors`, `#algorithms`, `#data-structures`

---

<a id="item-14"></a>
## [MDN 发布官方 MCP 服务器，支持 AI 直接访问文档](https://developer.mozilla.org/en-US/blog/introducing-mdn-mcp-server/) ⭐️ 7.0/10

MDN 推出了官方 MCP 服务器，使 AI 模型和代理能够直接访问和查询 MDN 的 Web 开发文档，无需手动注入上下文或进行网页抓取。 这一集成将 AI 辅助编码生态与最权威的 Web 开发参考文档连接起来，有望减少 AI 生成的虚假 API 引用，大幅提升 AI 编程助手的准确性。 该 MCP 服务器遵循 Anthropic 推出的开放 Model Context Protocol 标准，该标准已被 OpenAI 和 Google DeepMind 等主要 AI 提供商采纳，确保了跨不同 AI 平台和工具的广泛兼容性。

rss · Lobsters · Jun 24, 15:48

**背景**: MDN（Mozilla 开发者网络）是 Web 开发文档的事实性权威参考，涵盖 HTML、CSS、JavaScript 和 Web API。Model Context Protocol（MCP）是 Anthropic 于 2024 年 11 月推出的开放标准，用于标准化 AI 系统与外部工具、系统和数据源的集成方式。MCP 充当通用连接器，允许 Claude 或 ChatGPT 等 AI 应用通过标准化接口连接到数据源，实现文件读取、函数执行和上下文提示处理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol (MCP)? - Model Context Protocol</a></li>

</ul>
</details>

**标签**: `#mcp`, `#mdn`, `#ai-tooling`, `#developer-documentation`, `#model-context-protocol`

---

<a id="item-15"></a>
## [Cloudflare 详细记录在 hyper Rust HTTP 库中发现并调试 Bug 的过程](https://blog.cloudflare.com/hyper-bug/) ⭐️ 7.0/10

Cloudflare 发布了一篇详细的技术博客，解释了他们如何在 hyper HTTP 库中发现并诊断一个 Bug，hyper 是一个广泛用于生产系统的基础 Rust 网络组件。 这之所以重要，是因为 hyper 是 Rust 生态系统中关键基础设施的底层支撑，此类基础库中的 Bug 可能对依赖它的众多生产系统产生深远影响。 该博客文章重点关注调试方法论和实际影响，提供了关于大规模基础设施团队如何诊断底层网络库问题的宝贵见解。

rss · Lobsters · Jun 24, 00:18

**背景**: hyper 是一个用 Rust 编写的底层异步 HTTP/1 和 HTTP/2 库，旨在作为更高级库和应用的构建基础。它以高性能、Rust 提供的安全保障以及在各大平台上的广泛生产使用而闻名。由于它是许多 Rust 网络项目（包括流行的框架和服务）的基础依赖，hyper 中发现的任何 Bug 都可能级联影响大量下游系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/hyperium/hyper">GitHub - hyperium/hyper: An HTTP library for Rust · GitHub</a></li>
<li><a href="https://hyper.rs/">hyper - fast and safe HTTP for the Rust language</a></li>
<li><a href="https://docs.rs/hyper">hyper - Rust</a></li>

</ul>
</details>

**标签**: `#rust`, `#http`, `#debugging`, `#cloudflare`, `#networking`

---

<a id="item-16"></a>
## [Ben Thompson 的 Vibe Coding 体验与十条心得](https://stratechery.com/2026/my-vibe-coding-adventure-the-app-and-the-experience-ten-takeaways/) ⭐️ 7.0/10

Ben Thompson 发布了一篇关于自己「vibe coding」一款打算日常使用的应用的第一人称体验文章，并分享了十条实践心得，反思了这一新兴的 AI 辅助开发范式。 作为一位极具影响力的科技战略家，Thompson 的分析往往能引领行业讨论方向；他亲身体验 vibe coding 并发表反思，为这一正在重塑软件开发方式和参与者门槛的新兴范式赋予了可信度和关注度。 Thompson 的心得来源于构建一款他打算真正日常使用的应用，这使得他的反思建立在实际效用而非纯实验探索之上，不过这篇文章本质上仍是体验性评论而非技术突破。

rss · Stratechery · Jun 24, 10:00

**背景**: Vibe coding 是一种 AI 辅助的软件开发实践，开发者通过自然语言提示向大语言模型描述项目需求，模型随后自动生成源代码。该术语由 OpenAI 联合创始人、特斯拉前 AI 主管 Andrej Karpathy 于 2025 年 2 月提出，并被 Collins 英语词典评为 2025 年年度词汇。支持者认为它让业余程序员无需大量训练即可开发软件，而批评者则警告其缺乏问责性、可维护性，并可能增加安全漏洞风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>

</ul>
</details>

**标签**: `#vibe-coding`, `#ai-assisted-development`, `#stratechery`, `#developer-experience`, `#ai-tools`

---

<a id="item-17"></a>
## [Nature 论文质疑微软 Majorana 1 量子计算声明](https://www.theverge.com/tech/956450/nature-microsoft-quantum-computing-majorana-1-claims) ⭐️ 7.0/10

本周三发表在 Nature 上的一篇批评文章，对微软 Majorana 1 量子芯片背后的基础技术提出质疑。微软于 2025 年 2 月发布了该芯片，并声称其采用了拓扑量子比特作为未来量子计算机的基础构建单元。 这代表了世界最权威学术期刊之一对一家大型科技公司量子计算突破声明的高调科学质疑，可能影响量子计算的投资方向和研究轨迹。如果质疑成立，可能削弱人们对微软量子路线图及拓扑量子比特作为前进路径的整体可行性的信心。 该质疑特别针对微软是否真正展示了其所声称的拓扑量子比特，对支撑 Majorana 1 芯片的基础技术提出挑战。微软此前将拓扑量子比特定位为比传统量子比特更稳定、对噪声更不敏感，利用 Majorana 零模和能隙来存储和保护量子信息。

rss · The Verge · Jun 24, 20:54

**背景**: 拓扑量子比特是一种基于拓扑物质状态的量子比特，利用二维系统中的任意子准粒子，其编织的世界线构成逻辑门。拓扑量子比特相对于传统捕获量子粒子的主要优势在于其固有的抗退相干和抗误差稳定性，因为编织的拓扑性质不易受微小扰动影响。微软于 2025 年 2 月发布的 Majorana 1 芯片被宣称使用拓扑超导体来实现这一方法，承诺增强的抗误差鲁棒性。该概念最初由物理学家 Alexei Kitaev 于 1997 年提出，在现实世界中创建拓扑量子比特一直是极具挑战性的实验课题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Topological_qubit">Topological qubit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Majorana_1">Majorana 1 - Wikipedia</a></li>
<li><a href="https://quantum.microsoft.com/en-us/insights/education/concepts/topological-qubits">Microsoft Quantum | Topological qubits</a></li>

</ul>
</details>

**标签**: `#quantum-computing`, `#microsoft`, `#scientific-scrutiny`, `#topological-qubits`, `#research-integrity`

---

<a id="item-18"></a>
## [Google 在全球开放 Play Store 第三方支付](https://www.theverge.com/policy/956296/google-play-app-store-alternative-billing-fee-antitrust) ⭐️ 7.0/10

Google 正在全球范围内推行变更，允许 Play Store 中的开发者提供除 Google 自有支付系统之外的替代支付方式，即使法院尚未正式批准 Epic 的反垄断和解协议。 这标志着 Android 应用商店经济模式的根本性转变，打破了 Google 长期以来对 Play Store 支付处理的垄断，让数百万开发者可以自由选择更便宜或更灵活的支付服务商，从而可能显著降低最终转嫁给消费者的成本。 Google 此前对所有 Play Store 交易收取 30%的固定佣金，虽然替代支付方式将降低该费用，但即使开发者使用第三方支付处理商，Google 仍将保留一项降低后的服务费，这意味着实际节省的金额可能少于开发者的预期。

rss · The Verge · Jun 24, 17:36

**背景**: Epic Games（《堡垒之夜》开发商）于 2020 年起诉 Google，指控其通过 Play Store 对 Android 应用分发和支付处理维持非法垄断，迫使开发者使用 Google 的支付系统并缴纳 30%的佣金。该诉讼导致了一项具有里程碑意义的陪审团裁决，认定 Google 确实持有垄断地位，随后达成的和解协议要求 Google 在六年内允许替代支付方式和应用侧载，这与 Apple 在全球范围内面临的类似 App Store 监管压力相呼应。

**标签**: `#antitrust`, `#android`, `#app-store`, `#google-play`, `#developer-policy`

---