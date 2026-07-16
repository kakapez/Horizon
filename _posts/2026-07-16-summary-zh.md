---
layout: default
title: "Horizon Summary: 2026-07-16 (ZH)"
date: 2026-07-16
lang: zh
---

> From 55 items, 15 important content pieces were selected

---

1. [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](#item-1) ⭐️ 8.0/10
2. [研究人员绕过 Claude 的 web_fetch 防护机制窃取用户数据](#item-2) ⭐️ 8.0/10
3. [OpenAI 发布 GPT-Red 自动化 AI 安全测试系统](#item-3) ⭐️ 8.0/10
4. [Thinking Machines 发布 Inkling：最大的开源权重多模态模型，支持音频](#item-4) ⭐️ 7.0/10
5. [13 年老 Xeon 无 GPU 运行 Gemma 4 26B 达 5 token/秒](#item-5) ⭐️ 7.0/10
6. [完整 Firefox 浏览器被移植到 WebAssembly 中运行](#item-6) ⭐️ 7.0/10
7. [misa77 编解码器实现两倍于 LZ4 的解压速度](#item-7) ⭐️ 7.0/10
8. [AI Weekly 发布免费可搜索的 159 个真实 AI 部署案例库](#item-8) ⭐️ 7.0/10
9. [FreeBSD 16 从基础系统中移除全部 GPL 代码](#item-9) ⭐️ 7.0/10
10. [微软确认 Windows 存在不可关闭的 GDID 追踪标识符](#item-10) ⭐️ 7.0/10
11. [elfuse 让 macOS Apple Silicon 原生运行 Linux ELF 二进制文件](#item-11) ⭐️ 7.0/10
12. [Epic 和解撤回后，Google Play 下周将支持第三方应用商店](#item-12) ⭐️ 7.0/10
13. [The Memory Heist：浏览器攻击利用操作系统内存去重机制泄露跨域数据](#item-13) ⭐️ 7.0/10
14. [安全研究人员披露 Cursor IDE 零日任意代码执行漏洞](#item-14) ⭐️ 7.0/10
15. [泄露文件曝光 Suno 未经授权抓取音乐数据](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Stripe 与 Advent 联合出价 530 亿美元收购 PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 8.0/10

据报道，Stripe 与私募股权公司 Advent International 已联合出价超过 530 亿美元收购 PayPal，这将使 Stripe、PayPal、Venmo、Braintree 和 Xoom 等主要在线支付处理商归于同一企业旗下。 这项拟议中的巨型合并将通过整合在线支付领域最大的两家竞争对手来彻底改变行业格局，由于其在无卡（CNP）支付市场中造成的集中度，可能会引发严厉的反垄断审查。 合并后的实体将控制在线支付市场的绝大部分份额，PayPal 和 Stripe 分别占据约 43%和 21%的市场份额；社区成员担心，与 PayPal 相比，Stripe 更严格的内容政策可能会对与大麻相关和成人相关行业的商户产生负面影响。

hackernews · rvz · Jul 15, 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: Stripe 和 PayPal 是在线支付处理领域的两大主导企业，为企业和个人提供互联网收款服务。Advent International 是一家总部位于波士顿的全球性私募股权公司，成立于 1981 年，专注于跨多个大陆的收购业务。赫芬达尔-赫希曼指数（HHI）是反垄断监管机构常用的市场集中度衡量指标，用于评估合并是否会实质性削弱竞争。Braintree、Venmo 和 Xoom 均为 PayPal 旗下的支付相关服务，交易完成后将转入合并后的实体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Advent_International">Advent International - Wikipedia</a></li>
<li><a href="https://6sense.com/tech/payment-management/stripe-market-share">Stripe - Market Share, Competitor Insights in Payment Management</a></li>
<li><a href="https://tech-insider.org/stripe-vs-paypal-2026/">Stripe vs PayPal 2026: 5.4x Currency Gap and $12K Fee Divide</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体持怀疑态度，从业者担心竞争减少会导致交易费用上涨，Stripe 更严格的内容政策将取代 PayPal 更宽松的做法，以及行业整合会降低企业支付渠道的冗余性、增加系统性风险。

**标签**: `#fintech`, `#mergers-and-acquisitions`, `#payments`, `#antitrust`, `#stripe`

---

<a id="item-2"></a>
## [研究人员绕过 Claude 的 web_fetch 防护机制窃取用户数据](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

安全研究员 Ayush Paul 发现并成功演示了绕过 Anthropic 为 Claude 设置的 web_fetch 防护机制的方法，通过嵌套链接跟随攻击提取了用户的敏感数据，包括姓名、居住城市和雇主信息。 该漏洞暴露了 AI 智能体安全架构中的关键缺陷，表明即使是为防止数据外泄而精心设计的防护措施，在允许工具递归访问已获取页面内容时也可能存在细微漏洞。 该攻击利用了 web_fetch 能够导航到先前获取页面中嵌入的 URL 这一特性，使得蜜罐网站可以引导 Claude 逐字母提取数据；Anthropic 随后通过移除 web_fetch 的嵌套链接导航功能修复了这一漏洞。

rss · Simon Willison · Jul 15, 14:21

**背景**: Simon Willison 提出了'致命三重奏'（lethal trifecta）一词，用于描述 AI 智能体的三类危险漏洞组合：访问私人数据、接触不可信内容以及具备外部通信能力。Anthropic 的 web_fetch 工具正是针对这一威胁模型设计了防护机制，将导航限制在用户输入的精确 URL 或 web_search 返回的结果上。然而，该工具能够跟随已获取内容中嵌入的链接，这意外形成了可绕过上述确定性防护措施的攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/">The lethal trifecta for AI agents: private data, untrusted content, and external communication</a></li>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论对 Anthropic 在公开演示后仍决定不支付漏洞赏金表示担忧，部分评论者质疑该公司是否确实在内部发现了该问题。另一些人则强调，当多种能力以复杂方式交互时，AI 工具设计会产生不可预见的安全边界，这是一种更广泛的模式。

**标签**: `#AI security`, `#prompt injection`, `#data exfiltration`, `#Claude`, `#Anthropic`

---

<a id="item-3"></a>
## [OpenAI 发布 GPT-Red 自动化 AI 安全测试系统](https://openai.com/index/unlocking-self-improvement-gpt-red) ⭐️ 8.0/10

OpenAI 推出了 GPT-Red，这是一个利用自我博弈（self-play）来提升 AI 安全性、对齐性以及对提示注入攻击抵抗力的自动化红队测试系统。该系统于 2026 年 7 月 15 日发布，目前仅限内部使用。 GPT-Red 代表了一种可规模化提升模型安全性的新方法，通过自动化发现传统上需要人类红队才能找到的漏洞。这有望大幅加速 AI 系统对抗性攻击测试与强化的速度，解决负责任 AI 部署中的关键瓶颈。 该博客文章对 GPT-Red 的自我博弈机制如何实现、以及与之前的自动化红队测试方法有何不同等技术细节披露有限。该系统特别聚焦于提示注入鲁棒性，这是一种已被充分记录的漏洞，攻击者会在良性提示中嵌入恶意指令以操纵 LLM 输出。

rss · OpenAI Blog · Jul 15, 10:00

**背景**: 红队测试（red teaming）是一种安全实践，专家故意尝试发现系统中的漏洞以改进其防御能力。自我博弈（self-play）是一种强化学习技术，智能体通过与自身对抗来提升表现，著名的例子包括 AlphaGo。提示注入攻击利用了 LLM 会遵循输入中任意位置指令的特性，攻击者通过在用户提供的文本中嵌入恶意命令来覆盖模型的预期行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/unlocking-self-improvement-gpt-red/">GPT - Red : Unlocking Self-Improvement for Robustness | OpenAI</a></li>
<li><a href="https://www.oflight.co.jp/en/columns/openai-gpt-red-self-improving-safety-2026-07">OpenAI 's GPT - Red Explained: Automated Red - Teaming ... | Oflight Inc.</a></li>
<li><a href="https://www.iankhan.com/gpt-red-unlocking-self-improvement-for-robustness/">GPT - Red : Automated Red Teaming for AI Safety - Ian Khan</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#red teaming`, `#prompt injection`, `#self-play`, `#OpenAI`

---

<a id="item-4"></a>
## [Thinking Machines 发布 Inkling：最大的开源权重多模态模型，支持音频](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 7.0/10

Thinking Machines 发布了 Inkling，这是一款支持文本、图像和音频处理的开源权重多模态 AI 模型，也是目前支持音频能力的最大开源权重模型。该模型可以通过 Tinker 进行微调，社区成员已经为其制作了 GGUF 和 NVFP4 版本以支持本地部署。 Inkling 通过将多模态能力与前所未有的音频支持规模相结合，为开源权重生态系统增添了重要一员，使企业能够以潜在更低的成本拥有和定制适合自身任务的模型。它的发布加剧了开源模型领域的竞争，并为开发需要跨模态长上下文理解的智能体应用提供了更多选择。 Inkling 并未被定位为当前最强的模型，而是作为一个具有高效思考能力、可定制的开源权重基础模型；该模型已被整合到 llama.cpp 分支和 Unsloth 生态系统中，以便进行本地部署和微调。

hackernews · vimarsh6739 · Jul 15, 18:12 · [社区讨论](https://news.ycombinator.com/item?id=48924912)

**背景**: 开源权重模型是指将其训练完成的参数公开发布的 AI 模型，允许任何人下载、运行、修改和微调。多模态 AI 是指能够在单一统一架构内处理和理解多种输入数据类型（如文本、图像和音频）的系统。微调是指通过针对特定数据集进一步训练预训练模型，使其适应特定任务或行为方式的过程，这对于希望获得定制化 AI 解决方案而无需依赖专有闭源模型的企业来说日益重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://arxiv.org/html/2408.13296v1">The Ultimate Guide to Fine-Tuning LLMs from Basics to ...</a></li>

</ul>
</details>

**社区讨论**: 社区对 Inkling 的多模态能力和本地部署潜力表现出真正的热情，尤其关注其音频功能与竞争对手的比较；一些评论者认为 Thinking Machines 有望成为 DeepSeek 等中国开源模型领导者的美国 counterpart，而另一些人则反思现代模型开发日益复杂和竞争激烈的本质，将其形容为需要不断创新才能维持地位的「红皇后竞赛」。

**标签**: `#open-source-llm`, `#multimodal-ai`, `#audio-models`, `#model-finetuning`, `#thinking-machines`

---

<a id="item-5"></a>
## [13 年老 Xeon 无 GPU 运行 Gemma 4 26B 达 5 token/秒](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 7.0/10

一名工程师在一台没有 GPU 的 13 年老款 Intel Xeon 服务器上成功以每秒 5 个 token 的速度运行 Google 的 Gemma 4 26B 语言模型，证明经过优化的现代 LLM 可以在老旧硬件上运行。 这一成果挑战了关于 LLM 硬件需求的固有假设，并引发了关于本地推理与云端推理成本效益的争论，尤其对于成本敏感型部署和边缘计算场景具有参考价值。 Gemma 4 26B A4B 采用混合专家（MoE）架构，其中'A4B'表示 260 亿总参数中仅有 40 亿活跃参数，从而实现高效推理；社区成员指出类似配置功耗达 300-500W，并计算得出本地电费成本可能超过云端 API 定价，约为每百万 token 0.30 美元。

hackernews · neomindryan · Jul 15, 15:34 · [社区讨论](https://news.ycombinator.com/item?id=48922434)

**背景**: Gemma 4 是 Google 于 2026 年 6 月发布的最新开源模型家族，包含密集型和 MoE 架构，参数量从 20 亿到 310 亿不等。像 Gemma 4 26B A4B 这样的 MoE 模型每个 token 仅激活部分参数，因此比传统密集型模型更高效，尽管总参数量很大。通过 llama.cpp 和 Intel PyTorch 扩展等框架，基于 CPU 的 LLM 推理已获得显著优化，但 GPU 仍是高吞吐量应用的首选。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B">google/gemma-4-26B-A4B · Hugging Face</a></li>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 4 model overview | Google AI for Developers</a></li>
<li><a href="https://www.intel.com/content/www/us/en/developer/articles/technical/boost-performance-llms-pytorch-xeon-processors-pt2.html">Boost Performance for LLMs Using PyTorch: Part 2 - Intel</a></li>

</ul>
</details>

**社区讨论**: 社区成员提供了多元但技术深入的视角：一些人看好技术民主化潜力，有用户预测到 2027 年消费者硬件上可运行 2000 亿参数以上的 MoE 模型；另一些人则进行了详细的总拥有成本分析，指出云端推理可能比本地电费更便宜，尤其在德国等高电价地区——500W 本地推理生成 18000 个 token 约需 0.15 美元，而 API 提供商仅需约 0.005 美元。

**标签**: `#LLM inference`, `#edge computing`, `#hardware optimization`, `#cost analysis`, `#open models`

---

<a id="item-6"></a>
## [完整 Firefox 浏览器被移植到 WebAssembly 中运行](https://developer.puter.com/labs/firefox-wasm/) ⭐️ 7.0/10

一名开发者已将整个 Firefox 浏览器——包括 Gecko 渲染引擎、SpiderMonkey JavaScript 引擎和所有 UI 组件——编译到 WebAssembly 中，使其能够通过 canvas 元素在另一个浏览器内运行，并通过 WISP 协议实现端到端加密。 该项目拓展了 WebAssembly 的能力边界，证明复杂的原生应用可以在浏览器中完全模拟，这可能使得在限制原生应用安装的封闭系统上运行现代浏览器成为可能。 该移植版本包含一个新颖的 WASM→JS JIT 编译器用于实验性加速站点加载，调试和研究消耗了超过 25,000 美元的 AI token，但其内存占用较高，且递归自托管（Firefox 中运行 Firefox）会变得不稳定。

hackernews · coolelectronics · Jul 15, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48926939)

**背景**: WebAssembly（WASM）是一种低级二进制指令格式，旨在作为编程语言的便携编译目标，在浏览器中实现接近原生的性能。Gecko 是 Mozilla 的开源浏览器引擎，为 Firefox 提供支持；SpiderMonkey 则是其 JavaScript 和 WebAssembly 引擎，最初由 Brendan Eich 编写。WISP 协议是一种轻量级标准，用于在单个 WebSocket 连接上代理多个 TCP/UDP 套接字，该项目利用它来实现加密网络连接。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://spidermonkey.dev/">Home | SpiderMonkey JavaScript/WebAssembly Engine</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpiderMonkey">SpiderMonkey - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区成员对实际应用场景表示兴奋，例如在封闭的电视操作系统上运行 Firefox 以实现广告拦截；但也有人质疑 25,000 美元只是"趣味实验"的说法，并指出递归嵌套（Firefox 中的 Firefox 中的 Firefox）虽然可行，但极不稳定。

**标签**: `#WebAssembly`, `#Firefox`, `#browser-engineering`, `#JIT-compilation`, `#web-technology`

---

<a id="item-7"></a>
## [misa77 编解码器实现两倍于 LZ4 的解压速度](https://github.com/welcome-to-the-sunny-side/misa77) ⭐️ 7.0/10

开发者 welcome-to-the-sunny-side 发布了 misa77，这是一种新的无损压缩编解码器，在 Intel x86-64 上可达到 5,219 MB/s 的解压吞吐量，是 LZ4 的 2,505 MB/s 的两倍多，同时保持了可比的压缩率。代价是压缩速度显著变慢，misa77 的编码速度仅为 54.5 MB/s，而 LZ4 为 371 MB/s。 这一进展提升了数据库存储、游戏资源流式和日志处理等解压密集型工作负载的最先进水平，在这些场景中解压速度是瓶颈。该工程表明，在成熟的压缩领域，通过针对 CPU 微架构的优化而非算法突破，仍然可以实现显著的性能提升。 速度提升主要来自减少分支以及设计对 CPU 乱序执行友好的格式，但该项目目前处于 v0.x.y 实验状态，对无效输入会产生未定义行为。在 Silesia 语料库基准测试中，misa77 -0 的压缩率为 42.64%，而 LZ4 为 47.59%；LZ4HC -12 则以更慢的编码速度换取了更好的压缩率（36.45%）。

hackernews · nonadhocproblem · Jul 15, 15:58 · [社区讨论](https://news.ycombinator.com/item?id=48922838)

**背景**: LZ4 由 Yann Collet 开发，于 2011 年发布，是一种广泛使用的 LZ77 家族无损压缩算法，优先考虑极快的压缩和解压速度而非最大压缩率。它是系统性能工程中的标准基准，解压速度可达每核数 GB/s，在现代多核系统上受限于内存速度。Silesia 语料库是 2003 年在西里西亚工业大学开发的标准压缩基准数据集，旨在覆盖计算中使用的典型数据类型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LZ4_(compression_algorithm)">LZ4 (compression algorithm) - Wikipedia</a></li>
<li><a href="https://github.com/lz4/lz4">GitHub - lz4/lz4: Extremely Fast Compression algorithm LZ4 - Extremely fast compression Basic Compression Library (lz4.c) | lz4/lz4 | DeepWiki LZ4 compression algorithm : A Deep Dive Data Compression: LZ77 vs. LZ4 vs. LZ4HC - Baeldung lz4/doc at dev · lz4/lz4 · GitHub</a></li>
<li><a href="http://mattmahoney.net/dc/silesia.html">Silesia Open Source Compression Benchmark - Matt Mahoney</a></li>

</ul>
</details>

**社区讨论**: 专家 danlark1 将该权衡置于已知背景中：优化面向 memcpy 密集型解码需要以格式限制换取更慢的编码。wolf550e 标记了关于实验性 v0.x.y 状态和对无效输入产生未定义行为的关键注意事项，而 mijoharas 则质疑是什么具体洞见实现了加速。scottchiefbaker 称赞结果很有前景，但指出 README 缺少面向开发者的集成示例。

**标签**: `#compression`, `#performance`, `#systems-programming`, `#algorithms`, `#open-source`

---

<a id="item-8"></a>
## [AI Weekly 发布免费可搜索的 159 个真实 AI 部署案例库](https://aiweekly.co/issues/applied-ai-is-here-whats-working-what-got-pulled-back-and) ⭐️ 7.0/10

AI Weekly 发布了一个无需注册即可免费使用的 AI 用例库（AI Use-Case Library），收录了横跨 21 个行业的 159 个具名真实 AI 部署案例，其中 77 个案例附有工具、供应商和报告成果，还包括 6 个被叫停或撤销的案例。 该案例库填补了 AI 从业者和决策者的关键信息缺口——他们在投入预算前需要具体的参考先例，而在企业级 AI 采用加速、但可靠案例研究仍然匮乏的当下，这一资源为成功与失败案例都提供了难得的透明度。 该库收录了 159 个部署中 77 个案例的报告成果，并特别包含 6 个被叫停或撤销的案例，这些失败案例可能提供特别有价值的学习机会；整个库支持搜索功能，旨在为预算编制前的研究和供应商评估提供支持。

rss · AI Weekly · Jul 15, 00:00

**背景**: 应用型 AI（Applied AI）指的是将人工智能技术落地到真实的商业和组织场景中，而非停留在研究或理论层面。企业级 AI 的采用增长迅速，但从业者往往难以找到包含供应商信息、实际成果、尤其是失败案例的详细且经过验证的案例研究，而失败案例通常很少被公开。像这个案例库这样的"先例档案"可以作为实用参考，帮助组织在投入大量资源之前降低风险并辅助决策。

**标签**: `#applied-ai`, `#ai-adoption`, `#enterprise-ai`, `#case-studies`, `#ai-failures`

---

<a id="item-9"></a>
## [FreeBSD 16 从基础系统中移除全部 GPL 代码](https://www.phoronix.com/news/FreeBSD-16-Goes-GPL-Free) ⭐️ 7.0/10

FreeBSD 16 完成了长达数年的努力，通过用 BSD 许可证的替代工具替换最后剩余的 GNU 组件，从其基础系统中移除了所有 GPL 许可的代码。 这一里程碑为下游用户和厂商提供了更大的许可证灵活性，这些用户和厂商可能对 GPL 要求存在顾虑，同时也强化了该项目对宽松型开源许可证的承诺。 被替换的组件包括 diff 和 grep 等常见 GNU 工具，它们已在 BSD Toolchain 项目下被功能等效的 BSD 许可实现所取代。

rss · Lobsters · Jul 15, 12:33

**背景**: FreeBSD 基础系统是随 FreeBSD 一起发布的核心操作系统，与提供第三方软件的 Ports Collection 不同。GNU 通用公共许可证（GPL）是一种 copyleft 许可证，要求衍生作品以相同的许可证条款分发；而 BSD 许可证是一种宽松型许可证，对软件的使用、修改和再分发的限制较少。FreeBSD 的 BSD Toolchain 项目多年来一直致力于用 BSD 许可的替代方案替换 GPL 许可的组件，以减少商业用户的许可证复杂性，并对其代码库保持更大的控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wiki.freebsd.org/BSDToolchain">BSDToolchain - FreeBSD Wiki</a></li>
<li><a href="https://wiki.freebsd.org/GPLinBase">GPLinBase - FreeBSD Wiki</a></li>
<li><a href="https://freebsdfoundation.org/blog/project-update-toolchain-modernization/">Development Project Update: Toolchain Modernization | FreeBSD ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反映了复杂的情绪：一些人称赞这一成就是许可证自由和法律复杂性降低的胜利，而另一些人则质疑 BSD 替代品在功能和性能上是否能与 GNU 工具相媲美，并争论这项工程投入是否值得。

**标签**: `#FreeBSD`, `#open-source-licensing`, `#operating-systems`, `#GPL`, `#BSD`

---

<a id="item-10"></a>
## [微软确认 Windows 存在不可关闭的 GDID 追踪标识符](https://www.ghacks.net/2026/07/12/microsoft-confirms-windows-gdid-device-identifier-that-cannot-be-disabled-documented-in-fbi-case-filing/) ⭐️ 7.0/10

微软确认存在一种名为 GDID（Global Device ID）的持久性设备级标识符，用户无法将其关闭，该标识符首次在 FBI 针对一名 alleged 黑客的联邦起诉文件中被公开记录。 这一发现对全球 Windows 用户构成了重大隐私隐患，因为该标识符能够实现持久性设备追踪，即使用户通过 VPN 或其他隐私工具试图保护匿名性也无济于事；同时，其在执法案件中的使用表明商业遥测数据如何转化为法庭证据。 GDID 与特定设备上的 Windows 安装绑定，并通过 DiagTrack 遥测服务传输；尽管某些设置可以限制微软收集的数据范围，但终端用户无法完全禁用或移除该标识符本身。

rss · Lobsters · Jul 15, 15:36

**背景**: 像 GDID 这样的设备标识符被操作系统厂商用于遥测、诊断，以及在某些情况下与执法部门合作。持久性标识符与 Cookie 或会话数据不同，因为它们在某些情况下能够在系统重装后依然存在，并与硬件关联。FBI 在 Scattered Spider 黑客案件中使用 GDID，标志着该标识符的存在及其在刑事调查中的应用首次得到公开确认，这重新引发了关于商业软件中安全与隐私平衡的争论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ghacks.net/2026/07/12/microsoft-confirms-windows-gdid-device-identifier-that-cannot-be-disabled-documented-in-fbi-case-filing/">Microsoft Confirms Windows GDID Device Identifier That Cannot Be Disabled, Documented in FBI Case Filing - gHacks Tech News</a></li>
<li><a href="https://cybernews.com/security/windows-telemetry-gdid-helps-arrest-hacker/">Windows telemetry backlash: GDID tracking exposes Scattered ...</a></li>
<li><a href="https://www.windowslatest.com/2026/07/10/you-cant-fully-disable-microsofts-gdid-windows-11-tracker-but-these-settings-limit-what-it-captures/">Microsoft admits Windows 11 has a GDID tracker with no off switch, first documented publicly in an FBI hacker complaint</a></li>

</ul>
</details>

**标签**: `#privacy`, `#windows`, `#forensics`, `#device-tracking`, `#security`

---

<a id="item-11"></a>
## [elfuse 让 macOS Apple Silicon 原生运行 Linux ELF 二进制文件](https://github.com/sysprog21/elfuse) ⭐️ 7.0/10

elfuse 是一款基于 FUSE 的新工具，它能够在 macOS Apple Silicon 上直接运行 ARM64 和 x86-64 架构的 Linux ELF 二进制文件，而无需传统的虚拟机或 Docker 容器。 该工具解决了使用 Apple Silicon Mac 的开发人员在运行 Linux 特定二进制文件时的重大痛点，提供了一种比完整虚拟机更轻量的替代方案，有助于提高工作效率并降低资源消耗。 elfuse 利用 FUSE（用户空间文件系统）框架来拦截和处理 ELF 二进制文件操作，但其实现的稳健性和性能特征仍需更广泛的社区验证。

rss · Lobsters · Jul 15, 19:33

**背景**: ELF（可执行与可链接格式）是 Linux 等类 Unix 系统上用于可执行文件、共享库和目标文件的标准二进制文件格式。FUSE（用户空间文件系统）是一种软件接口，允许非特权用户在不修改内核代码的情况下创建自定义文件系统，从而实现对文件系统操作的创新方法。Apple Silicon Mac 采用 ARM64 架构，如果没有 Rosetta 2 等翻译层，则与 x86-64 二进制文件不兼容，这给需要跨平台兼容性的开发人员带来了挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Filesystem_in_Userspace">Filesystem in Userspace - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rosetta_(software)">Rosetta (software) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#macos`, `#apple-silicon`, `#linux-compatibility`, `#systems-programming`, `#emulation`

---

<a id="item-12"></a>
## [Epic 和解撤回后，Google Play 下周将支持第三方应用商店](https://arstechnica.com/gadgets/2026/07/third-party-app-stores-coming-to-google-play-next-week-as-epic-settlement-withdrawn/) ⭐️ 7.0/10

在 Epic Games 撤回与 Google 的和解协议后，Google 将于下周开始允许第三方应用商店入驻 Google Play 平台。 这标志着 Android 应用分发经济的根本性重组，可能削弱 Google 对应用变现的控制，并为开发者和消费者提供更多发现与购买应用的选择。 这一变化源于持续的反垄断诉讼——2023 年陪审团裁定 Google Play 构成非法垄断，联邦法官此前已下令对 Google 应用商店做法进行重大改革。

rss · Lobsters · Jul 15, 20:05

**背景**: Epic Games 于 2020 年起诉 Google，指控其 Play Store 存在反竞争行为，特别是 30%的应用内购抽成以及对替代支付系统的限制。2023 年，陪审团支持 Epic，裁定 Google 在 Android 应用分发领域维持非法垄断。Google 与 Epic 在 2023 年达成和解，但 Epic 随后撤回和解协议，导致法院下令采取补救措施，包括向竞争对手应用商店开放 Google Play。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/03/google-and-epic-look-to-bury-the-hatchet-with-new-app-store-settlement/">Google and Epic announce settlement to end app store ...</a></li>
<li><a href="https://themainstream.co.in/google-proposes-lower-play-store-fees/">Google proposes lower Play Store fees and access for rival app stores...</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#mobile-platforms`, `#app-distribution`, `#google-play`, `#epic-games`

---

<a id="item-13"></a>
## [The Memory Heist：浏览器攻击利用操作系统内存去重机制泄露跨域数据](https://ayush.digital/blog/the-memory-heist) ⭐️ 7.0/10

安全研究员 Ayush 发表了一篇详细的技术分析，展示了一种新型基于浏览器的侧信道攻击，该攻击结合 WebAssembly、时序攻击和操作系统内存去重机制，实现跨域数据泄露。 该攻击将浏览器安全边界与操作系统级内存优化联系起来，证明内存去重——现代操作系统中的一项性能特性——可被武器化以对抗同源策略等 Web 安全模型，可能影响数百万用户。 该攻击利用内存去重引发的写时复制页错误作为可测量的时序侧信道，而 WebAssembly 提供了精细控制内存访问模式的能力，这是在浏览器跨域场景下实施攻击所必需的。

rss · Lobsters · Jul 15, 00:11

**背景**: 内存去重是一种操作系统优化技术，它将跨进程的相同内存页合并为共享的写时复制映射以节省 RAM，但这会产生侧信道，因为对去重页写入会触发可被测量时长的页错误和复制操作。WebAssembly 是一种在浏览器中运行的低层字节码格式，具有接近原生的性能和直接内存访问能力，这使其成为构建精确时序攻击的有力工具。跨域数据泄露攻击旨在窃取用户打开的其他网站的信息，违反了通常隔离 Web 内容的同源策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/266522793_Software_Side_Channel_Attack_on_Memory_Deduplication">(PDF) Software Side Channel Attack on Memory Deduplication</a></li>
<li><a href="https://arxiv.org/abs/2111.08553v1">[2111.08553v1] Remote Memory-Deduplication Attacks - arXiv.org</a></li>
<li><a href="https://weihang-wang.github.io/papers/WaSCR.pdf">WaSCR: A WebAssembly Instruction-Timing Side Channel Repairer</a></li>

</ul>
</details>

**标签**: `#security`, `#side-channel-attack`, `#browser-security`, `#memory-deduplication`, `#webassembly`

---

<a id="item-14"></a>
## [安全研究人员披露 Cursor IDE 零日任意代码执行漏洞](https://mindgard.ai/blog/cursor-0day-when-full-disclosure-becomes-the-only-protection-left) ⭐️ 7.0/10

Mindgard 的安全研究人员在声称负责任的披露流程失败后，公开披露了流行 AI 驱动开发工具 Cursor IDE 中的一个零日漏洞，该漏洞允许任意代码执行。据报道，该缺陷使得攻击者在用户仅打开受感染的代码仓库时就能在 Windows 机器上执行恶意代码，无需额外的点击或明确的用户批准。 这一披露对广泛采用的 AI 编程工具的安全实践提出了严重关切，这些工具作为传统 IDE 的替代方案已获得大量开发者采用。该漏洞的执行门槛极低——仅需开发者打开恶意代码仓库即可触发——再加上协调披露机制的失效，凸显了快速扩张的 AI 辅助开发生态系统中的系统性风险。 该漏洞特别影响 Windows 系统，Cursor 会在未获取用户同意的情况下自动从打开项目的根目录搜索并执行 git.exe，为攻击者创造了受信任的执行路径。研究人员在据称负责任的披露失败后选择了完全公开披露，这反映了安全社区中关于供应商响应速度和研究人员保护的持续紧张关系。

rss · Lobsters · Jul 15, 02:02

**背景**: Cursor 是一款基于 Visual Studio Code 构建的 AI 驱动集成开发环境（IDE），因其先进的代码补全和 AI 辅助编程功能而在开发者中获得广泛欢迎。负责任的披露是安全行业的标准做法，研究人员私下向供应商报告漏洞，在公开披露前留出修复时间以保护用户。当这一流程失效时，研究人员有时会采取"完全披露"——立即公开所有细节——以迫使对方采取行动或直接警告用户，但这可能使未修补的系统面临被利用的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/security">Cursor · Security</a></li>
<li><a href="https://snyk.io/blog/responsible-disclosure/">Responsible disclosure : the impact of vulnerability ... | Snyk</a></li>
<li><a href="https://www.remio.ai/post/cursor-ide-0day-vulnerability-allows-arbitrary-code-execution-by-opening-malicious-repository">Cursor IDE 0day Vulnerability Allows Arbitrary Code Execution by...</a></li>

</ul>
</details>

**社区讨论**: 新闻项目中提到的 Lobste.rs 讨论可能包含关于漏洞利用机制和技术细节以及披露方法伦理性的技术辩论，开发者们在权衡完全披露的风险与协调漏洞报告机制的失效。社区情绪在此类事件中通常反映分歧观点：一些人支持研究人员在正规渠道失效时公开披露的决定，另一些人则担心使用户暴露于未修补的漏洞风险中，还有许多人讨论 Cursor 用户的实际缓解措施。

**标签**: `#security`, `#vulnerability-disclosure`, `#cursor-ide`, `#arbitrary-code-execution`, `#ai-tools`

---

<a id="item-15"></a>
## [泄露文件曝光 Suno 未经授权抓取音乐数据](https://www.theverge.com/ai-artificial-intelligence/966072/suno-ai-music-training-scraping-youtube-hack) ⭐️ 7.0/10

据 404 Media 报道，通过黑客事件获取的泄露文件显示，AI 音乐生成器 Suno 通过从 YouTube Music、Deezer 和 Genius 抓取数百万首受版权保护的歌曲和歌词来训练其模型，且未获得授权。 这一披露对生成式 AI 行业具有重大法律和伦理影响，因为它揭露了一家资金雄厚的 AI 音乐公司可能存在的版权侵权行为，并凸显了 AI 训练数据实践持续缺乏透明度的问题。 Suno 此前一直回避披露其训练数据集的内容或获取方式，这使得此次泄露尤为具有揭示意义。黑客入侵的角度增加了新闻价值，但未经授权抓取数据用于 AI 训练已成为行业内越来越常见的问题。

rss · The Verge · Jul 15, 17:48

**背景**: Suno 是一个根据文本提示生成原创音乐的生成式 AI 平台，定位为可制作专业级音频的工具。使用受版权保护的材料训练 AI 模型的法律地位仍然存在激烈争议，各公司常以合理使用为由进行辩护，而权利人则认为这构成侵权。YouTube 的 API 服务条款明确禁止未经授权下载、导入或存储音视频内容的副本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.google.com/youtube/terms/api-services-terms-of-service">YouTube API Services Terms of Service | Google for Developers</a></li>
<li><a href="https://dataprixa.com/web-scraping-for-ai-training-legal-issues/">Web Scraping for AI Training : Legal Issues , Best Practices, and...</a></li>
<li><a href="https://thunderbit.com/blog/web-scraping-legal-implications">Is Web Scraping Illegal? Understanding the Legal Implications</a></li>

</ul>
</details>

**标签**: `#AI`, `#copyright-infringement`, `#generative-AI`, `#data-scraping`, `#music-technology`

---