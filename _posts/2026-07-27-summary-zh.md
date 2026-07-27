---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> From 38 items, 10 important content pieces were selected

---

1. [地下中继市场利用 AI Token 转售和云计费欺诈牟利](#item-1) ⭐️ 7.0/10
2. [GrapheneOS 详解针对锁屏设备数据提取的防护措施](#item-2) ⭐️ 7.0/10
3. [欧盟委员会提议通过浏览器级隐私偏好设置消除 Cookie 横幅](#item-3) ⭐️ 7.0/10
4. [It's not empowering to hand off the details](#item-4) ⭐️ 7.0/10
5. [MonkeyOCRv2 以 0.7B 模型登顶开源文档解析](#item-5) ⭐️ 7.0/10
6. [Xavier Leroy 探讨编程语言与形式化验证](#item-6) ⭐️ 7.0/10
7. [《Let Over Lambda》深入探讨 Forth 与 Lisp 编程范式的交融](#item-7) ⭐️ 7.0/10
8. [Lean 在 DEFLATE 压缩基准测试中超越 Rust](#item-8) ⭐️ 7.0/10
9. [探索 Valkey 内部数据生命周期](#item-9) ⭐️ 7.0/10
10. [美国公民因在边境使用胁迫密码擦除手机数据被起诉](#item-10) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [地下中继市场利用 AI Token 转售和云计费欺诈牟利](https://vectoral.com/blog/token-relay-market) ⭐️ 7.0/10

一项详细调查揭示了一个活跃的地下市场，不法分子通过滥用云服务商计费系统、利用免费额度和被盗账户来转售打折的 AI 推理 Token。转售者通过共享账户和支付欺诈等手段，以低于官方 API 价格 70%至 90%的折扣提供 Claude 等模型。 这暴露了 AI 和云定价模型中的系统性漏洞，订阅制和免费层服务为复杂的欺诈者创造了利润丰厚的套利机会。它威胁到 AI 提供商的经济可持续性，并对按全价购买推理服务的合法企业造成不公平竞争。 转售者至少通过三种方式运作：使用被盗或伪造信用卡、滥用 AWS 和 Azure 面向新公司的免费额度，以及共享 Claude Max 等高级订阅账户。据报道，一些买家仅以实际成本 4%的价格获得推理服务，在计算密集型业务中获得了巨大的竞争优势。

hackernews · mlenhard · Jul 26, 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49058993)

**背景**: AI 推理 Token 是 Anthropic、OpenAI 和 Google 等提供商在开发者通过 API 使用其模型时收取的计算单位。AWS、Azure 和 Google Cloud 等云服务商向新公司提供免费额度以鼓励采用，但这些额度可通过创建多个空壳公司大规模滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/ai-token-black-market-claude-resellers-distillation-2026">AI Token Black Market: Claude Resellers at 70–93% Off ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48667495">Here's what is happening: Chinese resellers are offering Claude tokens at 70-90%... | Hacker News</a></li>
<li><a href="https://elevenlab.net/token-relay-station-ai-model-reseller-business/">Token Relay Stations: 5 Brutal Truths About AI 's Most Dangerous...</a></li>

</ul>
</details>

**社区讨论**: 评论者将其与广告技术欺诈和黄牛倒票相类比，指出这是已知模式在新领域的应用。多人强调订阅模式本质上会创造套利机会，而免费云额度使不法分子能以极低成本获取推理服务。讨论认为，如果不从根本上重新思考 AI 计算的定价和访问控制方式，就很难防止此类滥用。

**标签**: `#AI-infrastructure`, `#cloud-security`, `#fraud-detection`, `#token-economics`, `#cloud-abuse`

---

<a id="item-2"></a>
## [GrapheneOS 详解针对锁屏设备数据提取的防护措施](https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices) ⭐️ 7.0/10

GrapheneOS 发布了详细文档，介绍其针对锁屏设备数据提取的防御措施，包括自动重启功能使设备回到首次解锁前（BFU）模式，以及防止密钥提取的强加密机制。该文档澄清了即使没有胁迫密码，该系统也能为用户抵御取证工具提供强有力的保护。 这对于在边境或法律程序中面临设备被扣押风险的记者、活动人士和注重隐私的用户意义重大，因为它证明了 GrapheneOS 即使硬件落入对手手中也能保护敏感数据。它为移动安全设立了超越原生 Android 和 iOS 的更高标准。 自动重启计时器会在可配置的时间段（例如 18 小时）后强制设备回到 BFU 模式，确保加密密钥从内存中清除，数据恢复到完全加密的静态存储状态。据报道，自 2022 年中期的补丁以来，Cellebrite Premium 一直无法利用 GrapheneOS 设备的漏洞，而自动重启功能则作为对未来未知漏洞利用的防御手段。

hackernews · Cider9986 · Jul 26, 05:57 · [社区讨论](https://news.ycombinator.com/item?id=49055169)

**背景**: 首次解锁前（BFU）是指设备重启后加密密钥尚未加载到内存中的状态，与首次解锁后（AFU）状态相比，数据提取难度大幅增加。Android Keystore 通过确保密钥材料永远不会进入应用程序进程来提供防提取保护，而 GrapheneOS 在此基础上进行了额外的安全加固。Cellebrite 等取证工具利用运行中操作系统的漏洞来绕过锁屏并从设备中提取数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grapheneos.org/features">Features overview | GrapheneOS</a></li>
<li><a href="https://grapheneos.social/@GrapheneOS/110664343914579123">GrapheneOS: "GrapheneOS includes our auto-r…" - GrapheneOS Mastodon</a></li>
<li><a href="https://www.reddit.com/r/GrapheneOS/comments/1nbwn9h/how_can_gos_protect_me_from_governments_unlocking/">How can GOS protect me from governments unlocking my phone? : r/GrapheneOS</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞了 GrapheneOS 在实际应用中的有效性，引用了其 18 小时自动重启功能帮助记者保护机密消息来源的案例。然而，用户指出了一个明显的不足：缺乏完整的备份和恢复解决方案，无法在过境前进行预防性擦除。其他人则讨论了 Android 图案锁的熵值局限性，并将其与 Apple 类似的自动重启和锁定模式功能进行了比较。

**标签**: `#mobile-security`, `#grapheneos`, `#encryption`, `#privacy`, `#android-security`

---

<a id="item-3"></a>
## [欧盟委员会提议通过浏览器级隐私偏好设置消除 Cookie 横幅](https://killthecookiebanner.eu/) ⭐️ 7.0/10

欧盟委员会提出了一项改革方案，允许用户在浏览器或操作系统层面一次性设置隐私和 Cookie 同意偏好，该设置将自动向网站发送信号，从而消除重复出现的 Cookie 同意横幅。这一变化是一项更广泛的数字简化计划的一部分，旨在减轻合规负担，同时长期尊重用户的隐私选择。 如果该改革获得通过，它将从根本上改变欧洲网络的隐私同意机制，终结自 ePrivacy 指令和 GDPR 生效以来一直困扰用户的 Cookie 横幅疲劳问题。它还为全球浏览器级同意信号树立了先例，与加利福尼亚州即将于 2027 年实施的浏览器隐私控制等类似方案保持一致。 该提案包含一项针对媒体机构的争议性豁免条款，理由是媒体依赖广告收入，这引发了重大的政治争论。网站将自动读取浏览器的同意信号并调整跟踪行为，无需显示任何横幅，但这些信号的技术实施标准仍有待定义。

hackernews · rapnie · Jul 26, 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49057175)

**背景**: ePrivacy 指令（通常被称为

**标签**: `#privacy`, `#EU-regulation`, `#web-standards`, `#cookie-consent`, `#browser-policy`

---

<a id="item-4"></a>
## [It's not empowering to hand off the details](https://davidnicholaswilliams.com/its-not-empowering-to-hand-off-the-details/) ⭐️ 7.0/10

An essay arguing that delegating details to others (or AI) isn't truly empowering, sparking a rich community debate about verification vs. understanding, AI-assisted coding fatigue, and the evolving role of developer judgment.

hackernews · davnicwil · Jul 26, 17:58 · [社区讨论](https://news.ycombinator.com/item?id=49060592)

**标签**: `#AI-assisted-development`, `#software-engineering-culture`, `#developer-empowerment`, `#code-review`, `#vibecoding`

---

<a id="item-5"></a>
## [MonkeyOCRv2 以 0.7B 模型登顶开源文档解析](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&mid=2247907283&idx=2&sn=5df8a52712c79f67232ca9672d4cc34e) ⭐️ 7.0/10

华中科技大学与金山办公的研究团队发布了 MonkeyOCRv2，这是一个仅 0.7B 参数的文档解析模型，在 MDPBench 基准测试中取得了覆盖 17 种语言的开源最优性能。该项目包括训练数据（MonkeyDoc v2）和模型权重，已在 Apache-2.0 许可证下完全开源。 MonkeyOCRv2 挑战了模型规模不断扩大的主流趋势，证明高度专业化的小型模型在文档解析任务中可以超越大得多的模型。这一突破有望显著降低部署成本，并推动多语言企业环境中的端侧文档 AI 应用。 该模型采用文档原生视觉骨干网络搭配轻量级语言模型，并在大规模多语言语料库上使用双重预训练策略。其核心架构理念强调参数专业化——每个参数都必须有明确的职责分工——而非简单地增加模型容量。

rss · 量子位 · Jul 26, 04:30

**背景**: 文档解析（Document AI）涉及从数字或拍照文档中提取文本、表格和版面等结构化信息，对企业工作流至关重要。传统 OCR 流水线通常需要多个专用模型协同工作，而新兴的视觉语言模型（VLM）试图将其统一为单一架构。近期行业趋势倾向于使用越来越大的模型（3B 以上参数）以获得更高精度，但这带来了计算和部署方面的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/yuliang-liu/monkeyocr">GitHub - Yuliang-Liu/MonkeyOCR: A lightweight LMM-based Document Parsing Model · GitHub</a></li>
<li><a href="https://arxiv.org/abs/2607.11562">[2607.11562] MonkeyOCRv2: A Visual-Text Foundation Model for Document AI</a></li>
<li><a href="https://www.alphaxiv.org/overview/2607.11562">MonkeyOCRv2: A Visual-Text Foundation Model for Document AI | alphaXiv</a></li>

</ul>
</details>

**标签**: `#OCR`, `#document-parsing`, `#small-language-models`, `#open-source`, `#multilingual-AI`

---

<a id="item-6"></a>
## [Xavier Leroy 探讨编程语言与形式化验证](https://www.youtube.com/watch?v=9Cswiqrq6So) ⭐️ 7.0/10

一段新的 YouTube 视频邀请了 OCaml 和 CompCert 验证 C 编译器的主要创建者 Xavier Leroy，探讨编程语言设计和形式化验证方法论。该访谈涵盖了他在构建高可信软件系统方面的数十年经验。 Xavier Leroy 是编程语言和形式化方法领域最具影响力的人物之一，在业界探索利用 AI 使形式化验证走向主流的背景下，他的见解尤为重要。他在 CompCert 上的工作证明了形式化验证编译器在安全和关键任务软件中的实用性。 CompCert 是一个经过形式化验证的优化 C 编译器，支持大部分 ISO C99/C11 标准，可为 ARM、PowerPC、RISC-V 和 x86 处理器生成高效代码。Leroy 担任 OCaml 系统的主要开发者已超过 30 年，目前是法兰西公学院的软件科学教授。

rss · Lobsters · Jul 26, 14:59

**背景**: 形式化验证是利用数学证明来验证程序或系统是否完全按照规范运行的过程，能够消除传统测试可能遗漏的整类缺陷。OCaml 是一种广泛应用于学术界和工业界的函数式编程语言，尤其用于编译器开发和形式化方法研究。CompCert 是一个里程碑式的项目，证明了生产级编译器可以进行形式化验证，这意味着其编译过程在数学上被保证不会引入错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Xavier_Leroy">Xavier Leroy - Wikipedia</a></li>
<li><a href="https://compcert.org/">CompCert - Main page</a></li>
<li><a href="https://en.wikipedia.org/wiki/CompCert">CompCert - Wikipedia</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#formal-verification`, `#OCaml`, `#interview`, `#CompCert`

---

<a id="item-7"></a>
## [《Let Over Lambda》深入探讨 Forth 与 Lisp 编程范式的交融](https://letoverlambda.com/textmode.cl/guest/chap8.html) ⭐️ 7.0/10

高级 Lisp 编程书籍《Let Over Lambda》中题为'Forth Moving Lisp Moving Forth'的一章因其对 Forth 和 Lisp 编程范式关系的深入探索而受到关注。该章节探讨了这两种具有不同设计哲学的历史重要语言如何相互启发和影响。 这种跨范式分析对编程语言爱好者和关注语言设计的系统程序员具有重要价值，因为它揭示了 Forth 基于栈的元编程与 Lisp 基于宏的代码生成之间的对比。理解这些交叉点可以激发构建领域特定语言和可扩展系统的新方法。 该章节出自以深入讲解 Common Lisp 宏（即编写程序的程序）而闻名的《Let Over Lambda》一书。它对比了 Forth 通过词拼接和栈操作来扩展语言的方式，与 Lisp 在编译时提供完整语言访问能力的宏系统。

rss · Lobsters · Jul 26, 17:39

**背景**: Forth 是 Charles H. Moore 于 1970 年创建的面向栈的编程语言，以其简洁性和通过扩展语言本身来构建应用程序的范式而闻名。Lisp 最初于 20 世纪 50 年代末定义，是目前仍在广泛使用的第二古老的高级编程语言，以其完全括号化的前缀表示法和强大的宏系统而著称。《Let Over Lambda》是 Doug Hoyte 撰写的一本高级 Common Lisp 书籍，广泛专注于宏和元编程技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forth_(programming_language)">Forth (programming language) - Wikipedia</a></li>
<li><a href="https://letoverlambda.com/">Let Over Lambda</a></li>
<li><a href="https://www.tutorialpedia.org/blog/comparison-of-common-lisp-macros-and-forth-metaprogramming-capabilities/">Common Lisp Macros vs . Forth Metaprogramming: Comparing ...</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#lisp`, `#forth`, `#language-design`, `#paradigms`

---

<a id="item-8"></a>
## [Lean 在 DEFLATE 压缩基准测试中超越 Rust](https://kim-em.github.io/blog/2026-7-24-why-lean-is-faster-than-rust/) ⭐️ 7.0/10

一篇新博客文章详细介绍了如何在 Lean 4 编程语言中实现 DEFLATE 压缩算法，并取得了比同类 Rust 实现更快的性能。作者探讨了这一意外结果背后的技术原因，挑战了人们对系统级编程语言性能的常见假设。 这一结果意义重大，因为 Lean 主要以定理证明器和证明助手闻名，而非高性能系统级编程语言。证明 Lean 能够在原始计算任务中与 Rust 竞争甚至超越它，可能会扩大其应用范围，并重塑人们对形式化验证语言能力的认知。 该博客文章深入探讨了具体的编译器优化、内存管理策略和算法选择，这些因素使 Lean 在这一特定基准测试中超越了 Rust。这一具有挑衅性的比较突显了不同语言运行时和编译器在处理底层数据任务时的细微差别。

rss · Lobsters · Jul 26, 15:54

**背景**: Lean 是一种函数式编程语言和交互式定理证明器，主要由 Leonardo de Moura 开发，其最新版本 Lean 4 同时也可作为通用编程语言使用。DEFLATE 是一种广泛使用的无损数据压缩算法，结合了 LZ77 和 Huffman 编码，在 RFC 1951 中定义，并用于 gzip、ZIP 和 PNG 等格式。Rust 是一种以内存安全保证和高性能著称的系统级编程语言，常被用作比较语言效率的基准标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DEFLATE_compression_algorithm">DEFLATE compression algorithm</a></li>
<li><a href="https://github.com/leanprover/lean4">GitHub - leanprover/lean4: Lean 4 programming language and theorem prover · GitHub</a></li>

</ul>
</details>

**标签**: `#Lean`, `#Rust`, `#compression`, `#performance`, `#systems-programming`

---

<a id="item-9"></a>
## [探索 Valkey 内部数据生命周期](https://valkey.io/blog/secret-life-of-data/) ⭐️ 7.0/10

Valkey 官方博客发布了一篇题为"The secret life of data in Valkey"的深度技术文章，详细探讨了数据在 Valkey 内存数据库系统内部的整个生命周期中是如何被处理、存储和管理的。 了解 Valkey 的内部数据处理机制对于依赖这一兼容 Redis 数据库进行高性能缓存和数据存储的系统工程师和开发者至关重要，因为它有助于更好地进行性能优化和故障排查。 该文章深入介绍了 Valkey 的数据结构和内存管理内部架构，面向对数据库实现细节而非表面用法感兴趣的技术型读者。

rss · Lobsters · Jul 26, 21:28

**背景**: Valkey 是一个开源内存 NoSQL 数据库，在 2024 年 Redis 将许可证更改为源码可用模式后从 Redis 分叉而来。它在 Linux 基金会下进行开发，保持与旧版 Redis OSS 的兼容性，被广泛用作生产系统中的缓存、消息代理和数据存储。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://valkey.io/">Valkey</a></li>
<li><a href="https://redis.io/blog/what-is-valkey/">What is Valkey? A comparison with Redis</a></li>
<li><a href="https://dimasyotama.medium.com/valkey-vs-redis-the-fork-awakens-understanding-the-split-key-differences-and-implementation-89c0123403eb">Valkey vs . Redis : The Fork Awakens — Understanding the... | Medium</a></li>

</ul>
</details>

**标签**: `#Valkey`, `#database-internals`, `#in-memory-database`, `#systems-engineering`, `#data-structures`

---

<a id="item-10"></a>
## [美国公民因在边境使用胁迫密码擦除手机数据被起诉](https://www.theverge.com/policy/971097/us-charging-american-citizen-wiping-phone-duress-password) ⭐️ 7.0/10

美国政府正在起诉美国公民 Sam Tunick，指控他于 2025 年 1 月 24 日在亚特兰大 Hartsfield-Jackson 机场向联邦探员提供了一个胁迫密码，导致手机数据被擦除。这被认为是美国首例联邦检察官因嫌疑人使用手机内置胁迫密码功能销毁数据而提起的刑事指控。 此案在数字隐私与边境安全的交汇处确立了一个可能具有重大意义的法律先例，表明胁迫密码等隐私保护功能可能使用户面临刑事责任。这对设计加密工具的安全专业人员和开发者，以及关注边境第四修正案权利的公民自由倡导者都具有重大影响。 联邦探员拘留了 Tunick 并指控就儿童剥削图像对其进行询问，随后试图扣押他的手机，而他据报提供了触发数据擦除的胁迫密码。法律争论的焦点在于，使用旨在保护用户的内置软件功能是否构成联邦法律下的故意销毁证据行为。

rss · The Verge · Jul 26, 18:45

**背景**: 胁迫密码是某些操作系统（尤其是 GrapheneOS）提供的一项安全功能，允许用户设置一个备用 PIN 或密码，当在胁迫下输入时，表面上会解锁设备，但实际上会擦除数据或显示一个伪装配置文件。该功能旨在保护用户在被迫交出凭证时的敏感信息。第四修正案保护公民免受不合理的搜查和扣押，但美国法院历来根据

**标签**: `#digital-privacy`, `#encryption`, `#border-security`, `#civil-liberties`, `#legal-policy`

---