---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 184 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [GLM-5.3 发布：具备新兴网络能力的编程模型](#item-tech-news-1) ⭐️ 9.0/10
2. [中国医生用 GPT-5.6 证明 22 年数学难题，Crouzeix 本人确认](#item-tech-news-2) ⭐️ 9.0/10
3. [Qwen 3.8 27B 开源模型获社区好评](#item-tech-news-3) ⭐️ 8.0/10
4. [执法黑客时代：加密普及下的暗战](#item-tech-news-4) ⭐️ 8.0/10
5. [Linux 内核、musl libc 和 BGP 实现 IPv8 互联网草案](#item-tech-news-5) ⭐️ 8.0/10
6. [英伟达全面投产全球首款 200G/lane CPO 以太网交换机](#item-tech-news-6) ⭐️ 8.0/10
7. [将 Doom 渲染器编译为 210 亿参数 Transformer，无需训练](#item-tech-news-7) ⭐️ 8.0/10
8. [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](#item-tech-news-8) ⭐️ 8.0/10
9. [苹果联手阿里自研中国专属 AI 大模型，或成首个获批外企](#item-tech-news-9) ⭐️ 8.0/10

**财经新闻**
1. [SpaceX 以 600 亿美元收购 AI 编程公司 Cursor](#item-finance-news-1) ⭐️ 9.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GLM-5.3 发布：具备新兴网络能力的编程模型](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

智谱 AI 发布了 GLM-5.3，该模型具备前沿编程能力和新兴的网络能力，能够自主进行安全研究和漏洞发现。据社区用户反馈，该模型在红队场景中表现出色，包括发现 WordPress 插件中的零日漏洞、实现远程代码执行（RCE）以及适配 6.8 内核漏洞利用等。此外，智谱 AI 还通过 cvd.z.ai 平台公开披露了其扫描开源软件和流行软件所发现的漏洞，其中许多已被分配 CVE 编号，且大多处于保密状态。该模型基于 GLM 5.2 进行后训练优化，目前权重尚未公开发布，预计两周后可用。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**「背景」** GLM-5.3 是智谱 AI（Z.ai）于 2026 年 8 月发布的开源权重模型，基于 7430 亿参数的基座模型进行后训练，重点提升编码与智能体能力，并意外涌现出网络安全能力。据 Z.ai 报告，该模型在 Terminal Bench 3.0 上创下开源模型最高分，内部编码智能体评测比 GLM-5.2 提升 50%。此前 GLM-5.2 已具备较强编码能力，而 GLM-5.3 的网络安全能力在训练扩展中增长超出预期，被定位为防御性能力。

**「影响」** GLM-5.3 的发布可能显著提升 AI 辅助安全研究的效率和可及性，使更多组织能够自主发现和修复漏洞，但同时也引发了关于大规模漏洞扫描和披露政策对软件生态影响的讨论。

**「社区讨论」** 社区用户对 GLM-5.3 的性能表示高度认可，认为其接近甚至超越其他前沿模型，但也有用户指出其仍落后于 Sol 和 Fable。部分用户赞赏智谱 AI 的研究风格，认为其文档更专业而非营销炒作。同时，有用户对大规模漏洞扫描的成本和披露政策提出质疑，认为这可能带来新的安全挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/glm-5-3-launch-cyber-defense-benchmarks-august-2026">GLM-5.3 Launch: Benchmarks, Pricing &amp; Access (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>
<li><a href="https://siliconangle.com/2026/08/14/z-ai-debuts-glm-5-3-long-horizon-coding-cybersecurity-upgrades/">Z.ai debuts GLM-5.3 with long-horizon coding, cybersecurity upgrades - SiliconANGLE</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#coding`, `#GLM`, `#vulnerability discovery`

---

<a id="item-tech-news-2"></a>
### [中国医生用 GPT-5.6 证明 22 年数学难题，Crouzeix 本人确认](https://www.ithome.com/0/989/952.htm) ⭐️ 9.0/10

据《南华早报》报道，北京协和医院神经外科博士后金山木利用 OpenAI 的 GPT-5.6-Sol 模型，在约 16 小时内证明了自 2004 年以来困扰数学界 22 年的 Crouzeix 猜想。美国康奈尔大学数学家 Alex Townsend 与华盛顿大学数学系教授 Anne Greenbaum 公开了与金山木的邮件往来，并确认他们以及猜想提出者、法国数学家 Michel Crouzeix 本人均已审阅论文手稿，确认证明正确无误。金山木的学术背景为地质学和临床医学，数学知识主要靠自学，他采用非常规方法，在物理断网环境下让模型自主运行，经历数万次假设与推翻后得到证明。金山木已将全部研究资料开源，包括论文、提示词、迭代手稿、Lean 4 形式化证明代码及公理审计报告。在预印本发布仅 8 天后，数学家 Emiel Lorist 和 Felix Schwenninger 于 2026 年 8 月初发布了独立证明，思路不同，且同样使用了 ChatGPT 5.6。

rss · IT HOME · 8月14日 15:08

**「背景」** Crouzeix 猜想由法国数学家 Michel Crouzeix 于 2004 年提出，核心内容是：对于任意矩阵和任意多项式函数，矩阵经函数作用后的范数不超过该函数在矩阵数值域上最大值的两倍。该猜想表述简洁但证明难度极高，2007 年 Crouzeix 本人仅证明了常数在 11.08 时成立，2017 年全球顶尖专家在美国数学研究所专题研讨会上将常数降至 2.414，此后无实质进展。金山木是北京协和医院神经外科博士后，本科为北京大学地质学专业，2020 年通过协和医学院“4+4 试点班”转入临床医学，其数学知识均为自学。

**「影响」** 这一突破展示了 AI 在数学研究中的实际能力，可能加速 AI 辅助证明的接受度，并对数学研究方法和工具链产生深远影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nationpress.com/sciencetech/surgeon-cracks-20-year-maths-problem-with-gpt">Beijing surgeon solves 20-year-old Crouzeix conjecture using ...</a></li>
<li><a href="https://github.com/jinshanmu/CrouzeixConjecture">GitHub - jinshanmu/CrouzeixConjecture: Research draft of a ...</a></li>
<li><a href="https://alextownsend.net/essays/SIAMNews_CrouzeixConjecture.pdf">The Neurosurgery Resident Who Proved Crouzeix’s Conjecture</a></li>

</ul>
</details>

**标签**: `#AI-assisted proof`, `#Crouzeix conjecture`, `#GPT-5.6`, `#mathematics`, `#OpenAI`

---

<a id="item-tech-news-3"></a>
### [Qwen 3.8 27B 开源模型获社区好评](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B 是一个新发布的开源 AI 模型，因其推理能力和输出质量而受到社区关注。用户报告称，该模型是继 Gemma 4 之后第二个能够正确通过其私有基准测试的本地模型，尽管它消耗了 5 倍的 token 和 12 分 30 秒（启用 MTP）才完成推理。该模型在显存使用效率上不如 Gemma 4 或 Glimmer，但它在推理时表现出更显式的思考过程。社区讨论还强调了该模型在笔记本电脑上的出色表现，以及它与其他开源模型（如 GLM 5.3 和 Deepseek）一起，可能预示着前沿 AI 能力的商品化，对 OpenAI 和 Anthropic 等公司构成潜在挑战。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**「背景」** Qwen 3.8 27B 是阿里巴巴旗下 Qwen 团队于 2026 年 8 月 14 日发布的开源大语言模型，参数规模为 27B，上下文窗口为 262k。该模型与 Qwen 3.8-Max 一同宣布，但 Qwen 3.8 27B 的开放权重版本更受本地 AI 社区关注，因为它可以在消费级硬件上运行。此前，Qwen 系列模型（如 Qwen 3.6）已在开源社区中建立了良好声誉，而 Qwen 3.8 27B 的发布被视为本地 AI 领域的重要进展。

**「影响」** 对于在本地运行模型的开发者和研究者，Qwen 3.8 27B 提供了又一个高性能开源选择，其推理能力可与 Gemma 4 相媲美，但显存效率较低，可能限制其在资源受限环境中的使用。

**「社区讨论」** 社区普遍对该模型的性能表示赞赏，有用户称其为“最好的鹈鹕”绘图示例，并指出其推理痕迹与之前版本相比有显著变化，但有人怀疑这种独特的思考模式可能影响 MTP 预测效率。此外，有用户提到 Jinja 模板存在问题，建议使用特定工具来减少或关闭相关功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@rosgluk/qwen-3-8-27b-is-coming-and-it-could-be-the-most-important-local-ai-release-of-2026-c1cf381d5292">Qwen 3.8 27B Is Coming - and It Could Be the Most Important Local AI Release of 2026 | by Rost Glukhov | Aug, 2026 | Medium</a></li>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://aireleasetracker.com/model/qwen/qwen3.8-27b">Qwen3.8-27B — Benchmarks, Specs &amp; Release Date</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Model Release`, `#LLM`, `#Benchmark`

---

<a id="item-tech-news-4"></a>
### [执法黑客时代：加密普及下的暗战](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

一篇来自知名密码学博客的分析文章指出，随着加密技术的普及，执法机构正从传统监听转向“执法黑客”手段，即通过入侵设备或利用软件漏洞获取信息。文章认为，这一转变对软件安全和隐私具有深远影响，并预测可利用的漏洞数量可能很快达到上限，而人工智能可能改变软件安全格局。作者强调，这并非呼吁专家采取复杂行动，而是提醒关注这一趋势的后果。文章引发了关于漏洞数量、AI 对软件质量影响以及执法权限边界的讨论。

hackernews · vslira · 8月14日 20:52 · [社区讨论](https://news.ycombinator.com/item?id=49304447)

**「背景」** “Going Dark”一词源于 2014 年时任 FBI 局长 James Comey 发起的倡议，旨在讨论加密技术如何阻碍执法机构获取通信内容，并寻求让服务提供商配合执法的方法。随着端到端加密的普及，执法部门传统的监听手段失效，转而发展“执法黑客”技术，即通过入侵设备或利用软件漏洞获取信息。这一背景有助于理解当前关于加密、隐私与执法需求之间平衡的争论。

**「影响」** 对于依赖加密保护数据的用户和开发者而言，执法黑客手段的兴起意味着设备安全漏洞可能成为执法工具，从而削弱加密提供的隐私保障，并促使软件行业重新评估漏洞披露和修复的优先级。

**「社区讨论」** 评论者中，有人对“漏洞数量将达上限”的观点表示怀疑，认为 AI 辅助开发可能反而增加软件缺陷；也有人对比了执法机构的高技术手段与普通企业糟糕的安全实践，指出安全鸿沟的存在。此外，有评论者提醒，电话监听的历史远早于计算机时代，执法黑客并非全新现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/">Everything is about to “go dark” – A Few Thoughts on ...</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#law-enforcement`, `#security`, `#privacy`, `#encryption`

---

<a id="item-tech-news-5"></a>
### [Linux 内核、musl libc 和 BGP 实现 IPv8 互联网草案](https://goonhost.rocks/blog/implementing-ipv8-internet-draft) ⭐️ 8.0/10

一个团队在 Linux 内核、musl libc 和 BGP 中实现了 IPv8 互联网草案，这是一项重大的系统工程成就。该实现展示了在核心网络基础设施中部署新协议的能力，可能影响未来协议的采用。尽管 IPv8 仍是一个互联网草案，尚未广泛部署，但这项工作为评估其可行性提供了实际基础。具体的技术细节和性能数据未在源内容中提供。

rss · Lobsters · 8月14日 19:05

**「背景」** IPv8（Internet Protocol Version 8）是一个由 IETF 互联网领域工作组提出的互联网协议草案（draft-thain-ipv8），旨在构建一个可管理的网络协议套件，通过 OAuth2 JWT 令牌授权网络中的每个可管理元素，并引入 64 位 ASN 前缀地址、将 IPv4 作为其真子集，以及一个整合 DHCP、DNS、认证和出口控制的 Zone Server。该草案目前仍处于标准跟踪状态，尚未广泛部署。

**「影响」** 对于网络研究人员和协议开发者，这一实现提供了 IPv8 在真实系统上运行的实证，有助于评估其设计并推动标准化进程。然而，由于 IPv8 尚未成为标准且部署有限，其短期影响可能局限于实验和学术领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-thain-ipv8-00.html">Internet Protocol Version 8 (IPv8) - ietf.org</a></li>
<li><a href="https://datatracker.ietf.org/doc/draft-thain-ipv8/">draft-thain-ipv8-02 - Internet Protocol Version 8 (IPv8)</a></li>
<li><a href="https://transitai.app/blog/ipv8-draft-zone-server-math/">IPv8: The Draft of a New Internet — Transit AI</a></li>

</ul>
</details>

**标签**: `#IPv8`, `#Linux kernel`, `#networking`, `#BGP`, `#systems programming`

---

<a id="item-tech-news-6"></a>
### [英伟达全面投产全球首款 200G/lane CPO 以太网交换机](https://www.ithome.com/0/989/970.htm) ⭐️ 8.0/10

英伟达于 8 月 14 日宣布全面投产 Spectrum-X 以太网光子交换机，这是全球首款量产的 200G/lane 共封装光器件（CPO）以太网交换机系统，主要面向大规模 AI 训练与推理集群。该交换机将光学引擎与交换芯片封装在同一模块内，并采用外置激光源模块统一供光，所需激光器数量仅为传统方案的 1/4。相比传统可插拔光模块，英伟达称功耗降低至 1/5，AI 应用无中断运行时间延长 5 倍，平均事件间隔时间提高 10 倍。硬件方面，SN6810 在 2U 液冷机箱内提供 128 个 800Gb/s 端口，总交换能力 102.4Tb/s；SN6800 在 5U 系统中堆叠 4 颗 ASIC，提供 409.6Tb/s 交换能力，支持 512 个 800Gb/s 端口或超过 2000 个 200Gb/s 端口。制造由台积电负责硅光子技术，SPIL 负责封装测试，Lumentum 与 TFC 供应激光器，富士康开发整机系统，英伟达已完成最终测试并启动全面生产。

rss · IT HOME · 8月14日 22:53

**「背景」** 共封装光器件（CPO）是一种将光学引擎与交换芯片集成在同一封装内的技术，旨在缩短电信号传输路径，降低功耗和延迟。传统可插拔光模块方案中，光模块独立于交换机面板，电光转换距离较远，功耗和故障点较多。英伟达此前已推出基于 InfiniBand 的 CPO 产品，而 Spectrum-X 是其首款以太网 CPO 交换机，标志着 CPO 技术在以太网领域的量产应用。

**「影响」** 该产品的量产将显著降低 AI 集群的网络功耗和故障率，提升运行稳定性，对大规模 AI 基础设施的建设和运营成本产生直接影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lightcounting.com/research-note/march-2025-nvidias-cpo-is-the-first-step-in-a-long-journey-395">LightCounting :: March 2025 Nvidia &#x27;s CPO is the First Step in a Long...</a></li>
<li><a href="https://www.linkedin.com/pulse/co-packaged-optics-cpos-deep-dive-sharada-yeluri-e0hyc">Co-Packaged Optics ( CPOs ) - A Deep Dive</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#CPO`, `#Ethernet switch`, `#AI infrastructure`, `#silicon photonics`

---

<a id="item-tech-news-7"></a>
### [将 Doom 渲染器编译为 210 亿参数 Transformer，无需训练](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

一位开发者（Reddit 用户 notforrob）编写了一个编译器，将 Doom 的渲染算法转换为一个 210 亿参数的 Transformer 检查点，该检查点无需训练即可生成像素绘制命令来渲染游戏帧。生成的检查点可作为标准 Hugging Face 检查点加载，无需 trust\_remote\_code。主机程序仅 43 行 Python 代码，用于加载检查点、生成渲染并解析输出为 E1M1 帧。每帧需要 3,614 个 token 的提示和 53,747 个生成 token，在 B200 上耗时约 40 分钟，而原版 Doom 在 486 上可达 35 FPS，此实现约为每天 35 帧。项目提供了完整的代码、权重和文档。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**「背景」** Transformer 通常通过大量数据训练来学习任务，而此项目采用了一种不同的方法：使用编译器将计算图直接转换为 Transformer 权重，从而将算法编码到模型中。Doom 的渲染器是一个经典的实时 3D 渲染算法，通过将其移植到兼容的计算图中，该编译器能够生成一个无需训练即可执行渲染任务的 Transformer。

**「影响」** 这一成果展示了将真实世界算法编译为 Transformer 权重的可行性，为模型可解释性和程序合成提供了新思路，可能影响未来将传统代码嵌入神经网络的方法。

**标签**: `#transformer`, `#compilation`, `#Doom`, `#neural networks`, `#program synthesis`

---

<a id="item-tech-news-8"></a>
### [小红书开源 dots3-note：280B MoE 仅 16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note preview，这是 dots3 系列首个开放权重模型。该模型总参数达 280B，但每次推理仅激活 16B 参数，支持 512K 上下文，并能处理文字、图片、视频和音频等多模态输入。模型引入了新的强化学习方法 TEMPO，通过自批判和测试时价值估计来训练长程智能体。权重已在 Hugging Face 上开源，同时发布了 VibeSearchBench 和 VibeLifeBench 两个真实场景智能体基准。此次开源为 AI 社区提供了高效的大规模 MoE 模型，并推动了多模态和强化学习领域的发展。

telegram · zaihuapd · 8月14日 08:27

**「背景」** dots3-note preview 是小红书 dots 实验室开源的 dots3 系列首个开放权重模型，采用混合专家（MoE）架构，总参数 280B，激活参数 16B，支持最长 512K token 的上下文，能够处理文本、图像、视频和音频输入并生成文本输出。该模型引入了名为 TEMPO 的强化学习方法，通过自批判和测试时价值估计来训练长程智能体，并同步发布了 VibeSearchBench 和 VibeLifeBench 两个面向真实场景的智能体基准。

**「影响」** 该开源模型为 AI 开发者和研究者提供了一个高效的大规模 MoE 模型，其 16B 激活参数和 512K 上下文支持，使得在有限计算资源下处理长序列多模态任务成为可能，同时 TEMPO 方法和新基准为智能体训练与评估提供了新工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/dots3-note-prev: dots3 note preview</a></li>
<li><a href="https://eu.36kr.com/en/p/3938759517896072">Xiaohongshu Open-Sourced Dots3-Note: The Same-Series Model ...</a></li>
<li><a href="https://huggingface.co/dots-studio/dots3-note-prev">dots-studio/dots3-note-prev · Hugging Face</a></li>

</ul>
</details>

**标签**: `#open-source`, `#MoE`, `#multimodal`, `#reinforcement-learning`, `#benchmarks`

---

<a id="item-tech-news-9"></a>
### [苹果联手阿里自研中国专属 AI 大模型，或成首个获批外企](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

据路透社报道，苹果已专门为中国市场训练一款大语言模型，并获得了阿里巴巴的支持，改变了此前依赖第三方模型的策略。苹果的生成式 AI 服务已在上月获得中国网信办备案，Apple Intelligence 预计将在未来数月随 iOS 更新在华上线。若落地，苹果可能成为首个获北京批准在华提供自有 AI 模型的外国公司。此举将使苹果更好地掌控中国市场的 AI 体验，并具有重要的战略意义。

telegram · zaihuapd · 8月14日 14:47

**「背景」** 苹果此前计划在中国市场依赖本地合作伙伴提供的 AI 技术，而非自研模型。此次与阿里巴巴合作训练专为中国市场定制的大语言模型，标志着苹果战略的转变，旨在更好地掌控其在中国设备生态系统中的 AI 体验。这一合作发生在中美科技紧张局势加剧的背景下，显得尤为突出。

**「影响」** 此举可能使苹果成为首个在中国获批提供自有 AI 模型的外国公司，从而增强其在中国市场的竞争力，并对其他外国科技公司进入中国 AI 市场产生示范效应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.remio.ai/post/alibaba-apple-ai-partnership-gives-apple-more-control-in-china">Alibaba Apple AI Partnership Gives Apple More Control in China</a></li>
<li><a href="https://clashreport.com/world/articles/apple-develops-china-specific-ai-model-in-partnership-with-alibaba-qfsiu4onya">Apple Develops China -Specific AI Model in Partnership With Alibaba</a></li>
<li><a href="https://aichief.com/news/apple-taps-alibaba-for-china-ai-model-training/">Apple Taps Alibaba for China AI Model Training</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Regulation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [SpaceX 以 600 亿美元收购 AI 编程公司 Cursor](https://www.ithome.com/0/989/944.htm) ⭐️ 9.0/10

SpaceX 完成了对 AI 编程初创公司 Cursor 的 600 亿美元（约合 4,054.22 亿元人民币）收购，这是科技行业史上最大收购之一。监管文件显示，收购于当地时间 8 月 14 日正式生效，SpaceX 两个月前已宣布达成收购协议。

rss · IT HOME · 8月14日 14:34

**「背景」** SpaceX 于两个月前宣布与 Cursor 达成收购协议，此次交易以全股票形式完成，是科技行业史上规模最大的收购之一。Cursor 是一家 AI 编程初创公司，其 AI 编程助手可帮助程序员提高代码编写和调试效率。

**「影响」** 此次收购将增强 SpaceX 在 AI 编程领域的竞争力，Cursor 团队将获得 SpaceX 的先进 AI 芯片和全球最大 GPU 集群的算力支持，有助于开发更强大、成本更低的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.forbes.com/sites/sandycarter/2026/06/16/spacex-buys-cursor-in-largest-startup-acquisition-ever-at-60-billion/">SpaceX Buys Cursor In Largest Startup Acquisition Ever At $60 ...</a></li>
<li><a href="https://www.cnbc.com/2026/06/16/spacex-spcx-cursor-acquisition-ipo.html">SpaceX to acquire the AI coding startup Cursor for $60 billion</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Cursor`, `#acquisition`, `#AI`, `#tech industry`

---