---
layout: default
title: "Horizon Summary: 2026-06-28 (ZH)"
date: 2026-06-28
lang: zh
---

> From 48 items, 13 important content pieces were selected

---

1. [DeepSeek 发布 DSpark 推测解码框架](#item-1) ⭐️ 8.0/10
2. [OpenAI 发布 GPT-5.6 Sol/Terra/Luna，仅限可信合作伙伴使用](#item-2) ⭐️ 8.0/10
3. [IP Crawl 绘制公网上未加密摄像头实时画面地图](#item-3) ⭐️ 7.0/10
4. [金融科技工程手册引发货币表示方式辩论](#item-4) ⭐️ 7.0/10
5. [可疑的数据断点揭示隐藏的系统激励](#item-5) ⭐️ 7.0/10
6. [本地编程代理作为 Claude Code 和 Codex 的替代方案](#item-6) ⭐️ 7.0/10
7. [深入 Reddit 反垃圾信息检测与过滤系统内部](#item-7) ⭐️ 7.0/10
8. [严重降低 CPU 性能的数据访问模式](#item-8) ⭐️ 7.0/10
9. [值得其他语言借鉴的 OxCaml 特性](#item-9) ⭐️ 7.0/10
10. [Stephen Diehl 推出 Prism：带类型效应的非纯函数式语言](#item-10) ⭐️ 7.0/10
11. [AI 学会了射频芯片设计的“黑魔法”](#item-11) ⭐️ 7.0/10
12. [UEFI CA 过期导致多系统安全启动失效](#item-12) ⭐️ 7.0/10
13. [Transformer 与混合模型架构的 Token 级别对比](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [DeepSeek 发布 DSpark 推测解码框架](https://github.com/deepseek-ai/DeepSpec/blob/main/DSpark_paper.pdf) ⭐️ 8.0/10

DeepSeek 发布了 DSpark，一个开源的推测解码框架，在 MTP-1 基线之上将 DeepSeek-V4 的单用户生成速度提升了 57–85%，Flash 和 Pro 模型变体已在 HuggingFace 上线，同时开源了全栈工具 DeepSpec。 这是 LLM 推理优化领域的一项重大实用进展，直接降低了最广泛使用的开源模型系列之一的延迟和成本，DeepSeek 同时发布论文和生产可用模型的做法树立了强有力的开放研究先例，与其他主要实验室日益封闭的做法形成鲜明对比。 DSpark 结合了并行生成与自适应负载感知验证，最高可实现 85%的速度提升，可用模型包括 DeepSeek-V4-Pro（1.6T 总参数，49B 激活）和 DeepSeek-V4-Flash（284B 总参数，13B 激活），两者均为支持百万 token 上下文长度的混合专家（MoE）架构。

hackernews · aurenvale · Jun 27, 09:18 · [社区讨论](https://news.ycombinator.com/item?id=48696585)

**背景**: 推测解码是自回归 LLM 的一种推理时优化技术，每个解码步骤生成多个 token 而非一个，类似于 CPU 设计中的推测执行。较小的草稿模型提出候选 token，较大的目标模型通过修改的拒绝采样方案在一次前向传播中验证它们，在保持原始输出分布的同时将延迟降低约两到三倍。此前的方法包括 Medusa（添加轻量解码头）和 EAGLE（使用外推草稿头），而 MTP（多 token 预测）是 DSpark 所改进的基线方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/06/27/deepseek-releases-dspark-a-speculative-decoding-framework-that-accelerates-deepseek-v4-per-user-generation-60-85-over-mtp-1/">DeepSeek Releases DSpark, a Speculative Decoding Framework That Accelerates DeepSeek-V4 Per-User Generation 60–85% Over MTP-1 - MarkTechPost</a></li>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro-DSpark">deepseek-ai/DeepSeek-V4-Pro-DSpark · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体极为正面，用户称赞 DeepSeek 的开放性和创新精神，认为美国实验室越来越封闭且只追求跑分。实际使用报告突出了成本效率——一位用户用 DeepSeek-V4 Pro 仅花费 40 美元就处理了 15 亿 token——同时社区对将 DSpark 集成到 DwarfStar 等本地推理工具中表现出兴趣，也有人提出了 DSpark 与 2022 年早期推测解码工作的技术对比问题。

**标签**: `#speculative-decoding`, `#llm-inference`, `#deepseek`, `#ai-optimization`, `#open-research`

---

<a id="item-2"></a>
## [OpenAI 发布 GPT-5.6 Sol/Terra/Luna，仅限可信合作伙伴使用](https://www.latent.space/p/ainews-openai-gpt-56-sol-terra-luna) ⭐️ 8.0/10

OpenAI 于 2026 年 6 月 26 日预发布了 GPT-5.6，包含三个变体——Sol（旗舰级）、Terra（均衡型）和 Luna（高吞吐量）——但应美国政府官员的要求，仅将初始访问权限限制在 20 个经政府批准的可信合作伙伴。此次发布与 Anthropic 在同一天向部分公司推出 Claude Mythos 同步进行。 这标志着 OpenAI 发布策略的重大转变，引入了将模型名称与版本号解耦的持久能力层级体系，同时也是前沿 AI 模型首次因美国政府直接要求而限制发布，可能为未来的部署设定先例。 此次限制发布是由特朗普政府下的国家网络总监办公室和科技政策办公室要求的，OpenAI 计划在未来几周内进行更广泛的公开发布。分层命名约定与 Anthropic 的 Opus/Sonnet/Haiku 体系类似，其中 Sol 最强，Terra 平衡性能与成本，Luna 面向高吞吐量使用场景。

rss · Latent Space · Jun 27, 05:23

**背景**: GPT-5.6 引入了新的命名约定，其中数字代表代际，名称（Sol、Terra、Luna）代表跨版本持久的能力层级，这意味着未来的发布可能以 GPT-5.7 Sol/Terra/Luna 的形式推出，而非全新的模型名称。这与 Anthropic 长期采用的三档发布策略（Opus、Sonnet、Haiku）相呼应。限制可信合作伙伴使用源于美国政府日益增长的对前沿 AI 模型安全影响的担忧，并与 OpenAI 近期推出的 1.5 亿美元合作伙伴网络计划同步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.digitalapplied.com/blog/gpt-5-6-sol-terra-luna-preview-guide-2026">GPT - 5 . 6 Sol , Terra & Luna : OpenAI's New Model Family</a></li>
<li><a href="https://interestingengineering.com/culture/openai-gpt-5-6-sol-terra-luna-limited-preview">OpenAI launches GPT - 5 . 6 but restricts rollout after US request</a></li>
<li><a href="https://icharles.com/articles/openai-gpt-56-trusted-partners-release">OpenAI Limits GPT-5.6 to Trusted Partners - icharles.com</a></li>

</ul>
</details>

**标签**: `#openai`, `#gpt`, `#ai-models`, `#tiered-release`, `#anthropic`

---

<a id="item-3"></a>
## [IP Crawl 绘制公网上未加密摄像头实时画面地图](https://ipcrawl.com/) ⭐️ 7.0/10

IP Crawl 是一个新上线的网站，它系统地发现、映射并展示公网上可访问的未加密摄像头实时视频流，允许用户浏览、筛选并实时观看这些摄像头画面。 该项目直观地展示了 IoT 安全长期且普遍的失败，暴露了无数私人空间如何在不知不觉中被广播给互联网上的任何人，引发了关于隐私、监控以及设备制造商和消费者责任的严肃伦理问题。 该网站允许用户按多种条件浏览和筛选实时摄像头画面，而其揭示的根本问题并不新鲜——类似的漏洞至少从 2012 年就已存在，廉价 IP 摄像头通常缺乏适当的安全默认设置，且可通过搜索引擎查询轻易发现。

hackernews · arm32 · Jun 27, 19:09 · [社区讨论](https://news.ycombinator.com/item?id=48700834)

**背景**: 许多廉价的 IP 摄像头，尤其是低价消费级型号，在销售时几乎没有安全配置，用户只是按照包装上的说明操作，不了解防火墙概念或公网暴露意味着什么。历史上，在 Google 中输入特定搜索字符串就能找到这些未加密设备，因为搜索引擎爬虫会索引它们的 Web 界面。这是一个长期存在的 IoT 安全问题：设备出厂时带有默认凭据、没有加密且端口暴露，形成了任何人都可以访问的庞大脆弱网络摄像头生态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ipcrawl.com/">IP Crawl</a></li>

</ul>
</details>

**社区讨论**: 社区讨论揭示了强烈的伦理担忧，多位评论者对未经同意观看私人空间表达了深深的不安，并描述了观察陌生人私人时刻时那种令人不安的恐惧感。另一些人指出大多数消费者只是按照产品说明操作，缺乏网络安全的技术知识，并将该网站比作用望远镜透过未拉上的窗帘窥视邻居公寓，而非仅仅是路过。有人注意到这个问题至少从 2012 年以来就一直没有改变，还有评论者幽默地建议注入伪造的循环录像作为一种创意对策。

**标签**: `#privacy`, `#iot-security`, `#surveillance`, `#ethical-hacking`, `#network-security`

---

<a id="item-4"></a>
## [金融科技工程手册引发货币表示方式辩论](https://w.pitula.me/fintech-engineering-handbook/) ⭐️ 7.0/10

一份新发布的金融科技工程手册旨在记录以货币为核心的系统中的重要软件工程模式，却引发了大量社区辩论，资深从业者对其部分建议提出质疑，并分享了关于货币值表示和交换格式陷阱的宝贵生产经验。 这场实质性的辩论将金融系统设计中罕见记录的基础问题——如如何表示货币值和处理货币交换边缘情况——带入公共讨论，使这些关键经验对任何构建或维护金融软件的人都变得可获取。 该手册本身被批评内容浅薄且包含一些可疑建议，但社区讨论揭示了关键注意事项：由于 IEEE 754 浮点精度问题，将货币值存储为整数以外的任何类型都有风险，而用于交换/API 格式的次要单位精度策略在合作伙伴对同一货币使用不同隐含小数位数时可能造成灾难性失败。

hackernews · signa11 · Jun 27, 10:28 · [社区讨论](https://news.ycombinator.com/item?id=48696982)

**背景**: 在软件中表示货币值是金融科技工程的基础挑战：使用浮点数（IEEE 754）会引入精度误差，可能导致财务差异；而使用次要单位（如用美分代替美元）的整数方法虽然避免了加减法舍入问题，但在不同系统对同一货币假设不同小数精度时会产生交换问题。外汇（FX）汇率增加了更多复杂性，因为汇率解析并非简单的即时值，还涉及买方即时汇率考量，影响交易的正确性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://w.pitula.me/fintech-engineering-handbook/">Fintech Engineering Handbook</a></li>
<li><a href="https://news.ycombinator.com/item?id=48696982">Fintech Engineering Handbook | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区讨论呈现了资深从业者的多元观点：一位评论者强烈主张货币值必须始终以整数存储，警告 Rust 小数序列化为 JSON 浮点数的危险性；另一位警告不要将次要单位精度用作交换/API 格式，因为合作伙伴具有不同隐含小数位数的边缘情况；第三位反思金融科技中不同视角如何揭示了优秀编程的情境性本质；一位前金融科技 CTO 验证了手册大部分内容的正确性，同时强调许多决策最终取决于具体项目需求。

**标签**: `#fintech`, `#monetary-representation`, `#systems-design`, `#financial-engineering`, `#edge-cases`

---

<a id="item-5"></a>
## [可疑的数据断点揭示隐藏的系统激励](https://danluu.com/discontinuities/) ⭐️ 7.0/10

Dan Luu 发表了一篇分析文章，探讨了数据分布中可疑的断点——例如马拉松完赛时间在整数分钟的聚集、税收政策阈值处的骤降、考试成绩截断点处的异常凸起——如何揭示原本不可见的底层结构属性、人类行为和系统激励机制。 理解数据断点有助于分析师和政策制定者识别人为激励或系统设计造成的扭曲，从而改进政策设计、更准确地解读数据，并发现现实系统中的操纵行为或结构性缺陷。 文章指出，散点图、直方图和累积分布函数（CDF）等简单可视化工具通常足以检测这些断点，并提到队列会制造一种断点，在某些情况下应当被平滑处理。

hackernews · tosh · Jun 27, 13:32 · [社区讨论](https://news.ycombinator.com/item?id=48698151)

**背景**: 回归断点设计（RDD）是一种准实验方法，通过比较阈值两侧的观测值来估计干预的因果效应。Dan Luu 的文章反向运用了类似的观察思路：不是将断点作为研究工具，而是将断点本身视为隐藏激励、结构约束或人类行为反应（如追求整数目标或规避税收悬崖）的证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://danluu.com/discontinuities/">Suspicious discontinuities - danluu.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/Regression_discontinuity_design">Regression discontinuity design</a></li>
<li><a href="https://news.ycombinator.com/item?id=28452926">Suspicious Discontinuities | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论者用亲身经历和额外案例丰富了文章内容：马拉松跑者解释了配速组和整数目标导致完赛时间聚集；英国和印度税制被指出存在严重的悬崖效应，边际税率在某些收入区间超过 60%甚至达到 100%；还有评论者强调波兰语考试成绩图在 30 分处呈现出混乱的异常堆积，破坏了原本干净的钟形曲线。

**标签**: `#data-analysis`, `#statistics`, `#policy-design`, `#system-incentives`, `#dan-luu`

---

<a id="item-6"></a>
## [本地编程代理作为 Claude Code 和 Codex 的替代方案](https://magazine.sebastianraschka.com/p/using-local-coding-agents) ⭐️ 7.0/10

Sebastian Raschka 发表了一篇实用性探索文章，探讨在本地编程框架中使用开放权重模型，作为 Claude Code 和 Codex 等订阅制 AI 编程助手的可行替代方案。 这回应了开发者日益增长的对成本、隐私和供应商独立性的关切，为那些希望避免持续订阅费用并完全掌控代码库与数据的人提供了可行的路径。 本地编程框架的选择与模型本身同样关键；主要的开源选项包括 OpenCode（最接近 Claude Code 体验、供应商无关）、Pi Coding Agent（最具可扩展性、最小核心理念）以及 OpenHands（功能完整的自主代理框架）。

rss · Ahead of AI (Sebastian Raschka) · Jun 27, 11:21

**背景**: 开放权重模型是指其学习参数公开可供下载的 AI 系统，使个人研究人员和小公司能够在本地运行、研究和修改前沿级语言模型。Claude Code 是 Anthropic 的代理式编程系统，可在整个项目中运作以理解代码库、执行多文件更改并自主完成开发任务。编程框架是将 LLM 连接到开发工具、文件系统和终端访问的编排框架，有效地将语言模型转变为活跃的编程代理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grigio.org/local-harness-benchmark-pi-coding-agent-vs-opencode/">Local Harness Benchmark: Pi Coding Agent vs. OpenCode</a></li>
<li><a href="https://gist.github.com/asermax/4fb2be4f6f1fc0d6be1e3966b6e2bb91">Coding Agent Harnesses — Comparative Overview (2026) · GitHub</a></li>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system \ Anthropic</a></li>

</ul>
</details>

**标签**: `#coding-agents`, `#local-ai`, `#open-weight-models`, `#developer-tools`, `#ai-alternatives`

---

<a id="item-7"></a>
## [深入 Reddit 反垃圾信息检测与过滤系统内部](https://lyra.horse/blog/2026/06/reddit-spam-internals/) ⭐️ 7.0/10

一篇详细的博客文章发布，罕见地公开展示了 Reddit 内部反垃圾信息检测与过滤机制的运作方式，揭示了全球最大平台之一的垃圾信息防御架构与策略。 大型平台几乎从不公开其反垃圾信息系统的内部运作，这使得该文章成为工程师在设计大规模类似防御系统时以及安全研究人员理解现实垃圾信息缓解策略的宝贵资源。 该文章涵盖了 Reddit 特定的检测流水线、过滤算法以及系统设计选择，用于在平台庞大的用户群中识别和处理垃圾信息内容。

rss · Lobsters · Jun 27, 15:10

**背景**: 像 Reddit 这样的大规模平台上的反垃圾信息系统必须实时处理海量的提交和评论，在保护用户的激进过滤与压制合法内容的误报风险之间取得平衡。这些系统通常结合启发式规则、机器学习分类器和基于信誉的评分，来检测垃圾信息攻势、协同操纵和滥用行为所特有的模式。

**标签**: `#anti-spam`, `#reddit`, `#platform-internals`, `#security`, `#systems-design`

---

<a id="item-8"></a>
## [严重降低 CPU 性能的数据访问模式](https://blog.weineng.me/posts/slowest_add/) ⭐️ 7.0/10

一篇技术博客文章深入探讨了特定的数据访问模式如何通过引发缓存未命中和内存效率低下而严重降低 CPU 性能，并通过看似等效操作的实际示例展示了戏剧性的性能影响。 理解数据访问模式及其对缓存行为的影响对于系统程序员和性能工程师至关重要，因为单次缓存未命中就可能消耗 100-300 个 CPU 周期，而处理器在此期间只能空闲等待来自 RAM 的数据。 该文章涵盖了缓存未命中、内存布局优化等重要概念，并展示了顺序访问与随机访问模式如何极大地影响吞吐量，证明了在逻辑上看似等效的操作会因数据在内存中的排列方式而产生截然不同的性能特征。

rss · Lobsters · Jun 27, 14:18

**背景**: 现代 CPU 严重依赖多级缓存层次结构（L1、L2、L3）来弥补处理器与主内存（RAM）之间的速度差距，后者可能慢几个数量级。缓存命中意味着请求的数据在缓存中找到，允许快速访问；而缓存未命中则迫使 CPU 从 RAM 获取数据，使执行停滞数百个周期。内存访问模式——无论是顺序访问、随机访问还是跨步访问——直接决定了缓存利用效率，使得数据布局优化成为系统编程和高性能计算中的基本关注点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CPU_cache">CPU cache - Wikipedia</a></li>
<li><a href="https://medium.com/@sohail_saifi/the-cpu-cache-miss-thats-slowing-every-web-application-c98b71515125">The CPU Cache Miss That’s Slowing Every Web Application | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Memory_access_pattern">Memory access pattern - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cpu-optimization`, `#data-access-patterns`, `#cache-performance`, `#systems-programming`, `#memory-layout`

---

<a id="item-9"></a>
## [值得其他语言借鉴的 OxCaml 特性](https://theconsensus.dev/p/2026/06/27/the-feature-in-oxcaml-more-languages-should-steal.html) ⭐️ 7.0/10

The Consensus 上的一篇文章推荐了 OxCaml（Jane Street 的 OCaml 扩展编译器）中的一个特定特性，作者认为该特性值得其他编程语言广泛借鉴。 这种跨语言特性倡导能够影响语言设计讨论，并推动那些已被验证但未被充分重视的创新在其原始生态之外获得更广泛的采纳。 OxCaml 既是 Jane Street 的生产编译器，也是面向性能的 OCaml 扩展的实验平台，这意味着它引入的特性在大规模工业使用中经过了实战检验，然后才被提议供更广泛采纳。

rss · Lobsters · Jun 27, 21:07

**背景**: OxCaml 是由 Jane Street 开发的 OCaml 编程语言的一组快速演进的扩展，Jane Street 是一家大型量化交易公司，也是 OCaml 十多年来最显著的工业用户之一。Jane Street 历史上一直维护着 OCaml 的一个分支，包含大量扩展（包括具体的语法变更），OCaml 社区内部也曾讨论将这些变更上游合并的可能性。文章中'值得借鉴'的表述暗示该特性已在 Jane Street 的生产环境中证明了其价值，并且能够很好地推广到其他语言生态系统中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxcaml.org/">OxCaml | About</a></li>
<li><a href="https://blog.janestreet.com/introducing-oxcaml/">Jane Street Blog - Introducing OxCaml</a></li>

</ul>
</details>

**社区讨论**: 该文章在 Lobste.rs 上引发了讨论，该社区以围绕编程语言设计进行技术严谨的对话而闻名，但提供的材料中未包含具体评论内容。

**标签**: `#programming-languages`, `#oxcaml`, `#ocaml`, `#language-design`, `#jane-street`

---

<a id="item-10"></a>
## [Stephen Diehl 推出 Prism：带类型效应的非纯函数式语言](https://www.stephendiehl.com/posts/prism/) ⭐️ 7.0/10

Stephen Diehl 推出了 Prism，一种新的非纯函数式编程语言，它在语言的类型系统中集成了类型效应系统，以正式追踪和管理副作用。 类型效应系统是编程语言理论中一个活跃的研究前沿，而由像 Diehl 这样受人尊敬的 PL 设计者推出的实用语言实现，可能会显著影响社区在函数式编程中处理副作用管理的方式。 Prism 被专门设计为非纯函数式语言，这意味着它允许副作用，但通过类型效应系统使这些副作用在类型层面可见且可追踪，而不是隐藏或完全禁止它们。

rss · Lobsters · Jun 27, 19:39

**背景**: 在纯函数式编程中，函数没有副作用，这使得程序更容易推理，但对于需要状态修改或 I/O 的现实任务往往不够实用。像 OCaml 和 Clojure 这样的非纯函数式语言为了实用性允许副作用，但传统上缺乏在类型系统中正式追踪它们的机制。效应系统通过为函数标注其可能执行的效应来扩展类型系统，使编译器和程序员能够在不牺牲非纯编程表达力的情况下对副作用进行推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Effect_system">Effect system - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Functional_programming">Functional programming - Wikipedia</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#effect-systems`, `#functional-programming`, `#type-systems`, `#pl-research`

---

<a id="item-11"></a>
## [AI 学会了射频芯片设计的“黑魔法”](https://spectrum.ieee.org/ai-radio-chip-design) ⭐️ 7.0/10

AI 技术现在正被应用于射频集成电路（RFIC）设计，这一领域长期以来一直抗拒自动化，始终依赖于专家的人类直觉而非标准化的科学流程。 自动化或加速射频芯片设计可能会对半导体和无线行业产生重大影响，通过降低成本、缩短设计周期，并加速依赖这些芯片的无线通信技术的创新。 虽然大多数计算芯片设计已通过 EDA 工具标准化为一门系统科学，但射频设计却顽固地停留在艺术的范畴，这使得 AI 进入该领域成为一个特别引人注目且充满挑战的突破。

rss · Lobsters · Jun 27, 18:03

**背景**: 射频（RF）芯片是无线通信设备中的关键组件，负责信号的发送和接收。电子设计自动化（EDA）工具已成功将数字芯片设计标准化为系统化流程，但射频芯片设计涉及复杂的模拟考量——如寄生效应、阻抗匹配和电磁干扰——这些因素一直抗拒自动化。这种复杂性使射频设计获得了“黑魔法”的称号，需要多年的经验和深厚的直觉，而这些难以被编码为软件规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spectrum.ieee.org/ai-radio-chip-design">AI Learns the “Dark Art” of RFIC Design - IEEE Spectrum</a></li>
<li><a href="https://en.wikipedia.org/wiki/Electronic_design_automation">Electronic design automation - Wikipedia</a></li>

</ul>
</details>

**标签**: `#ai`, `#chip-design`, `#rf-engineering`, `#eda`, `#semiconductor`

---

<a id="item-12"></a>
## [UEFI CA 过期导致多系统安全启动失效](https://blog.einval.com/2026/06/27#its_dead_jim) ⭐️ 7.0/10

Microsoft UEFI 证书授权机构 2011 证书即将过期，导致未在固件中更新至较新的 UEFI CA 2023 层级证书的系统上安全启动功能失效。 这影响了全球数十亿台个人电脑，包括依赖 Microsoft UEFI 签名链加载第三方引导程序的 Windows 和 Linux 系统，构成了重大的基础设施和安全风险，因为安全启动能防止未经授权或恶意代码在启动过程中执行。 Windows Production PCA 2011 证书将于 2026 年 10 月 19 日过期，固件中仅包含 Microsoft Corporation UEFI CA 2011 证书的系统需要立即进行固件更新以纳入 2023 年的替代证书。

rss · Lobsters · Jun 27, 22:42

**背景**: UEFI 安全启动是 UEFI 固件中的一项安全功能，确保只有经过数字签名的可信软件（如引导加载程序和操作系统内核）在启动过程中被加载，防止未经授权或恶意代码执行。Microsoft UEFI CA 2011 在十多年间一直是数百万设备启动过程的信任基石，既签名 Windows 引导加载程序，也签名 Linux 发行版广泛使用的第三方引导加载程序。Microsoft 推出了 UEFI CA 2023 层级作为替代方案，但固件必须在旧证书过期之前主动更新以包含新证书，否则安全启动将拒绝已签名的引导组件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcommunity.microsoft.com/blog/windows-itpro-blog/secure-boot-playbook-for-certificates-expiring-in-2026/4469235?after=MjUuMTJ8Mi4xfGl8MTB8MTMyOjB8aW50LDQ0OTk3MjAsNDQ3NjUyMw">Secure Boot playbook for certificates expiring in 2026</a></li>
<li><a href="https://cybersecuritynews.com/windows-secure-boot-certificate-expired/">Windows Secure Boot Certificate Expired — Billions of PCs Affected...</a></li>
<li><a href="https://www.trellix.com/blogs/platform/navigating-microsoft-uefi-cert-transition-encrypted-devices/">Navigating the Microsoft UEFI Certificate Transition for Encrypted...</a></li>

</ul>
</details>

**社区讨论**: 该博客文章链接到 lobste.rs 上的讨论，社区成员可能正在分享关于修复方案的多元观点、对旧硬件固件更新可用性的担忧，以及依赖 Microsoft 签名链建立跨平台安全启动信任的更广泛影响。

**标签**: `#UEFI`, `#secure-boot`, `#infrastructure`, `#security`, `#firmware`

---

<a id="item-13"></a>
## [Transformer 与混合模型架构的 Token 级别对比](https://arxiv.org/pdf/2606.20936) ⭐️ 7.0/10

一篇新的 arxiv 研究论文在纯 Transformer 和混合模型架构之间进行了 Token 级别的对比，在单个 Token 处理的细粒度层面分析了它们的行为差异，而非仅依赖整体基准测试指标。 Token 级别分析能够精确定位每种架构的优势和不足，为模型设计者在纯 Transformer 和混合设计之间做出选择提供可操作的洞察。鉴于当前行业正大力推进将注意力机制与其他机制结合以提升效率的混合模型，这一点尤为重要。 该研究在单个 Token 层面考察了纯 Transformer 与混合架构（结合了 SSM/Mamba 层、自注意力机制和 MLP 等组件）之间的行为差异，提供了传统宏观层面评估无法捕捉的全新分析粒度。

rss · Lobsters · Jun 27, 15:16

**背景**: Transformer 通过自注意力机制处理所有 Token，这在长序列场景下计算成本高昂。混合模型（如将 Mamba 状态空间模型层与注意力机制和 MLP 层相结合的模型）旨在降低计算成本的同时保持模型质量。近期行业模型如 DeepSeek V4 和 Qwen3-Next 采用了混合注意力机制，仅激活总参数的一小部分便实现了显著的效率提升。Token 级别分析考察模型如何处理每个单独的 Token，揭示整体基准测试可能掩盖的细粒度行为模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2406.07887">An Empirical Study of Mamba-based Language Models</a></li>
<li><a href="https://framia.converge.ai/page/en-US/news/deepseek-v4-model-architecture">DeepSeek V4 Architecture : CSA, HCA, mHC, MoE Deep Dive</a></li>
<li><a href="https://qwen3-next.com/">Qwen3-Next: Revolutionary AI Model Architecture</a></li>

</ul>
</details>

**标签**: `#transformers`, `#hybrid-models`, `#model-architecture`, `#token-analysis`, `#ai-research`

---