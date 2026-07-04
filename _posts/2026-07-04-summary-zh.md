---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> From 67 items, 21 important content pieces were selected

---

1. [新论文将市场竞争性与 P vs NP 问题联系起来](#item-1) ⭐️ 9.0/10
2. [GNU Guix 修复 substitute 与 pull 命令中的关键漏洞](#item-2) ⭐️ 9.0/10
3. [公民实验室确认欧洲议会议员设备感染飞马间谍软件](#item-3) ⭐️ 8.0/10
4. [Wordgard：ProseMirror 创作者推出的全新浏览器端富文本编辑器](#item-4) ⭐️ 8.0/10
5. [Ubicloud 主张使用严格内存过量分配以保护 PostgreSQL 免受 OOM Killer 影响](#item-5) ⭐️ 8.0/10
6. [HAT-4D 实现单目视频直出 4D 交互场景](#item-6) ⭐️ 8.0/10
7. [Current AI 发布开源 AI 差距地图 v0.1](#item-7) ⭐️ 8.0/10
8. [KDE Plasma 曝出任意代码执行漏洞，可突破应用沙箱](#item-8) ⭐️ 8.0/10
9. [深入剖析 Google Widevine L3 DRM 实现](#item-9) ⭐️ 8.0/10
10. [DJB 批评 IETF 的非混合 TLS-MLKEM 标准化方法](#item-10) ⭐️ 8.0/10
11. [HotSpot JIT 利用已知位分析优化按位掩码操作](#item-11) ⭐️ 8.0/10
12. [极简 Windows 内核在浏览器中运行，内存占用仅 4MB](#item-12) ⭐️ 8.0/10
13. [SearXNG：注重隐私的开源元搜索引擎在 AI 与 RAG 工作流中受到关注](#item-13) ⭐️ 7.0/10
14. [Jamesob 本地运行最先进大语言模型指南](#item-14) ⭐️ 7.0/10
15. [开发者探索替代性 LLM 工作流以保持编程心流](#item-15) ⭐️ 7.0/10
16. [Josh W. Comeau 报告 AI 导致课程销量大幅下滑](#item-16) ⭐️ 7.0/10
17. [Vercel 的 Andrew Qu 论为何 AI 代理是一种新型软件](#item-17) ⭐️ 7.0/10
18. [简化去中心化社交网络的 ActivityPub 实现](#item-18) ⭐️ 7.0/10
19. [ClickHouse 正在成为可观测性工作负载的首选数据库](#item-19) ⭐️ 7.0/10
20. [Gossamer：融合 Rust、Go 与 Swift 理念的全新编程语言](#item-20) ⭐️ 7.0/10
21. [Anthropic 推出面向科研人员的 Claude Science AI 工作台](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [新论文将市场竞争性与 P vs NP 问题联系起来](https://arxiv.org/abs/2602.20415) ⭐️ 9.0/10

一篇新的理论论文提出，金融市场具有竞争性当且仅当 P != NP，从而在数学上建立了市场效率与计算复杂性之间的等价关系。该研究在早期将弱式市场效率与 P = NP 条件相联系的工作基础上进行了重构与扩展。 这一发现架起了理论计算机科学与经济学之间的桥梁，表明计算的根本限制直接决定了市场效率的理论边界。如果该结论成立，则意味着在广泛接受的 P != NP 假设下，完全有效的市场在计算上是不可能实现的。 该论文专门探讨了市场竞争性与效率问题，提出了其与 P != NP 猜想之间的双向条件关系，而非单向推导。研究依赖于形式化的数学建模，将经济信息处理过程映射到计算复杂性类别中。

rss · Lobsters · Jul 3, 15:42

**背景**: P vs NP 问题探讨的是计算机能否快速求解所有可快速验证解的问题，这是计算机科学领域最重要的未解难题之一。有效市场假说（EMH）认为资产价格已充分反映所有可用信息，因此投资者无法持续战胜市场。此前的研究（尤其是 2010 年的一篇论文）曾指出，如果市场满足弱式有效，则 P 必须等于 NP，这意味着真正的市场效率要求瞬间解决计算上极其困难的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/P_versus_NP_problem">P versus NP problem - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/e/efficientmarkethypothesis.asp">investopedia.com/terms/e/efficientmarkethypothesis.asp</a></li>
<li><a href="https://arxiv.org/abs/1002.2284">[1002.2284] Markets are efficient if and only if P = NP</a></li>

</ul>
</details>

**社区讨论**: Lobsters 社区就该论文的假设以及对现实市场的数学建模展开了严谨的辩论。评论者们讨论了该证明的实际意义，部分人质疑理论上的计算限制是否能准确反映实际金融交易中充满启发式和不确定性的本质。

**标签**: `#computational-complexity`, `#economics`, `#theoretical-computer-science`, `#market-efficiency`, `#p-vs-np`

---

<a id="item-2"></a>
## [GNU Guix 修复 substitute 与 pull 命令中的关键漏洞](https://guix.gnu.org/en/blog/2026/guix-substitute-pull-vulnerabilities/) ⭐️ 9.0/10

GNU Guix 项目披露并修复了影响核心命令 'guix substitute' 和 'guix pull' 的安全漏洞，并敦促所有用户立即更新其安装。 这些漏洞对软件供应链安全构成严重威胁，因为攻击者可能利用它们在常规软件包更新和二进制文件下载过程中执行任意代码或破坏系统。 该安全公告特别针对用于获取预构建二进制文件和更新 Guix 工具链本身的机制，这意味着未打补丁的系统在每次与替代服务器交互或拉取新频道修订版时，仍面临被利用的风险。

rss · Lobsters · Jul 3, 06:45

**背景**: GNU Guix 是用于 GNU/Linux 系统的事务性包管理器，采用纯函数式部署模型，软件会被安装到通过加密哈希生成的唯一目录中。'guix substitute' 命令允许系统从授权服务器下载预构建的二进制文件，从而避免在本地编译所有内容，而 'guix pull' 则负责下载并部署最新的 Guix 源代码和软件包定义，以保持工具链处于最新状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://guix.gnu.org/">GNU Guix transactional package manager and distribution — GNU Guix</a></li>
<li><a href="https://guix.gnu.org/manual/en/html_node/Substitutes.html">Substitutes (GNU Guix Reference Manual)</a></li>
<li><a href="https://guix.gnu.org/manual/devel/en/html_node/Invoking-guix-pull.html">Invoking guix pull (GNU Guix Reference Manual)</a></li>

</ul>
</details>

**标签**: `#security`, `#guix`, `#package-manager`, `#supply-chain`, `#linux`

---

<a id="item-3"></a>
## [公民实验室确认欧洲议会议员设备感染飞马间谍软件](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

公民实验室通过取证分析确认，欧洲议会议员 Dimitrios Kouloglou 的 iPhone 于 2022 年 10 月及 2023 年 3 月多次成功感染飞马（Pegasus）间谍软件。该发现表明，此次攻击可能与针对欧洲境内流亡俄语及白俄罗斯语记者和活动人士的更广泛间谍活动有关。 此事件凸显了国家级数字间谍活动对高层民主机构构成的严重风险，并引发了关于欧盟内部跨境监控授权合法性的紧迫质疑。它强调了政府官员在处理敏感信息时实施严格的设备分离政策以及加强网络安全防护的必要性。 取证痕迹显示感染发生在 2022 年 10 月 21 日左右以及 2023 年 3 月 6 日至 7 日，可能导致机密政府文件和个人医疗数据同时泄露。此次攻击与过往行动的时间重叠表明，操作者拥有在多个欧洲司法管辖区部署间谍软件的授权。

hackernews · Lobsters · Jul 3, 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: 飞马（Pegasus）是由以色列 NSO Group 开发的高级间谍软件，能够通过无需用户交互的零点击漏洞感染设备。公民实验室是隶属于多伦多大学的跨学科研究机构，专注于数字间谍调查及以人权为核心的取证分析。零点击攻击通常利用 iMessage 等核心系统服务的漏洞，在目标设备上静默安装监控工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab - Wikipedia</a></li>
<li><a href="https://www.trendmicro.com/en_us/research/21/i/analyzing-pegasus-spywares-zero-click-iphone-exploit-forcedentry.html">Analyzing Pegasus Spyware's Zero-Click iPhone Exploit ForcedEntry ...</a></li>

</ul>
</details>

**社区讨论**: 评论者就攻击的地缘政治背景展开讨论，部分人提及希腊和波兰过往的间谍软件丑闻，并质疑究竟哪些实体拥有跨国监控授权。另一些人则批评欧洲议会似乎缺乏设备分离政策，指出在同一部手机上混合存储个人医疗数据与政府文件会带来巨大的安全风险。

**标签**: `#cybersecurity`, `#pegasus-spyware`, `#digital-espionage`, `#citizen-lab`, `#privacy`

---

<a id="item-4"></a>
## [Wordgard：ProseMirror 创作者推出的全新浏览器端富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

ProseMirror 的创作者发布了 Wordgard，这是一个用于构建结构化浏览器端富文本编辑器的全新开源 JavaScript 库。该框架允许开发者精确控制文档模式和内容类型，而不是作为一个自由格式的 HTML 编辑器运行。 Wordgard 通过提供严格的结构控制来解决现代文档编辑的复杂挑战，这对于需求已超出基础文本输入的团队至关重要。该版本的发布意义重大，因为它出自一位备受尊敬的领域专家之手，并为一个长期缺乏标准化 Web 解决方案的问题引入了全新的架构方法。 尽管 Wordgard 与 ProseMirror 共享核心概念，但两者之间没有直接的升级路径，这意味着迁移需要大量的重构工作。该系统强调结构化编辑模型，开发者可以精确定义支持的内容类型，从而避免传统 contentEditable 实现的不可预测性。

hackernews · indy · Jul 3, 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: Web 端的富文本编辑历来依赖浏览器原生的 contentEditable API，该 API 在不同平台上以不一致且难以控制而著称。ProseMirror 和 CodeMirror 等框架的创建旨在通过以编程方式管理文档状态并强制执行自定义模式来抽象这些复杂性。文档模式定义了编辑器内允许的结构和内容类型，从而确保数据完整性并支持协同编辑等功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wordgard.net/">Wordgard</a></li>
<li><a href="https://news.lavx.hu/article/wordgard-brings-structured-editing-to-javascript-apps">Wordgard brings structured editing to JavaScript apps | LavX News</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞了该项目的设计并认可其架构方法，但许多人指出缺乏从 ProseMirror 迁移的路径是一个重大障碍。开发者们还讨论了以编程方式与文档 JSON 进行交互的持续困难，并对几十年后 Web 端仍不存在标准化的所见即所得编辑实现表示沮丧。

**标签**: `#rich-text-editor`, `#web-development`, `#prosemirror`, `#javascript`, `#content-editing`

---

<a id="item-5"></a>
## [Ubicloud 主张使用严格内存过量分配以保护 PostgreSQL 免受 OOM Killer 影响](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 发布了一篇技术深度文章，解释了他们在 Linux 上强制执行严格内存过量分配（vm.overcommit_memory=2）的原因，以防止内存不足（OOM）杀手导致 PostgreSQL 集群不稳定。 该方法将内存分配失败从不可预测的集群级进程终止转变为即时、应用级的错误，从而显著提升了大规模数据库的可靠性和可预测性。 在严格过量分配模式下，内核会立即拒绝任何超出交换空间加上可配置物理内存百分比的分配请求并返回 ENOMEM 错误，而不是允许 OOM 杀手在随后终止关键进程。

hackernews · furkansahin · Jul 3, 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 默认采用启发式内存过量分配模式，允许进程分配超过实际物理内存的虚拟内存，系统假设这些进程不会同时使用所有分配的内存。当实际内存使用量超过可用资源时，内核会调用 OOM 杀手强制终止进程以回收内存。对于像 PostgreSQL 这样的有状态服务，主数据库进程被突然终止可能导致数据损坏、长时间停机以及集群范围内的级联故障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit">PostgreSQL and the OOM Killer: Why We Use Strict Memory Overcommit</a></li>
<li><a href="https://www.kernel.org/doc/Documentation/vm/overcommit-accounting">The Linux kernel supports the following overcommit handling modes</a></li>
<li><a href="https://utcc.utoronto.ca/~cks/space/blog/linux/StrictOvercommitProblem">Chris's Wiki :: blog/linux/StrictOvercommitProblem</a></li>

</ul>
</details>

**社区讨论**: 社区成员认可该方法，但强烈警告称，如果其他应用程序（如 Go 后端）激进地分配虚拟内存，严格过量分配可能导致系统级不稳定。Ubicloud 的作者承认标题语气较强，并指出虽然严格过量分配对托管 PostgreSQL 效果良好，但在混合工作负载环境中可能会产生意想不到的副作用。其他人则批评了 Linux 默认的虚拟内存行为不如 Windows 和 macOS，并强调在生产环境更改这些内核参数前必须进行彻底的 QA 和负载测试。

**标签**: `#PostgreSQL`, `#Linux`, `#Systems Engineering`, `#Memory Management`, `#Database Reliability`

---

<a id="item-6"></a>
## [HAT-4D 实现单目视频直出 4D 交互场景](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247901356&idx=3&sn=54ee94026f76691a380cd3ea214e0def) ⭐️ 8.0/10

上海交通大学的研究团队提出了 HAT-4D，这是一种能够直接从单目视频输入生成 4D 交互场景的新方法。该技术消除了传统上对昂贵的多相机动作捕捉摄影棚的依赖，简化了动态数字环境的创建流程。 通过摆脱对百万级动捕设施的依赖，HAT-4D 大幅降低了高保真 4D 内容创作的门槛。这一进展有望使游戏、虚拟现实和影视制作的工作流程更加普及，让小型团队仅凭普通视频素材就能制作复杂的交互场景。 该系统旨在从简单的视频片段（如刀切香蕉）中解析复杂的交互过程，同时捕捉物体几何形状与动态运动。与需要专用硬件和标记点跟踪的传统流程不同，HAT-4D 利用 AI 直接从单一视角重建空间与时间数据。

rss · 量子位 · Jul 3, 03:43

**背景**: 单目视频是指由单个摄像头拍摄的影像，通常缺乏立体或多机位设置所提供的深度信息。4D 场景生成在 3D 建模的基础上增加了时间维度，从而能够创建物体可真实移动和交互的动态环境。传统上，捕捉此类数据需要配备数十台同步红外摄像机和反光标记点的动捕摄影棚，导致成本高昂且大多数创作者难以企及。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://onevideooneworld.github.io/">OVOW: One Video , One World — Turning Monocular Video into...</a></li>
<li><a href="https://arxiv.org/html/2607.01202">World from Motion: Generative Dynamic Gaussian Reconstruction ...</a></li>

</ul>
</details>

**标签**: `#Computer Vision`, `#4D Scene Generation`, `#AI Research`, `#Motion Capture`, `#Monocular Video`

---

<a id="item-7"></a>
## [Current AI 发布开源 AI 差距地图 v0.1](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

获得 4 亿美元承诺资金支持的非营利组织 Current AI 发布了开源 AI 差距地图 v0.1，旨在全面梳理当前开源 AI 生态系统的现状。该初始版本深入分类了来自 228 个组织的 421 项关键产品，涵盖模型、数据集、软件工具和硬件项目。 该资源为开源 AI 领域提供了结构化、数据驱动的全景视图，帮助开发者、研究人员和政策制定者识别关键的基础设施缺口与机遇。通过在 MIT 许可下公开底层数据，Current AI 鼓励社区协作，共同构建更加透明且易于获取的 AI 技术公共选项。 该地图将 421 项精选成果按模型组件、产品/用户体验和基础设施三个层级划分为 14 个类别，同时指出还有超过 24,000 项未分类的长尾成果。底层数据集以 1,184 个 YAML 文件的形式托管在 GitHub 上，并附带处理脚本和架构，用户可通过 Datasette Lite 等工具浏览超过 16,000 个被追踪的代码库。

rss · Simon Willison · Jul 3, 22:04

**背景**: Current AI 于 2025 年 2 月在巴黎 AI 行动峰会上作为非营利组织成立，其使命是为人工智能构建公共选项。开源 AI 生态系统发展迅速但高度碎片化，使得利益相关者难以评估哪些基础组件已经成熟，以及哪些领域缺乏能够替代专有系统的稳健社区方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map | Simon Willison’s Weblog</a></li>
<li><a href="https://blog.jarv.tech/p/open-source-ai-gap-map-masshtabnaya-karta-ekosistemy-beea18396340c774">Open Source AI Gap Map : масштабная карта... — blog.jarv.tech</a></li>

</ul>
</details>

**标签**: `#open-source-ai`, `#ai-ecosystem`, `#ai-infrastructure`, `#ai-research`, `#community-resources`

---

<a id="item-8"></a>
## [KDE Plasma 曝出任意代码执行漏洞，可突破应用沙箱](https://blog.kimiblock.top/2026/07/01/arbitrary-code-execution-in-kde-plasma/) ⭐️ 8.0/10

开源开发者 Kimiblock 发布了一篇技术博文，详细披露了一个任意代码执行漏洞，攻击者可利用该漏洞突破 KDE Plasma 中的应用沙箱。该问题已上报给 KDE 上游开发团队，但在最新的 Plasma 6.7 版本中仍未得到修复。 该漏洞破坏了最广泛使用的 Linux 桌面环境之一的安全模型，可能导致恶意应用获取完整的系统访问权限。它凸显了 Linux 桌面沙箱技术面临的持续挑战，并引发了人们对厂商应对关键安全报告响应速度的担忧。 该漏洞专门针对 KDE Plasma 内部的沙箱机制，攻击者利用它可实现沙箱逃逸并在宿主系统上执行任意代码。尽管该漏洞已通过 KDE 官方安全邮箱渠道上报，但据称已被忽略，且依然存在于 Plasma 6.7 版本中。

rss · Lobsters · Jul 3, 02:39

**背景**: KDE Plasma 是一款广受欢迎的类 Unix 操作系统图形桌面环境，以其灵活性和丰富的功能集著称。应用沙箱是一种安全技术，用于隔离程序以防止其访问敏感系统资源或干扰其他进程。当存在沙箱逃逸漏洞时，恶意代码便可绕过这些隔离边界，并以宿主用户或系统的权限执行命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/KDE-Plasma-ACE-New-Window">KDE Plasma Affected By Arbitrary Code Execution To... - Phoronix</a></li>
<li><a href="https://en.wikipedia.org/wiki/KDE_Plasma">KDE Plasma - Wikipedia</a></li>
<li><a href="https://kde.org/plasma-desktop/">Plasma - KDE Community</a></li>

</ul>
</details>

**标签**: `#security`, `#kde-plasma`, `#sandbox-escape`, `#linux-desktop`, `#vulnerability-research`

---

<a id="item-9"></a>
## [深入剖析 Google Widevine L3 DRM 实现](https://neodyme.io/en/blog/widevine_l3) ⭐️ 8.0/10

Neodyme 发布了一篇详细的技术分析与逆向工程探索文章，深入剖析了 Google Widevine L3 DRM 实现的内部机制与安全局限。该文章逐步拆解了这一基于软件的保护层是如何运作的，以及其加密边界存在哪些弱点。 Widevine 是主流浏览器和 Android 设备上占主导地位的 DRM 系统，因此理解 L3 的弱点对于内容提供商和安全研究人员至关重要。该分析凸显了 L3 为何在本质上不如硬件支持的安全级别可靠，并进一步印证了行业对高级别内容强制要求更高安全层级的趋势。 Widevine L3 完全依赖主操作系统中的软件执行，因此与硬件隔离的 L1 和 L2 相比，更容易受到内存检查和密钥提取的攻击。研究人员此前已证明 L3 可被逆向工程以解密受保护的流媒体，这也是许多流媒体服务将 L3 客户端限制为仅支持标清播放的原因。

rss · Lobsters · Jul 3, 10:57

**背景**: Google Widevine 是一种专有的数字版权管理（DRM）技术，广泛用于保护浏览器、Android 和 iOS 平台上的流媒体内容。它分为三个安全级别：L1 和 L2 在基于硬件的可信执行环境（TEE）中执行加密操作，而 L3 则完全在软件中处理，缺乏硬件隔离。由于 L3 没有安全飞地保护，拥有系统级访问权限的攻击者可能截获解密密钥或篡改播放流程。内容分发商通常将 L3 作为旧设备或不支持硬件 DRM 设备的降级方案，并通常通过限制视频画质来降低盗版风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Widevine">Widevine - Wikipedia</a></li>
<li><a href="https://www.zdnet.com/article/security-researcher-cracks-googles-widevine-drm-l3-only/">Security researcher cracks Google's Widevine DRM ( L 3 only) | ZDNET</a></li>
<li><a href="https://www.gumlet.com/learn/widevine-drm/">How does Google's Widevine DRM protect your Videos?</a></li>

</ul>
</details>

**标签**: `#security`, `#reverse-engineering`, `#drm`, `#cryptography`, `#systems`

---

<a id="item-10"></a>
## [DJB 批评 IETF 的非混合 TLS-MLKEM 标准化方法](https://blog.cr.yp.to/20260702-standard.html) ⭐️ 8.0/10

著名密码学家 Daniel J. Bernstein 发表了一篇批判性分析，指出 IETF 正在通过标准化非混合 TLS-MLKEM 后量子密钥交换来逃避责任。他特别批评了围绕 draft-ietf-tls-mlkem 规范的命名惯例和程序性决策。 关于混合与非混合后量子密码学的争论直接影响互联网通信在向抗量子算法过渡期间的长期安全性。如果标准机构为了便利而牺牲密码学的稳健性，像 TLS 1.3 这样广泛部署的协议可能会继承日后难以修复的漏洞。 IETF 草案将 ML-KEM-512、ML-KEM-768 和 ML-KEM-1024 定义为 TLS 1.3 的独立命名组，而不是强制要求结合经典算法与后量子算法的混合结构。Bernstein 的批评强调了一个担忧，即解耦这些机制会将责任从标准机构转移到实现者身上。

rss · Lobsters · Jul 3, 13:38

**背景**: 后量子密码学（PQC）旨在保护通信免受未来能够破解当前公钥算法的量子计算机的威胁。由 NIST 标准化为 FIPS 203 的 ML-KEM 是一种为此目的设计的基于格的密钥封装机制。混合方法将 ML-KEM 与 ECDH 等传统算法结合使用，以便在新的后量子算法日后被发现存在缺陷时仍能保持安全性，而非混合方法则完全依赖于新算法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-ietf-tls-mlkem-00.html">ML - KEM Post-Quantum Key Agreement for TLS 1.3</a></li>
<li><a href="https://datatracker.ietf.org/doc/draft-ietf-tls-hybrid-design/">draft-ietf- tls - hybrid -design-16 - Hybrid key exchange in TLS 1.3</a></li>
<li><a href="https://ncse.info/post-quantum-cryptography/">Post - Quantum Cryptography : ML - KEM Implementation Guide</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#post-quantum`, `#ietf`, `#tls`, `#standards`

---

<a id="item-11"></a>
## [HotSpot JIT 利用已知位分析优化按位掩码操作](https://questdb.com/blog/jvm-jit-known-bits/) ⭐️ 8.0/10

QuestDB 发表了一篇技术深度文章，详细解释了 HotSpot JVM 的 JIT 编译器如何利用已知位分析来推理按位掩码操作。编译器通常能够确定某些位已经是固定的，从而在运行时完全消除冗余的掩码指令。 这项优化减少了 CPU 指令数量，并提升了大量使用按位逻辑的 Java 应用（如高性能数据库和系统软件）的执行吞吐量。它凸显了现代 JIT 编译器复杂的推理能力，展示了运行时分析如何实现静态编译器可能错过的优化。 已知位分析会追踪在不同代码路径中哪些位保证为零或一，从而使 JIT 能够证明掩码操作是多余的。该优化发生在 C2 编译器阶段，并依赖精确的数据流分析来安全地移除指令而不改变程序语义。

rss · Lobsters · Jul 3, 13:19

**背景**: HotSpot JVM 使用即时（JIT）编译器在程序执行期间将 Java 字节码动态转换为优化的本地机器码。它采用分层编译策略，其中 C1 编译器快速生成代码，而 C2 编译器则对频繁执行的方法进行重度优化。按位掩码是一种常见的底层操作，用于隔离或修改整数中的特定位，通常出现在对性能要求极高的系统编程中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.w3computing.com/articles/jvm-jit-compiler-deep-dive-c1-c2-tiered-compilation/">JVM JIT Compiler Deep Dive: C1, C2, and Tiered Compilation...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Just-in-time_compilation">Just -in- time compilation - Wikipedia</a></li>
<li><a href="https://www.ibm.com/docs/en/sdk-java-technology/8?topic=reference-jit-compiler">The JIT compiler</a></li>

</ul>
</details>

**标签**: `#JVM`, `#JIT Compilation`, `#Compiler Optimization`, `#Systems Engineering`, `#Java`

---

<a id="item-12"></a>
## [极简 Windows 内核在浏览器中运行，内存占用仅 4MB](https://www.msuiche.com/posts/nanokrnl-cold-boot-fast-boot/) ⭐️ 8.0/10

该系列技术文章的第一部分详细介绍了在浏览器标签页中直接运行极简 Windows 内核的实现过程。本篇重点探讨了冷启动与快速启动机制的工程实现，同时将内存占用严格控制在极小的 4MB 范围内。 在浏览器中成功启动 Windows 内核展示了基于 Web 的模拟技术和 WebAssembly 在处理复杂底层系统编程任务方面日益增长的能力。这项工作为系统工程师提供了关于极致内存优化和可移植内核开发的新见解，可能对未来调试、教学和轻量级虚拟化工具的发展产生影响。 该实现区分了传统的冷启动和类似休眠的快速启动模式，以便在严苛的资源限制下优化初始化速度。在 4MB 的限制内实现功能需要剥离非必要的驱动和服务，这凸显了将传统上庞大的操作系统核心适配到沙盒化浏览器环境中所面临的重大工程挑战。

rss · Lobsters · Jul 3, 20:03

**背景**: 现代 Windows 版本采用了一项名为快速启动（Fast Boot）的功能，该功能在关机时将内核会话保存到休眠文件中，从而相比完整的冷启动大幅缩短后续开机时间。WebAssembly 是一种二进制指令格式，允许浏览器运行原本用 C 或 Rust 等语言编写的高性能沙盒代码，使 x86 模拟器等复杂应用无需原生插件即可运行。在浏览器中运行操作系统内核通常需要将硬件调用转换为 Web 兼容的 API，并严格管理内存以避免导致宿主标签页崩溃。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reboot">Reboot - Wikipedia</a></li>
<li><a href="https://windowsforum.com/threads/disable-windows-fast-startup-pros-cons-and-how-to.383068/">Disable Windows Fast Startup: Pros, Cons, and... | Windows Forum</a></li>
<li><a href="https://dtptips.com/linux-in-the-browser-no-vm-no-cloud-just-webassembly-the-future-of-computing-has-begun/">Linux in the Browser : No VM, No Cloud, Just WebAssembly — The...</a></li>

</ul>
</details>

**标签**: `#systems-programming`, `#kernel-development`, `#webassembly`, `#emulation`, `#windows-internals`

---

<a id="item-13"></a>
## [SearXNG：注重隐私的开源元搜索引擎在 AI 与 RAG 工作流中受到关注](https://github.com/searxng/searxng) ⭐️ 7.0/10

社区正在热烈讨论 SearXNG，这是一个开源元搜索引擎，可聚合多达 280 个搜索服务的结果且不追踪用户，讨论重点涵盖了其在日常搜索、本地 AI 工具调用以及检索增强生成（RAG）管道中的实际应用。 随着隐私担忧加剧以及开发者为本地大语言模型寻找可控的数据源，SearXNG 提供了一个可自托管、无追踪的搜索层，有效弥合了隐私浏览与现代 AI 智能体工作流之间的鸿沟。 用户指出，虽然 SearXNG 提供了强大的隐私保护和用于 RAG 的 JSON 输出支持，但其速度可能慢于商业引擎，偶尔会触发上游提供商的验证码，并且借助 TinySearch 等封装工具可以优化 AI 智能体的上下文 token 使用。

hackernews · theanonymousone · Jul 3, 20:15 · [社区讨论](https://news.ycombinator.com/item?id=48779454)

**背景**: 元搜索引擎不维护自己的索引，而是将用户查询转发给多个第三方搜索提供商并聚合结果，这有助于避免单一提供商获取完整的用户身份。检索增强生成（RAG）是一种 AI 技术，语言模型在生成回答前会先获取相关的外部信息，从而显著减少幻觉并保持输出内容的时效性。自托管此类工具使个人和组织能够完全掌控其查询数据和基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SearXNG">SearXNG - Wikipedia</a></li>
<li><a href="https://docs.searxng.org/">SearXNG Documentation (2026.7.3+21773bbb2)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对隐私保护和自托管能力普遍持积极态度，但用户也承认存在速度较慢和偶尔被上游引擎验证码拦截等权衡取舍。Searx 的原始创建者指出了元搜索概念的局限性并分享了一个新的本地索引项目，而其他开发者则强调了其与本地大语言模型的成功集成以及用于 AI 智能体的 token 优化封装工具。

**标签**: `#open-source`, `#search-engines`, `#privacy`, `#AI-agents`, `#RAG`

---

<a id="item-14"></a>
## [Jamesob 本地运行最先进大语言模型指南](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

jamesob 在 GitHub 上发布了一份详尽指南，介绍如何在本地硬件上部署最先进的大语言模型，涵盖从消费级设备到高端多 GPU 配置的多种方案。该指南的发布引发了社区关于本地推理与云端方案在成本、性能权衡及经济可行性方面的广泛讨论。 随着 AI 模型能力的提升，本地运行不仅能增强数据隐私保护，还能避免持续的 API 费用，但这需要高昂的硬件投入和技术门槛。该指南及随之而来的辩论凸显了爱好者愿景与在本地匹配顶级云端模型性能的经济现实之间的巨大差距。 指南中提议的高端本地配置在计入多张企业级 GPU 后成本可能超过 5 万美元，而更易入手的方案通常依赖提供 48GB 显存的双 RTX 3090 显卡。为了将庞大模型塞入有限内存，用户必须采用降低数值精度的量化技术，社区成员警告这可能会削弱推理质量或导致模型陷入循环。

hackernews · livestyle · Jul 3, 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 本地大语言模型推理是指直接在个人设备或本地服务器上运行模型，而非依赖远程云端 API，这能保护敏感数据隐私，但对显存（VRAM）有极高要求。量化是一种关键的模型压缩技术，通过降低网络权重和激活值的数值精度来大幅缩小模型体积并减少计算需求，但可能会牺牲一定的准确性。Ollama 和 LM Studio 等工具简化了软件栈，使得拥有现代 GPU 的开发者和爱好者能够越来越轻松地实现本地部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://michielh.medium.com/llm-quantization-techniques-balancing-performance-and-efficiency-bc348eed3816">LLM Quantization Techniques : Balancing Performance and... | Medium</a></li>
<li><a href="https://fungies.io/local-llm-inference-tools-guide-2026-3/">How to Set Up and Use Local LLM Inference Tools in... - Fungies.io</a></li>
<li><a href="https://homelabstarter.com/homelab-local-ai-gpu-setup/">Running Local AI in Your Homelab: GPU Setup... — HomeLab Starter</a></li>

</ul>
</details>

**社区讨论**: 社区对该指南的成本估算持高度怀疑态度，用户指出所谓 4 万美元的配置实际花费超过 5 万美元，且仍无法匹敌 Claude Opus 等顶级云端模型。评论者强调，重度量化和专家剪枝会严重削弱模型的推理能力，因此许多人认为订阅云端服务在经济性和可靠性上仍远胜于构建昂贵的本地设备。

**标签**: `#LLMs`, `#Local Inference`, `#Hardware`, `#Quantization`, `#MLOps`

---

<a id="item-15"></a>
## [开发者探索替代性 LLM 工作流以保持编程心流](https://news.ycombinator.com/item?id=48771515) ⭐️ 7.0/10

Hacker News 上的一场讨论突显了开发者们正在尝试非传统的 LLM 交互模型，例如密闭代理（hermetic agents）和异构 LLM 集群，以克服标准提示-响应循环导致的心流中断问题。原帖作者和社区成员正在积极寻找并分享替代工作流，试图摆脱 Claude Code 和 Codex 等工具带来的“停顿-等待”模式。 保持深度心流状态对于开发者的生产力和工作满意度至关重要，而当前的 AI 编程助手往往因频繁的上下文切换需求打断这种认知节奏。找到更无缝的集成模式可能会从根本上重塑软件工程师与 AI 的协作方式，使这些工具从干扰性的审查者转变为真正隐形的加速器。 提出的实验性方法包括使用沙盒化的“密闭代理”，让它们根据同一规范独立生成代码和测试以避免确认偏差，以及在分布式硬件上编排异构 LLM 集群。其他建议还包括将交互范式转向“标签页模型”，或通过移动界面采用“步行编程”，以便在等待 AI 输出时保持精神专注。

hackernews · yehiaabdelm · Jul 3, 06:21

**背景**: Anthropic 的 Claude 和 OpenAI 的 Codex 等大型语言模型（LLMs）已在软件开发中普及，通常通过对话式的提示-响应界面运行。虽然这些工具显著加速了样板代码生成和调试，但提示、等待和审查的迭代循环迫使开发者不断在创造性编程和分析性评估之间切换。这种认知摩擦与传统的“心流状态”形成鲜明对比，后者是一种深度沉浸的心理状态，程序员可以在其中不受干扰地连续工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>
<li><a href="https://www.promptingguide.ai/research/llm-agents">LLM Agents | Prompt Engineering Guide</a></li>

</ul>
</details>

**社区讨论**: 社区情绪强烈认同原帖作者的挫败感，许多人一致认为当前的 AI 工具分散了注意力而非增强专注力。评论者分享了多种变通方案，从基于代理图执行引擎的技术架构到徒步旅行中“步行编程”的生活方式调整，还有人幽默地指出，新的心流状态只不过是在不同工作树之间管理多个终端标签页罢了。

**标签**: `#LLMs`, `#Software Engineering`, `#Developer Tools`, `#AI Coding Assistants`, `#Workflow Optimization`

---

<a id="item-16"></a>
## [Josh W. Comeau 报告 AI 导致课程销量大幅下滑](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

知名开发者教育者 Josh W. Comeau 报告称，其最新课程的销量仅为往常的三分之一左右，现有课程的销售额也出现显著下滑。他将这一低迷归因于更广泛的行业趋势，即多位课程创作者的收入降幅已超过 50%。 这凸显了开发者教育市场的结构性转变，因为 AI 带来的就业不确定性降低了学习者的投入意愿，同时 LLM 正成为付费内容的免费个性化替代品。这一趋势预示着独立教育者可能面临经济冲击，并引发了关于生成式 AI 时代内容补偿与可持续性的紧迫问题。 Comeau 指出了一种“双重打击”效应：潜在学员因担心开发者岗位可能消失而不愿投资技能学习，而那些确实想学习的人则越来越依赖 LLM 进行辅导。他还指出，这些模型在未经同意或补偿的情况下抓取创作者的作品，直接破坏了他们的商业模式。

rss · Simon Willison · Jul 3, 21:25

**背景**: Josh W. Comeau 是一位知名的 Web 开发者和教育者，以其关于 CSS 和 React 的高质量交互式课程而闻名。大型语言模型（LLM）是基于海量文本训练的 AI 系统，能够生成代码、解答技术问题并充当按需辅导工具。生成式 AI 的兴起引发了关于其对软件工程职业影响以及传统教育内容价值的广泛讨论。

**标签**: `#AI Impact`, `#Developer Education`, `#EdTech`, `#LLMs`, `#Industry Trends`

---

<a id="item-17"></a>
## [Vercel 的 Andrew Qu 论为何 AI 代理是一种新型软件](https://www.latent.space/p/vercel-agents-new-software) ⭐️ 7.0/10

Vercel 软件负责人 Andrew Qu 详细介绍了 'eve' 代理框架的创建过程，并概述了 AI 驱动软件的新架构范式。他认为，下一代应用必须围绕模块化技能、安全执行沙箱以及代理可读网站来构建。 这一观点标志着 Web 开发正从以人为中心的界面向机器可导航的生态系统发生根本性转变，将直接影响开发者构建和部署应用的方式。作为主要的基础设施提供商，Vercel 对该模式的认可很可能会加速行业对标准化代理工作流和安全实践的采用。 'eve' 框架是一个采用 Apache-2.0 许可的开源 TypeScript 工具，其中每个代理都表示为一个包含 Markdown 指令和 TypeScript 工具的文件系统目录。该框架会将这些文件编译成清单，并在 Vercel Functions 上提供持久化运行时，强调项目的可检查性和可扩展性。

rss · Latent Space · Jul 3, 00:08

**背景**: AI 代理是利用大语言模型来规划和执行多步骤任务的自主程序，但它们需要被称为沙箱的安全环境来运行生成的代码，以免危及主机系统。此外，代理可读网站提供结构化的元数据和明确的指令，使 AI 爬虫能够比传统仅面向人类浏览器设计的 HTML 更有效地理解网站架构和内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vercel.com/eve">eve – The Agent Framework - Vercel</a></li>
<li><a href="https://github.com/vercel/eve">GitHub - vercel / eve : The Framework for Building Agents · GitHub</a></li>
<li><a href="https://www.digitalapplied.com/blog/vercel-eve-open-source-typescript-agent-framework-launch">Vercel eve : Open-Source TypeScript Agent Framework</a></li>
<li><a href="https://vercel.com/kb/guide/agent-readability-spec">Agent Readability : A Specification for AI-Optimized Websites</a></li>
<li><a href="https://northflank.com/blog/how-to-sandbox-ai-agents">How to sandbox AI agents in 2026: MicroVMs, gVisor... — Northflank</a></li>

</ul>
</details>

**标签**: `#AI Agents`, `#Software Architecture`, `#Vercel`, `#Web Development`, `#LLM Infrastructure`

---

<a id="item-18"></a>
## [简化去中心化社交网络的 ActivityPub 实现](https://hackers.pub/@fedify/2026/why-activitypub-is-hard) ⭐️ 7.0/10

一篇新的技术文章深入分析了开发者在实现 ActivityPub 协议时面临的具体工程障碍，并提出了简化开发流程的实用方法。 降低实现 ActivityPub 的技术门槛对于扩展 Fediverse 生态系统至关重要，因为它使更多开发者能够构建可互操作的去中心化应用，而无需重复发明复杂的基础设施。 文章重点指出了具体的痛点，包括碎片化的加密签名标准、不可预测的 JSON-LD 文档变体、复杂的分布式系统工程要求以及阻碍协议采用的关键安全漏洞。

rss · Lobsters · Jul 3, 13:37

**背景**: ActivityPub 是一项 W3C 标准的去中心化社交网络协议，为包括 Mastodon 和 Pixelfed 在内的 Fediverse 平台提供支持。它采用带有 HTTP 方法和共享收件箱的 RESTful API 设计，使不同的服务器能够相互通信并交换数据。然而，由于该规范允许极大的灵活性，不同平台在实现功能时往往不一致，从而导致整个网络面临互操作性和服务发现的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hackers.pub/@fedify/2026/why-activitypub-is-hard">Fedify: Why implementing ActivityPub is hard, and why it doesn't have to be</a></li>
<li><a href="https://en.wikipedia.org/wiki/ActivityPub">ActivityPub - Wikipedia</a></li>
<li><a href="https://dasroot.net/posts/2026/04/activitypub-fediverse-decentralized-social-networking/">ActivityPub Protocol: Understanding the Fediverse · Technical news about AI, coding and all</a></li>

</ul>
</details>

**标签**: `#ActivityPub`, `#Decentralization`, `#Fediverse`, `#Protocol Design`, `#Web Standards`

---

<a id="item-19"></a>
## [ClickHouse 正在成为可观测性工作负载的首选数据库](https://matduggan.com/clickhouse-is-winning-the-observability-wars/) ⭐️ 7.0/10

一篇最新的行业分析指出，ClickHouse 正迅速成为可观测性工作负载的主导数据库，超越了传统的时间序列和日志管理方案。该文章强调，其卓越的性能、成本效益以及在现代基础设施栈中日益广泛的采用是推动这一转变的关键因素。 这一趋势标志着工程团队处理日志、指标和追踪数据的架构发生了重大转变，正从专用的传统工具转向统一的高性能分析型数据库。随着可观测性数据量的激增，采用像 ClickHouse 这样兼具成本效益和可扩展性的后端，能够显著降低基础设施成本，同时提升故障排查时的查询速度。 ClickHouse 的列式 OLAP 架构能够在海量数据集上实现极高的写入吞吐量和快速分析查询，非常适合基于时间的读取和仪表板数据聚合。然而，要有效利用它，必须在前期对数据分区、索引策略和查询模式进行周密设计，以避免在生产环境中出现性能瓶颈。

rss · Lobsters · Jul 3, 05:25

**背景**: 可观测性是指在整个 IT 生态系统中收集和分析日志、指标与追踪数据，以定位系统问题根本原因的实践。传统上，团队依赖专用的时间序列数据库或日志聚合器，但随着数据量增长，这些方案往往面临扩展成本高昂和查询延迟的问题。像 ClickHouse 这样的列式数据库按列而非按行存储数据，能够大幅压缩数据并加速分析查询，因此越来越受到实时分析和大规模监控工作负载的青睐。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.elastic.co/what-is/observability">What is Observability ? | A Comprehensive Observability ... | Elastic</a></li>
<li><a href="https://realworld.cloud/clickhouse-vs-traditional-time-series-databases-for-iot-when">ClickHouse vs . Traditional Time ‑ Series Databases for IoT: When to...</a></li>
<li><a href="https://www.iplocation.net/blog/architectural-solutions-for-scalable-systems-with-clickhouse">Architectural Solutions for Scalable Systems with ClickHouse</a></li>

</ul>
</details>

**标签**: `#observability`, `#clickhouse`, `#databases`, `#infrastructure`, `#data-engineering`

---

<a id="item-20"></a>
## [Gossamer：融合 Rust、Go 与 Swift 理念的全新编程语言](https://gossamer-lang.org/) ⭐️ 7.0/10

Gossamer 是一款新推出的编程语言，它结合了类 Rust 的语法、Go 风格的 goroutine 以及受 Swift 启发的内存模型。该项目目前已在 GitHub 上开源，其官方文档强调了快速编译和对 WebAssembly 的支持。 通过融合三种备受推崇的语言范式，Gossamer 试图解决开发者体验、安全并发与可预测内存管理之间的经典权衡问题。如果取得成功，它将为系统程序员提供一种极具吸引力的替代方案，在保持高性能的同时减少样板代码。 该语言采用受 Swift ARC 启发的自动且无暂停的内存管理机制，从而避免了传统垃圾回收带来的停顿。它还支持初始化栈空间极小的轻量级 goroutine 并发模型，并能高效编译为 WebAssembly 目标代码。

rss · Lobsters · Jul 3, 15:32

**背景**: Rust 以其严格的借用检查器闻名，能够在编译期保证内存安全，而 Go 则通过 goroutine 普及了由运行时管理的轻量级线程，实现了轻松的并发编程。Swift 使用自动引用计数（ARC）来确定性管理内存，无需依赖追踪式垃圾回收器。Gossamer 试图综合这些方法，提供熟悉的语法、内置的轻量级并发以及无暂停的自动内存处理机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/danpozmanter/gossamer">danpozmanter/ gossamer : The Gossamer programming language ...</a></li>
<li><a href="https://gossamer-lang.org/docs/wasm/">WebAssembly - Gossamer</a></li>
<li><a href="https://codeclaritylab.com/glossary/goroutine_concept">Goroutine - Style Concurrency — Code Glossary | CodeClarityLab</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#rust`, `#concurrency`, `#memory-management`, `#systems-programming`

---

<a id="item-21"></a>
## [Anthropic 推出面向科研人员的 Claude Science AI 工作台](https://www.theverge.com/ai-artificial-intelligence/961311/anthropic-claude-science-ai-drug-development) ⭐️ 7.0/10

Anthropic 发布了 Claude Science，这是一款全新的 AI 工作台，旨在将分散的科学工具和数据集整合到统一的环境中供研究人员使用。该平台还具备自动生成图表和可视化内容的功能，以简化科研工作流。 此次发布标志着一家头部 AI 实验室战略性地进军生命科学和药物发现领域，这些领域被视为检验人工智能能力的严苛试金石。通过集中复杂的科研工具，Anthropic 旨在加速科学突破，并减少当前数据密集型研发流程中固有的阻力。 Claude Science 专门针对计算密集型的科学分析进行了优化，并能生成可审计的产物以确保研究的透明度。然而，它并非为所有科研工作流设计的通用解决方案，将其应用于不匹配的任务可能会导致操作上的摩擦。

rss · The Verge · Jul 3, 13:56

**背景**: AI for Science 指的是应用人工智能来加速生物学、化学和物理学等领域的发现。在药物发现过程中，研究人员传统上需要同时操作大量互不相连的软件包和海量数据集，以筛选出可行的候选药物。AI 工作台试图通过整合这些工具并利用大语言模型辅助数据分析、分子建模和实验规划，来解决这种碎片化问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-science-ai-workbench">Claude Science , an AI workbench for scientists \ Anthropic</a></li>
<li><a href="https://paperguide.ai/blog/how-to-use-claude-science/">How to Use Claude Science for Scientific Research in 2026</a></li>
<li><a href="https://www.linkedin.com/pulse/ai-drug-discovery-one-size-fits-all-addressing-data-challenges-yby9e">AI Drug Discovery : Not One-Size-Fits-All – Addressing Data Challenges</a></li>

</ul>
</details>

**标签**: `#AI for Science`, `#Drug Discovery`, `#Anthropic`, `#Claude`, `#Research Tools`

---