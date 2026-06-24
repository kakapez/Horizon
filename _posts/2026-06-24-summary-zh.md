---
layout: default
title: "Horizon Summary: 2026-06-24 (ZH)"
date: 2026-06-24
lang: zh
---

> From 55 items, 14 important content pieces were selected

---

1. [AI 代理循环标志着软件开发范式的根本转变](#item-1) ⭐️ 8.0/10
2. [研究确认大语言模型优先依据文本风格而非角色标签](#item-2) ⭐️ 8.0/10
3. [存储芯片厂商的中国竞争威胁与微软的中国 AI 模型战略](#item-3) ⭐️ 8.0/10
4. [Swift Package Index 正式加入 Apple](#item-4) ⭐️ 7.0/10
5. [开源所见即所得 TikZ 编辑器，支持源代码实时同步](#item-5) ⭐️ 7.0/10
6. [百度 Unlimited OCR 解决线性 KV 缓存增长问题](#item-6) ⭐️ 7.0/10
7. [加州 AB 2047 法案要求 3D 打印机配备枪支检测算法](#item-7) ⭐️ 7.0/10
8. [谷歌员工因发布 Google Workspace CLI 工具被解雇](#item-8) ⭐️ 7.0/10
9. [漏洞报告已不再具有特殊地位](#item-9) ⭐️ 7.0/10
10. [Haskell 专家发布易懂的记录类型推断指南](#item-10) ⭐️ 7.0/10
11. [Cloudflare 联合主流浏览器推出隐私优先协议 PACT](#item-11) ⭐️ 7.0/10
12. [The Low-Tech AI Of Elden Ring](#item-12) ⭐️ 7.0/10
13. [2026 年 WebAssembly 运行时性能基准测试对比](#item-13) ⭐️ 7.0/10
14. [放缓节奏作为科技工程领域的战略优势](#item-14) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AI 代理循环标志着软件开发范式的根本转变](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

Flask 和 Jinja2 的创建者 Armin Ronacher 发表了一篇文章，认为 AI 驱动的代理循环代表了软件开发中的根本范式转变，从确定性规格说明转向行为更像生命体的软件，这种软件需要全新的交互和设计模式。 这篇文章挑战了软件应通过精确的确定性规格说明来构建这一基础假设，提出代理循环将重新定义开发者与系统的交互和设计方式，对整个软件工程学科具有广泛影响。 代理循环架构使 AI 编码代理能够自主地编写代码、运行测试、观察失败、修复错误并迭代，无需人类在每一步进行干预，从根本上将开发者的角色从编写指令转变为引导和塑造涌现行为。

hackernews · ingve · Jun 23, 11:06 · [社区讨论](https://news.ycombinator.com/item?id=48643180)

**背景**: 规格驱动开发是一种传统的软件工程方法论，其中正式的、详细的规格说明在编写代码之前作为权威的真实来源。相比之下，代理循环是现代 AI 编码代理的核心架构：它允许代理执行任务、观察结果并自主迭代直到达成目标。Armin Ronacher 是一位知名的开源开发者，创建了 Flask 和 Jinja2 这两个广泛使用的 Python 项目，这使得他的观点在开发者社区中具有重要分量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2025/Sep/30/designing-agentic-loops/">Designing agentic loops</a></li>
<li><a href="https://en.wikipedia.org/wiki/Specification-driven_development">Specification-driven development - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者大多认同这一范式转变，但强调了不同的瓶颈：一些人认为清晰度和规格编写仍然是真正的约束，指出没有任何代理能绕过人类理解自己真正想要什么所需的思考时间。另一些人接受了'软件即生命体'的隐喻，认为我们将学会在不理解其内部机制的情况下与软件协作，类似于我们与生命体打交道的方式。一个值得注意的反驳观点区分了目标驱动型工作（代理擅长）和品味驱动型工作（LLM 在美学和判断力上不足）。

**标签**: `#ai-agents`, `#software-development`, `#paradigm-shift`, `#agentic-loop`, `#spec-driven-development`

---

<a id="item-2"></a>
## [研究确认大语言模型优先依据文本风格而非角色标签](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Charles Ye、Jasmine Cui 和 Dylan Hadfield-Menell 的研究论文确认，大语言模型无法可靠地区分特权系统指令与不可信的用户输入，因为模型优先依据文本的风格格式而非<system>、<think>和<user>等结构性角色标签来判断文本的角色归属。 这一发现动摇了针对提示注入的一种常见防御方法，并揭示出除非大语言模型实现真正的角色感知能力，提示注入防御将永远是一场打地鼠游戏，这对生产环境中大语言模型部署的安全性具有重大影响。 研究人员发现，对攻击文本进行"去风格化"处理——即改写文本使其看起来不再像角色标签所期望的格式——会使平均攻击成功率从 61%骤降至 10%，这表明对人类几乎不可见的细微变化却能彻底改变大语言模型的角色感知。

rss · Simon Willison · Jun 22, 23:59

**背景**: 提示注入在 OWASP 大语言模型应用十大安全风险中排名第一，指用户提示以非预期方式改变大语言模型行为的现象。角色标签（如<system>、<think>、<assistant>和<user>）是一种广泛使用的防御机制，旨在帮助模型区分特权指令与不可信输入。越狱技术利用这些弱点绕过 AI 安全护栏，从简单的提示操纵到复杂的多轮攻击，可能导致模型推翻其安全训练。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://genai.owasp.org/llmrisk/llm01-prompt-injection/">LLM01:2025 Prompt Injection - OWASP Gen AI Security Project</a></li>
<li><a href="https://www.ibm.com/think/topics/prompt-injection">What Is a Prompt Injection Attack? | IBM</a></li>

</ul>
</details>

**标签**: `#prompt-injection`, `#ai-security`, `#llm-vulnerabilities`, `#role-confusion`, `#jailbreak`

---

<a id="item-3"></a>
## [存储芯片厂商的中国竞争威胁与微软的中国 AI 模型战略](https://stratechery.com/2026/memory-chips-and-china-microsoft-and-chinese-models/) ⭐️ 8.0/10

Ben Thompson 的 Stratechery 分析指出，三大存储芯片制造商可能无意中为中国存储芯片竞争对手的崛起打开了大门，而这些竞争对手未来可能威胁其市场地位；同时，该分析还揭示了微软在其平台上采用中国 AI 模型的战略动机。 该分析揭示了半导体和 AI 行业中的一个关键战略悖论：向中国的技术转移和供应链整合可能反噬为竞争威胁，而像微软这样的云平台则可能在地缘政治紧张局势下，从拥抱中国 AI 模型中获得商业优势。 该文章将两个看似独立但主题相关的问题——存储芯片供应链动态与 AI 模型采用策略——联系起来，说明中国在硬件和软件两方面日益增长的能力如何为西方现有科技巨头制造战略困境。

rss · Stratechery · Jun 23, 10:00

**背景**: 全球存储芯片市场由三星、SK 海力士和美光三大公司主导，它们共同控制了 DRAM 和 NAND 闪存生产的绝大部分份额。中国的新进入者如长江存储（YMTC）和长鑫存储（CXMT）已崛起为日益强劲的竞争对手，部分原因是通过与既有厂商的合作和合资获得了技术。在 AI 领域，中国开发的模型在能力上快速进步，像微软这样的云服务提供商面临着是否向全球客户提供这些模型的战略抉择。

**标签**: `#geopolitics`, `#semiconductors`, `#AI-competition`, `#China`, `#Microsoft`

---

<a id="item-4"></a>
## [Swift Package Index 正式加入 Apple](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 7.0/10

Swift Package Index 这个由社区运营的开源包搜索引擎（索引了超过 11,000 个 Swift 包）已被 Apple 收购，其创建者已作为全职员工加入 Apple。 此次收购将 Swift 生态系统中主要的包发现工具从社区项目转变为 Apple 官方资源，这可能会改善与 Swift Package Manager 的集成，但也引发了人们对 Apple 控制包分发及其在开源领域历史做法的担忧。 Swift Package Index 目前仅支持 GitHub 仓库，并索引了 11,152 个包的元数据；Apple 明确提到开发者身份验证是未来的发展方向，这引发了一些开发者的担忧。

hackernews · JDevlieghere · Jun 23, 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48648779)

**背景**: Swift Package Index 是一个由社区构建的开源搜索引擎，帮助开发者找到与 Swift Package Manager（SPM）兼容的 Swift 包。在此次收购之前，Swift.org 官方的包页面就已经将用户引导至 SPI 来发现包。Swift 生态系统历史上一直缺乏一个类似于 JavaScript 的 npm 或 Python 的 PyPI 那样完善的官方包注册中心，这使得 SPI 成为填补这一空缺的关键社区驱动资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://swiftpackageindex.com/">Swift Package Index</a></li>
<li><a href="https://www.swift.org/packages/">Packages | Swift.org</a></li>
<li><a href="https://github.com/SwiftPackageIndex">Swift Package Index · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：一些人庆祝创建者的成功，并期望 Swift Package Manager 获得更好的官方支持；另一些人则对 Apple 在开源和开发者服务方面的糟糕记录表示悲观。具体担忧包括潜在的包监管和筛选、开发者身份验证要求，以及 SPI 仅支持 GitHub 仓库的限制——一位评论者认为这是构建竞争产品的机会。

**标签**: `#swift`, `#apple`, `#package-management`, `#open-source`, `#developer-tools`

---

<a id="item-5"></a>
## [开源所见即所得 TikZ 编辑器，支持源代码实时同步](https://tikz.dev/editor/) ⭐️ 7.0/10

一款新的开源所见即所得 TikZ 编辑器（网页和桌面版均已可用）已发布，允许用户通过拖拽和缩放来可视化编辑 LaTeX 图形元素，同时保持源代码与渲染视图实时同步，支持双向编辑。 这解决了学术界长期存在的痛点——学者们需要反复调整坐标并重新编译来手动编写 TikZ 图形，因为此前没有任何编辑器能同时提供所见即所得的可视化编辑和源代码同步功能。 该编辑器通过解析 TikZ 代码并追踪每个对象的精确源代码位置来工作，因此拖拽元素时仅修改坐标数值而不改变换行或缩进；它还包含从 SVG/pptx/IPE 到 TikZ 的转换器、重新实现的 LaTeX 断字和换行算法，以及使用 red!20!black 等 LaTeX 混合颜色记法的颜色选择器。

hackernews · DominikPeters · Jun 23, 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48645437)

**背景**: TikZ 是学术界广泛使用的 LaTeX 绘图包，通过如\draw[->] (0,0) -- (1,2);等命令来程序化地定义线条、形状和文本。与基于标记的 SVG 不同，TikZ 更偏向代码驱动并支持\foreach 循环等结构，功能强大但 notoriously 难以使用，因为定位元素需要手动指定坐标并反复编译查看效果。该项目几乎完全由 AI 编程代理 Codex 构建，作者指出这使得重新实现 TikZ 的大部分功能成为可能——这是一项对人类来说过于繁琐而无法手动完成的任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PGF/TikZ">PGF/TikZ - Wikipedia</a></li>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://tikz.dev/">PGF/TikZ Manual - Complete Online Documentation</a></li>

</ul>
</details>

**社区讨论**: 社区讨论内容丰富，有人称赞该概念，但也有人批评生成的 TikZ 代码不必要地使用了绝对坐标（例如将单个节点放在(0.5,2.91)而非让 TikZ 默认居中）。作者分享该项目通过 Codex 消耗了约 700M tokens，按 API 费率计算成本为 1.5 万美元但通过 ChatGPT 订阅实际仅花费约 500 美元，评论者还提及了 Quiver 等替代工具，并讨论了从 TikZ 迁移到 draw.io 或 Mermaid 的情况。

**标签**: `#latex`, `#tikz`, `#wysiwyg-editor`, `#academic-tools`, `#open-source`

---

<a id="item-6"></a>
## [百度 Unlimited OCR 解决线性 KV 缓存增长问题](https://github.com/baidu/Unlimited-OCR) ⭐️ 7.0/10

百度发布了 Unlimited OCR 开源项目，引入了一种新颖的架构技巧来防止视觉语言模型中 KV 缓存的线性增长，使得能够一次性对任意长度的文档进行 OCR 处理，而不会耗尽 VRAM 或需要分页切割的替代方案。 这消除了长文档 OCR 中的一个主要实际瓶颈——开发者此前不得不构建繁琐的分页切割流程来避免内存崩溃，并为 RAG 管道和其他应用中无缝的端到端文档解析开辟了新的可能性。 该项目致谢了 Deepseek-OCR、Deepseek-OCR-2 和 PaddleOCR 作为基础模型，其名称"Unlimited OCR Works"刻意致敬了《Fate/stay night》中的"Unlimited Blade Works"魔法——该魔法的核心理念是复制他人锻造的武器，恰好映射了该项目基于现有模型构建的方法。配套论文可在 arxiv.org/abs/2606.23050 获取。

hackernews · ingve · Jun 23, 11:35 · [社区讨论](https://news.ycombinator.com/item?id=48643426)

**背景**: 在基于 Transformer 的自回归模型中，KV 缓存存储了先前计算的 Key 和 Value 状态，通过避免重复计算来加速解码。然而，该缓存随已处理 token 数量线性增长 O(N)，这意味着对于长文档，VRAM 需求会变得不可承受并最终导致模型崩溃。这种线性增长问题迫使开发者采用分页切割的替代方案，将长文档拆分为较小的片段分别处理，这引入了复杂性并可能丢失跨页上下文信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/baidu/Unlimited-OCR/tree/main/">GitHub - baidu/Unlimited-OCR: Unlimited OCR Works: Welcome ...</a></li>
<li><a href="https://medium.com/@joaolages/kv-caching-explained-276520203249">Transformers KV Caching Explained | by João Lages | Medium</a></li>
<li><a href="https://arxiv.org/abs/2405.12981">[2405.12981] Reducing Transformer Key-Value Cache Size with Cross-Layer Attention</a></li>

</ul>
</details>

**社区讨论**: 社区称赞了该项目优雅的架构技巧及其对消除繁琐分页流程的实际影响，一位用户指出光学音乐识别是 AI 驱动 OCR 的一个有前景的全新应用领域。评论者还赞赏了项目对 Deepseek-OCR 和 PaddleOCR 的慷慨致谢，并注意到项目名称中对《Fate/stay night》的巧妙文化致敬，这在隐喻上与基于他人基础工作构建的方法相契合。

**标签**: `#ocr`, `#kv-cache`, `#memory-optimization`, `#vision-language-models`, `#baidu`

---

<a id="item-7"></a>
## [加州 AB 2047 法案要求 3D 打印机配备枪支检测算法](https://www.the3dprintingnerd.com/ab2047) ⭐️ 7.0/10

加州众议员 Bauer-Kahan 在 2025-2026 立法会议中提出的 AB 2047 法案，要求所有在加州销售 3D 打印机的制造商为其产品配备枪支蓝图检测算法，并在 2029 年 3 月 1 日前向相关部门提交合规证明。 该法案可能严重限制学生、教育工作者和企业使用 3D 打印机的权限，并引发了关于强制要求一项无法真正检测数字文件'意图'的技术是否合理的根本性问题，可能为其他州或技术领域的类似监管过度扩张开创先例。 该法案要求制造商为每种型号提交证明，确认已配备枪支蓝图检测算法，但批评者指出 3D 打印机执行的是描述物理运动的 G-code 指令，本质上无法判断所打印形状的语义用途或意图。

hackernews · Buildstarted · Jun 23, 22:12 · [社区讨论](https://news.ycombinator.com/item?id=48652184)

**背景**: 3D 打印机通过读取描述物理运动和挤出的机器指令（如 G-code）来运行，而非所创建对象的语义含义或用途。自 2013 年首个全 3D 打印枪支设计在网上分享以来，关于 3D 打印枪支的争论持续不断，引发了各种监管尝试。该法案延续了加州对技术进行激进监管的模式，类似于近期失败的 SB 1047 法案（旨在监管前沿 AI 模型），也呼应了复印机中的货币防伪检测等现有 DRM 系统——这些系统历史上一直容易被有动机的用户绕过。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260AB2047">Bill Text - AB-2047 Firearms: 3-dimensional printing blocking technology.</a></li>
<li><a href="https://calmatters.digitaldemocracy.org/bills/ca_202520260ab2047">AB 2047: Firearms: 3-dimensional printing blocking technology.</a></li>

</ul>
</details>

**社区讨论**: 社区 overwhelmingly 反对该法案，评论者强调从几何数据中检测'意图'在技术上不可能实现，并将其与容易被绕过的 DRM 系统（如美元复印防伪保护）作类比，指出这类措施只能阻止'完全没有动机'的用户。一位评论者讽刺地设想了一个 AI 云服务预先审查 STL 文件武器意图的反乌托邦未来，其他人则对监管过度扩张及据称由 Bloomberg 推动的游说势力表示担忧。

**标签**: `#regulation`, `#3d-printing`, `#technology-policy`, `#education`, `#maker-community`

---

<a id="item-8"></a>
## [谷歌员工因发布 Google Workspace CLI 工具被解雇](https://twitter.com/JPoehnelt/status/2069482265953087602) ⭐️ 7.0/10

谷歌员工 Justin Poehnelt 因在"googleworkspace" GitHub 组织下个人发布了一个可能被误认为谷歌官方产品的 CLI 工具而被解雇，引发了关于企业开源政策的广泛讨论。 此案例凸显了大型科技公司中员工自发开源创新与企业治理之间的紧张关系，引发了关于谁控制企业命名空间下的发布以及员工发布与雇主产品相关工具时面临何种风险的关键问题。 该 CLI 工具在运行时动态读取 Google Discovery Service 来构建整个命令界面，自动获取新的 API 端点；值得注意的是，该工具现在似乎已正式托管在 googleworkspace GitHub 组织上，暗示谷歌可能在该员工被解雇后正式采纳了该项目。

hackernews · justinwp · Jun 23, 18:13 · [社区讨论](https://news.ycombinator.com/item?id=48649011)

**背景**: 谷歌维护着诸如"googleworkspace"等官方 GitHub 组织，用于发布与其产品相关的开源工具和库。在某些时期（如 2015-2021 年），谷歌员工和团队向这些谷歌管理的 GitHub 组织发布项目是常见做法。然而，企业政策要求在发布任何可能被视为谷歌官方产品的内容之前必须获得正式审批，未经批准在雇主官方命名空间下发布工具会带来严重的品牌混淆和法律责任风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/googleworkspace/cli">GitHub - googleworkspace/cli: Google Workspace CLI — one ...</a></li>
<li><a href="https://github.com/googleworkspace/cli/releases">Releases · googleworkspace/cli - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区讨论分歧严重：一些人认为解雇是合理的，因为在雇主官方命名空间下未经审批发布工具显然存在风险并会造成真正的混淆；另一些人则同情创作者，将解雇视为惩罚真正创新的官僚过度行为。现任/前任谷歌员工指出，向谷歌管理的 GitHub 组织发布项目历史上是常见做法，有人引用普奈尔官僚铁律来批评创新者最终受制于内部官僚的现象。

**标签**: `#google`, `#open-source`, `#employment`, `#corporate-policy`, `#cli`

---

<a id="item-9"></a>
## [漏洞报告已不再具有特殊地位](https://words.filippo.io/vuln-reports/) ⭐️ 7.0/10

Filippo Valsorda 发表了一篇文章，主张在当前的安全形势下，漏洞报告不应再被视为特殊或例外，这挑战了信息安全社区中长期存在的惯例。 这位知名密码学专家的观点可能会重塑组织和开发者对安全披露的优先级排序、处理流程和响应方式，可能推动漏洞处理向更常规的缺陷修复流程转变。 Valsorda 是密码学和安全领域备受尊敬的人物，曾领导 Google 的 Go 密码学团队，这使他对既有漏洞报告实践的批评具有相当大的影响力。

rss · Lobsters · Jun 23, 13:47

**背景**: 漏洞报告传统上一直被赋予更高的紧迫性和特殊协议，包括协调披露时间线、CVE 跟踪系统和漏洞赏金计划，这些都将安全漏洞与普通软件缺陷区分开来。传统观点认为，安全漏洞因其对用户和系统的潜在影响而应获得特殊处理。Valsorda 的论点挑战了这一范式，认为当前的安全形势已经演变到足以说明这种例外处理不再合理或有效。

**社区讨论**: 该文章在 Lobsters 上引发了讨论，表明该话题引起了更广泛的安全和开发者社区的共鸣，但提供的材料中未包含评论区的具体观点。

**标签**: `#security`, `#vulnerability-reporting`, `#infosec`, `#software-engineering`, `#community-practices`

---

<a id="item-10"></a>
## [Haskell 专家发布易懂的记录类型推断指南](https://haskellforall.com/2026/06/record-type-inference-for-dummies) ⭐️ 7.0/10

Gabriella Gonzalez 在她的 Haskell for All 博客上发布了题为"Record type inference for dummies"的新文章，通过记录构造和字段访问等具体示例，逐步讲解了记录类型的类型推断是如何工作的。 记录类型推断是编程语言理论和类型系统设计中公认的难题，Gonzalez 的通俗化讲解让这一高级主题能够被更广泛的开发者与语言设计者所理解。 文章通过包含"name"和"age"等字段的记录构造以及字段访问等示例表达式，逐步演示类型推断规则，先在简化场景中展示推断机制，再处理更复杂的情况。

rss · Lobsters · Jun 23, 12:46

**背景**: 类型推断是编程语言中自动检测表达式类型的过程，无需程序员提供显式的类型标注。记录类型将命名的字段组合在一起，当涉及记录拼接或扩展等操作时，推断其类型变得尤为困难。行多态（Row polymorphism）是类型理论中的相关概念，它允许对记录类型进行结构多态——使函数能操作具有不同字段集合的记录——而非依赖名义类型相等性。研究已证明带记录拼接的 lambda 演算的类型推断是可判定的，但在 Haskell 等语言中的实际实现仍面临显著的设计挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://haskellforall.com/2026/06/record-type-inference-for-dummies">Haskell for all: Record type inference for dummies</a></li>
<li><a href="https://en.wikipedia.org/wiki/Row_polymorphism">Row polymorphism - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/089054019190050C">Type inference for record concatenation and multiple inheritance - ScienceDirect</a></li>

</ul>
</details>

**社区讨论**: 与该文章关联的 lobste.rs 讨论链接表明编程语言社区正在进行实质性的技术讨论，说明读者在积极探讨所呈现的类型推断方法的细节与影响。

**标签**: `#type-inference`, `#haskell`, `#programming-languages`, `#type-systems`, `#functional-programming`

---

<a id="item-11"></a>
## [Cloudflare 联合主流浏览器推出隐私优先协议 PACT](https://cloudflare.net/news/news-details/2026/Cloudflare-Collaborates-With-Leading-Browsers-to-Develop-a-Privacy-First-Protocol-For-the-Global-Internet/default.aspx) ⭐️ 7.0/10

Cloudflare 宣布了一项名为 PACT（Private Access Control Tokens）的新计划，与 Mozilla Firefox、Google Chrome、Microsoft Edge 及 Shopify 合作开发，并将提交标准化，旨在帮助人类和机器人证明其流量非恶意的同时保护隐私。 Cloudflare 与三大主流浏览器引擎的协作代表了行业巨头在隐私标准上的罕见共识，可能重塑全球互联网流量验证的方式，用隐私保护方案替代当前侵入式的机器人检测方法（如 CAPTCHA 验证码）。 PACT 旨在允许客户端证明自身非恶意流量而无需泄露个人身份信息，该协议将提交至 IETF 等标准组织进行正式标准化。

rss · Lobsters · Jun 23, 16:20

**背景**: 目前，网站依赖 CAPTCHA 验证码和浏览器指纹等方法区分正常人类流量与恶意机器人，但这些方式具有侵入性且损害用户隐私。Cloudflare 自 2020 年起便致力于隐私保护协议的研发，通过与 Mozilla、Google 等合作伙伴在 IETF 框架下设计和部署互联网规模的隐私技术。PACT 似乎是这一努力的下一步演进，将概念从浏览器级隐私令牌扩展到更广泛的访问控制框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businesswire.com/news/home/20260622906058/en/Cloudflare-Collaborates-With-Leading-Browsers-to-Develop-a-Privacy-First-Protocol-For-the-Global-Internet">Cloudflare Collaborates With Leading Browsers to Develop a Privacy-First Protocol For the Global Internet</a></li>
<li><a href="https://blog.cloudflare.com/next-generation-privacy-protocols/">Helping build the next generation of privacy-preserving protocols</a></li>

</ul>
</details>

**社区讨论**: 该新闻在 lobste.rs 上引发了讨论，但具体评论内容未提供；讨论帖的存在表明社区对 Cloudflare 这样的大型基础设施提供商与浏览器厂商共同塑造互联网隐私标准的潜在影响表示关注。

**标签**: `#privacy`, `#internet-protocols`, `#cloudflare`, `#browser-standards`, `#web-security`

---

<a id="item-12"></a>
## [The Low-Tech AI Of Elden Ring](https://nega.tv/posts/low-tech-ai-of-elden-ring.html) ⭐️ 7.0/10

An analysis of how Elden Ring implements effective game AI using relatively simple, low-tech approaches rather than cutting-edge machine learning techniques.

rss · Lobsters · Jun 23, 05:25

**标签**: `#game-ai`, `#game-development`, `#behavior-systems`, `#elden-ring`, `#game-design`

---

<a id="item-13"></a>
## [2026 年 WebAssembly 运行时性能基准测试对比](https://00f.net/2026/06/23/webassembly-runtimes-2026/) ⭐️ 7.0/10

截至 2026 年，一项全面对比各 WebAssembly 运行时性能的基准测试已发布，提供了不同运行时实现在当前条件下的最新性能数据。 该基准测试为开发者在项目中选择 WebAssembly 运行时实现提供了关键的实用数据，同时也反映了 Wasm 在无服务器计算、边缘计算和 AI 推理管道等超越浏览器原始场景中的日益重要性。 该基准测试评估了多种运行时实现，它们可能采用不同的编译策略，如提前编译（AOT）、即时编译（JIT）或解释执行，这些策略在不同使用场景下对性能特征有显著影响。

rss · Lobsters · Jun 23, 14:29

**背景**: WebAssembly（Wasm）最初被设计为 Web 的便携式编译目标，使代码能在浏览器内以接近原生的速度执行。到 2026 年，Wasm 已远超浏览器范畴，现在可在边缘计算、无服务器函数和 AI 推理管道中运行。Wasm 实现通常采用 AOT 或 JIT 编译，部分也使用解释器，目前已有许多面向通用用途的非浏览器运行时。WebAssembly 系统接口（WASI）和组件模型进一步扩展了 Wasm 在服务端和跨语言互操作方面的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>
<li><a href="https://www.devtoollab.com/blog/webassembly-guide">WebAssembly Explained: Complete Wasm & WASI Guide for ...</a></li>

</ul>
</details>

**标签**: `#webassembly`, `#performance`, `#benchmarks`, `#runtimes`

---

<a id="item-14"></a>
## [放缓节奏作为科技工程领域的战略优势](https://newsletter.pragmaticengineer.com/p/slow-down-to-speed-up) ⭐️ 7.0/10

Gergely Orosz 在 Pragmatic Engineer 通讯中分析了过去六个月里各科技公司的工程实践和工作方式发生的转变，并提出在当前行业环境下，有意放缓节奏是一种明智且具有战略意义的做法。 这篇分析之所以重要，是因为它挑战了科技行业长期以来以速度为先的执行文化，并为工程领导者和从业者提供了一个在宏观环境变化下重新思考生产力的框架——在这种环境下，效率和可持续性可能比单纯的速度更重要。 这篇文章具体调查了多家科技公司如何改变其工程工作流程和文化规范，指出行业从快速扩张转向更加审慎的执行方式，这不仅是暂时的反应，而可能是一种持久的战略重新校准。

rss · The Pragmatic Engineer · Jun 23, 15:30

**背景**: Gergely Orosz 是 The Pragmatic Engineer 的作者，这是软件工程领域阅读量最大的通讯之一，以对行业趋势、工程文化和科技公司运营的深入分析而闻名。过去几年中，科技行业经历了重大的宏观转变——包括裁员、预算削减以及从超高速增长时代的退出——这些变化迫使公司重新审视其工程工作方式和项目优先级。

**标签**: `#software-engineering`, `#industry-trends`, `#engineering-culture`, `#tech-strategy`

---