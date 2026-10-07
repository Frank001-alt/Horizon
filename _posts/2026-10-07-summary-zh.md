---
layout: default
title: "Horizon Summary: 2026-10-07 (ZH)"
date: 2026-10-07
lang: zh
---

> 从 203 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [OpenAI 发布数学 AI 成果，声称解决 90 个开放问题](#item-tech-news-1) ⭐️ 9.0/10
2. [Mistral 发布 Large 4：欧洲自研旗舰模型](#item-tech-news-2) ⭐️ 8.0/10
3. [谷歌发布 EmbeddingGemma 2 轻量多模态嵌入模型](#item-tech-news-3) ⭐️ 8.0/10
4. [AnyPS5：无需模拟器将 PS5 二进制移植到 PC](#item-tech-news-4) ⭐️ 8.0/10
5. [2026 年诺贝尔物理学奖授予冰立方构想者弗朗西斯·哈尔岑](#item-tech-news-5) ⭐️ 8.0/10
6. [Polars 2.0 正式发布](#item-tech-news-6) ⭐️ 8.0/10
7. [合成先验训练字节级 Transformer 实现语言上下文学习](#item-tech-news-7) ⭐️ 8.0/10

**财经新闻**
1. [派拉蒙天舞完成 1100 亿美元收购华纳兄弟探索](#item-finance-news-1) ⭐️ 8.0/10
2. [SpaceX 据报拟募资 400 亿美元采购英伟达芯片](#item-finance-news-2) ⭐️ 8.0/10
3. [谷歌与 Constellation 签署 3.59GW 长期电力协议](#item-finance-news-3) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [OpenAI 发布数学 AI 成果，声称解决 90 个开放问题](https://openai.com/index/sharing-ai-progress-in-mathematics/) ⭐️ 9.0/10

OpenAI 在 GitHub 上发布了名为 openai/math 的仓库，其中包含预印本，声称已完全解决数学领域前 500 个开放问题中的 90 个。据社区评论者 zone411 的核查，其中排名最高的包括希尔伯特第十问题（有理数域上，排名第 22）、Unique Games（第 29）、Anderson 模型扩展态（第 31）、时空 Penrose 不等式（第 37）、Landau–Siegel 零点不存在性（第 48）、Baum–Connes（第 52）、Abundance（第 78）、Hadwiger（第 80）、玻色–爱因斯坦凝聚（第 87）以及二维纠缠（第 92）等。评论者 NotOscarWilde 指出，其中三机器单位作业调度的多项式时间算法自 1979 年 Garey 和 Johnson 的著作以来一直是开放问题，但其重要性低于 Unique Games 猜想。评论者 prideout 表示，仓库中包含 Barnette 猜想的证明，而他此前用最先进模型尝试攻克该猜想未能成功。这些声明极为重大，其验证情况仍存在不确定性。

hackernews · OpenAI Blog · 10月6日 22:17 · [社区讨论](https://news.ycombinator.com/item?id=49984923)

**「背景」** OpenAI 此次发布的是其内部前沿模型在数学开放问题上的新结果，并在 GitHub 上公开了 Lean 证明形式化与研究细节。据 Scientific American 报道，这些结果以 GitHub 仓库形式于美国东部时间下午 6 点公布，数学家可能需要数月时间才能消化，并判断这些证明是否包含新颖重要的思想，还是主要对现有技术的拼接。纽约时报则称 OpenAI 发布了覆盖代数、数论、理论计算机科学、数学逻辑等多个领域的数百项新发现。

**「影响」** 若这些结果通过验证，数学与理论计算机科学领域的研究者将获得一批长期悬而未决问题的候选证明，其中 Unique Games 猜想等结果可能直接影响大量不可近似性结论的成立基础。不过目前这些证明仍处于待同行验证阶段，其正确性与实际影响尚不确定。

**「社区讨论」** 社区讨论既关注这些成果的潜在重要性，也关注其可信度。评论者 xanderlewis 引用 Kevin Buzzard 的话，称人们正开始理解“如果一个人同时理解所有现代纯数学，能立刻看到多远”这一问题的答案。NotOscarWilde 从理论计算机科学和调度的角度指出，三机器调度结果的重要性低于 Unique Games 猜想，但自 1979 年以来一直是开放问题。prideout 提到自己曾用最先进模型尝试证明 Barnette 猜想但失败，并认为 OpenAI 的证明乍看之下是可理解的。enoether 则强调 Unique Games 猜想是复杂性理论中的开创性猜想，也是许多不可近似性结果的底层假设。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/sharing-ai-progress-in-mathematics/">Sharing AI progress in mathematics - OpenAI</a></li>
<li><a href="https://www.scientificamerican.com/article/openai-unleashes-hundreds-more-math-results-upon-a-field-already-in-shock/">OpenAI unleashes hundreds more math results... | Scientific American</a></li>
<li><a href="https://www.nytimes.com/2026/10/06/science/openai-math-problems.html">OpenAI Releases Findings on 377 Math Problems, Further ...</a></li>

</ul>
</details>

**标签**: `#AI for mathematics`, `#automated theorem proving`, `#open problems`, `#research`, `#OpenAI`

---

<a id="item-tech-news-2"></a>
### [Mistral 发布 Large 4：欧洲自研旗舰模型](https://mistral.ai/news/mistral-large-4//) ⭐️ 8.0/10

Mistral 发布新一代旗舰模型 Mistral Large 4（ML4），官方称其从零开始训练，使用约 3800 块 NVIDIA Grace Blackwell GPU，部署于 Mistral 位于欧洲的自有数据中心。该模型在 Hacker News 上引发大量讨论（1596 分、968 条评论），焦点集中在其基准测试成绩与推理控制机制上。开发者 Simon Willison 指出，该模型仅支持 reasoning 的“none”与“high”两档，且实测差异不明显，high 档甚至比 none 档输出更少 token，但 high 档生成的自行车车架 SVG 质量更好。有评论者称其在视觉基准上表现突出，网络安全类基准优于所有中国模型，并认为若视觉能力真如 Astra 般出色则可能是全球最佳。另有 Plotly 员工称在内部数据分析基准上，ML4 比 4 月的 Mistral Medium 3.5 便宜 10 倍，正确率从 58% 提升至 74%。

hackernews · Philpax · 10月6日 13:15 · [社区讨论](https://news.ycombinator.com/item?id=49977979)

**「背景」** Mistral 是一家总部位于法国的 AI 公司，此前已发布多代 Large 系列旗舰模型。Mistral Large 4 于 2026 年 10 月 6 日发布，目前处于 Research Public Preview 阶段，官方计划在 10 月底开放其 1T 参数（49B 激活）模型的权重。据第三方评测，该模型在 Artificial Analysis 智能指数上得分为 38，在 GDP.pdf 文档推理评测中得分为 19%。

**「影响」** 对需要数据主权或合规保障的欧洲企业而言，Mistral Large 4 提供了在欧盟境内训练与推理的选项，但其运行仍依赖 NVIDIA Grace Blackwell GPU，形成所谓“主权悖论”。开发者社区反馈显示，该模型在数据分析等任务上较 Mistral Medium 3.5 成本降低约 10 倍、准确率从 58% 提升至 74%，但推理控制仅支持“none”与“high”两档且实际差异有限。

**「社区讨论」** 社区对 ML4 的基准成绩总体评价积极，认为其视觉与网络安全能力突出，可作为日常使用的替代模型，并强调其在欧盟训练与推理对欧洲主权 AI 的意义。同时存在质疑：有评论者追问，若约 1T 参数模型仅用约 4000 块 GB GPU 训练就能接近 Kimi K3 水平，这对其他实验室意味着什么；也有人对推理档位设置的实际效果表示怀疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.benchleader.com/models/mistral-large-4">Mistral Large 4: benchmarks, pricing, speed and rank (2026)</a></li>
<li><a href="https://artificialanalysis.ai/articles/mistral-large-4-france-ai">Mistral has released Mistral Large 4, making France home to ...</a></li>
<li><a href="https://www.unite.ai/benchmark-firm-gives-mistral-large-4-preview-a-38-intelligence-score/">Benchmark Firm Gives Mistral Large 4 Preview a 38 ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/mistral-large-4-doesn-t-155055704.html?fr=sycsrp_catchall">Mistral Large 4 Doesn’t Just Compete With Chinese Open ...</a></li>
<li><a href="https://byteiota.com/mistral-large-4-drops-today-open-weights-on-october-27/">Mistral Large 4 Drops Today: Open Weights on October 27</a></li>
<li><a href="https://www.constellationr.com/insights/news/mistral-makes-its-open-model-case-mistral-large-4">Mistral makes its open model case with Mistral Large 4</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Mistral`, `#AI models`, `#model training`, `#benchmarks`

---

<a id="item-tech-news-3"></a>
### [谷歌发布 EmbeddingGemma 2 轻量多模态嵌入模型](https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2/) ⭐️ 8.0/10

谷歌发布了 EmbeddingGemma 2，这是一个采用 Apache 2.0 许可证的开放轻量级多模态嵌入模型。该模型提供两种规格：纯文本版本为 2.7 亿参数，文本加视觉版本总计 4.4 亿参数。此前谷歌于去年推出的 EmbeddingGemma 下载量已超过 2000 万次，主要应用于端侧搜索工具和隐私优先的检索增强生成（RAG）管线。此次新版本在 Hacker News 上引发了从业者的强烈关注，讨论集中在许可证、量化以及实际部署等方面。

hackernews · ilreb · 10月6日 16:03 · [社区讨论](https://news.ycombinator.com/item?id=49980487)

**「背景」** 嵌入模型（embedding model）将文本、图像等内容映射为向量，供检索、聚类和检索增强生成（RAG）等下游任务比较与存储。谷歌此前推出的 EmbeddingGemma 已提供轻量文本嵌入方案，据 IT 之家报道其下载量超过 2000 万次，广泛用于端侧搜索和隐私优先的 RAG 管线。EmbeddingGemma 2 延续这一路线，据谷歌开发者博客介绍，它以 Apache 2.0 许可发布，是面向端侧多模态嵌入的紧凑开放模型，可将文本、图像、音频和视频的组合原生映射到统一嵌入空间。

**「影响」** 对构建检索与嵌入管线的开发者而言，Apache 2.0 许可意味着可自行托管并长期保存数百万条向量，避免专有模型停服导致的历史嵌入失效风险；270M 文本版与 440M 文本+视觉版也降低了端侧部署门槛。不过目前尚无公开基准数据，实际检索质量仍需等待评测验证。

**「社区讨论」** 社区普遍赞赏该模型采用 Apache 2.0 许可证，simonw 指出嵌入模型涉及存储数百万向量，专有托管模型存在供应商停服风险。minimaxir 认为中等规模嵌入模型此前存在空白，2.7 亿文本参数和 4.4 亿文本加视觉参数较为合理。kaycebasques 询问二进制量化是否适用于 EmbeddingGemma 2，flockonus 则称赞谷歌开放了可能用于 Android 手机的模型权重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.googleblog.com/embeddinggemma-2-the-developer-guide/?ref=communeify.com">EmbeddingGemma 2 : The Developer Guide - Google Developers Blog</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2/">EmbeddingGemma 2 is a best-in-class open model for natively...</a></li>

</ul>
</details>

**标签**: `#embeddings`, `#multimodal`, `#open-source`, `#machine-learning`, `#google`

---

<a id="item-tech-news-4"></a>
### [AnyPS5：无需模拟器将 PS5 二进制移植到 PC](https://github.com/boykopovar/AnyPS5) ⭐️ 8.0/10

AnyPS5 是一个逆向工程项目，旨在无需模拟器的情况下将 PS5 二进制文件移植到 PC 上运行，目前已映射了 87% 的系统库。该项目由 boykopovar 发布在 GitHub 上，并在 Hacker News 上引发了 107 分、79 条评论的讨论。其核心思路是通过直接映射 PS5 系统库来实现二进制兼容，而非依赖传统的模拟层，这在技术路径上具有新颖性。该项目尚未完成，也并非正式的行业发布，但因其对软件兼容性和厂商锁定的潜在影响而受到关注。

hackernews · Fe2O3 · 10月6日 23:28 · [社区讨论](https://news.ycombinator.com/item?id=49985664)

**「背景」** 传统上在 PC 上运行主机游戏依赖模拟器，即用软件模拟 PS5 的硬件与系统环境，而 AnyPS5 走的是另一条路线：它通过重链接（relinking）改写游戏自身的程序，用社区制作的替代实现替换索尼的系统软件，最终输出可在 Windows 或 Linux 上运行的 .exe 文件，而非模拟硬件。据外部报道，该项目大量借助 AI 辅助开发，其 467 个拉取请求被标记为 AI 参与。目前项目尚无公开发布版本，开发者称工具最多只能执行到游戏的主函数，尚未完整运行任何一款游戏。

**「影响」** 若该项目持续发展，可能为 PS5 独占游戏在 PC 上运行提供一条不依赖模拟器的兼容路径，从而削弱索尼对 PS5 软件分发的控制并降低玩家的硬件锁定。但法律风险仍存：美国法院曾认定逆向工程构建模拟器属合理使用，然而绕过 DRM 或分发受版权保护的固件/密钥可能违反 DMCA，因此该项目的实际可用性与合法性取决于其是否涉及这些行为。

**「社区讨论」** 社区讨论中，有评论者担忧此类逆向工程会推动索尼、任天堂和微软进一步转向云游戏，从而限制本地运行的可能性。也有人建议对这类项目进行本地 git 克隆备份，以防因法律威胁而被下架，并引用了 Yuzu 和 Ryujinx 的先例。此外，还有评论以调侃口吻询问是否能在首发日获得 GTA 6 的 PC 移植版。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://latestintech.com/anyps5-project-ps5-games-pc-port/">AnyPS 5 Project : Impressive PS 5 -to- PC Port , No Emulator</a></li>
<li><a href="https://www.youtube.com/watch?v=Go_h0Y7BUm0">Modders Used AI to Port the PS 5 to PC … It&#x27;s 80% Done - YouTube</a></li>
<li><a href="https://en.3dmgame.com/news/4897">Open-source project AnyPS 5 attempts to run PS 5 games on Windows...</a></li>
<li><a href="https://aliteq.com/is-game-emulation-legal">Is emulation legal? What US emulation laws and court cases ...</a></li>
<li><a href="https://www.twoaveragegamers.com/are-emulators-legal-2026/">Are Emulators Legal? Everything You Need to Know in 2026</a></li>
<li><a href="https://expertbeacon.com/is-ps5-emulator-illegal/">Is Ps5 Emulator Illegal? - ExpertBeacon</a></li>

</ul>
</details>

**标签**: `#reverse-engineering`, `#game-console`, `#binary-compatibility`, `#systems-programming`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [2026 年诺贝尔物理学奖授予冰立方构想者弗朗西斯·哈尔岑](https://www.nobelprize.org/prizes/physics/2026/) ⭐️ 8.0/10

瑞典皇家科学院 10 月 6 日宣布，将 2026 年诺贝尔物理学奖授予美国威斯康星大学麦迪逊分校的弗朗西斯·哈尔岑，以表彰他对冰立方中微子观测站的决定性贡献以及发现天体物理起源的高能中微子。哈尔岑于 1988 年提出在南极冰层中探测中微子的构想，并领导了这座位于南极、体积达一立方公里的探测器的建设。其探测机制是中微子转化为带电粒子后，由带电粒子在介质中超过该介质光速时产生的切伦科夫辐射被记录下来。中微子不带电荷、质量近零，只参与弱核力和引力相互作用，极难探测，因此这一装置被视为大型科学仪器的里程碑。

hackernews · solarist · 10月6日 09:48 · [社区讨论](https://news.ycombinator.com/item?id=49976265)

**「背景」** 中微子是核反应（包括恒星内部、超新星和放射性衰变）产生的基本粒子，不带电荷、质量极小，只通过弱核力和引力与其他物质作用，因此极难探测。弗朗西斯·哈尔岑意识到南极冰层可作为探测介质，提出用一立方公里冰体并布设光传感器来追踪中微子，这一构想最终发展为冰立方中微子观测站。

**「影响」** 该奖项确认了冰立方作为高能中微子天文学核心设施的地位，其约 70 万个 100 GeV 至 1 PeV 的中微子数据（纯度超过 99%）以及发现能量通量可与河外高能伽马射线相当甚至更高的 PeV 级河外中微子，为后续多信使天文学和暗物质研究提供了关键观测基础。

**「社区讨论」** 有评论者详细解释了中微子为何被称为“幽灵粒子”以及探测之难，并指出切伦科夫辐射之所以可能，是因为介质中的光速低于真空光速。曾参与 2009 年南极建设的 southpolesteve 表示自己只承担了极小部分工作，并打趣说当时并未看到任何中微子；dekhn 则提到有同事专程飞往南极点，只为给数据处理系统安装 Debian。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nobelprize.org/prizes/physics/">NobelPrize .org</a></li>
<li><a href="https://www.theguardian.com/science/2026/oct/06/nobel-prize-in-physics-francis-halzen-south-pole-neutrinos-icecube-detector">Nobel prize in physics goes to Francis Halzen for... | The Guardian</a></li>
<li><a href="https://icecube.wisc.edu/">IceCube Neutrino Observatory</a></li>
<li><a href="https://icecube.wisc.edu/science/research/">Research Highlights – IceCube Nobel Prize in Physics 2026 Scientific Background Latest results from the IceCube Neutrino Observatory Nobel prize in physics goes to Francis Halzen for south pole ... 2026 Nobel Prize in Physics awarded to Francis Halzen ...</a></li>

</ul>
</details>

**标签**: `#physics`, `#scientific-computing`, `#instrumentation`, `#neutrino-detection`, `#research`

---

<a id="item-tech-news-6"></a>
### [Polars 2.0 正式发布](https://pola.rs/posts/release-polars-2/) ⭐️ 8.0/10

Polars 2.0 已正式发布，这是这一广泛使用的 Rust/Python DataFrame 库的一次重大版本更新。该消息由项目官方站点 pola.rs 公布，并通过 Lobste.rs 上的讨论链接传播。由于目前可获取的内容仅为指向评论页面的链接，缺少具体的技术细节、变更日志或性能基准数据，因此尚无法从现有信息中核实此次大版本升级的具体改动与影响范围。

rss · Lobsters · 10月6日 14:30

**「背景」** Polars 是一个用 Rust 编写、同时提供 Python 接口的 DataFrame 库，在 Python/Rust 数据生态中被广泛使用。Polars 2.0 的正式发布此前已有铺垫：官方在 2026 年 9 月 2 日发布了首个 2.0 候选版本，并预告正式版将在随后几周内推出。官方当时表示并不打算把 2.0 做成一次大规模功能发布，甚至希望升级过程对用户而言“平淡无奇”，而正式发布公告称该版本仍包含不少值得关注的亮点。

**「影响」** Polars 2.0 的发布将直接影响使用 Python 和 Rust 进行数据处理与分析的开发者，其重新设计的 API、通过 cuDF 集成实现的 GPU 加速以及流式处理改进，可能改变日常数据工作流的性能表现。不过，由于所提供的内容仅为评论链接，缺少官方变更日志、基准测试和兼容性说明，上述影响尚无法从原始条目中得到完整验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pola.rs/posts/release-polars-2/">Polars — Release of Polars 2.0</a></li>
<li><a href="https://pola.rs/posts/announcing-polars-2/">Polars — Pre-release of Polars 2.0</a></li>
<li><a href="https://pyrastra.com/posts/polars-2-dataframe-api-2026/">Polars 2.0: What the New DataFrame API Means for Python Data ...</a></li>
<li><a href="https://pola.rs/posts/release-polars-2/">Polars — Release of Polars 2.0</a></li>
<li><a href="https://pola.rs/">Polars — DataFrames for the new era</a></li>

</ul>
</details>

**标签**: `#polars`, `#dataframes`, `#rust`, `#python`, `#open-source`

---

<a id="item-tech-news-7"></a>
### [合成先验训练字节级 Transformer 实现语言上下文学习](https://www.reddit.com/r/MachineLearning/comments/1wyzhdw/learning_to_learn_a_language_incontext_learning/) ⭐️ 8.0/10

一项新论文《Learning to Learn a Language》将先验拟合网络（TabPFN 背后的思路）扩展到结构化序列，提出一种语言先验：每条训练序列都来自随机采样的循环因果模型，因此每个样本都是一种新的合成“语言”。一个仅在这些合成序列上训练的 300M 参数字节级 Transformer，在权重冻结的情况下能够对真实语言进行上下文学习：在维基百科文本上，其下一字节预测随阅读量增加而改善，在英语、中文、印地语、阿拉伯语、日语和韩语六种语言中均从 8 bits per byte 降至一百万字节后的 0.9–2.4。该模型还能完全在上下文中学会计数、比较数字、近似加法，以及预测素数或 Kolakoski 序列等确定性序列。作者指出，该模型在文本上的表现仍远逊于用数万亿 token 训练的经典语言模型，因为它在测试时最多只看到一百万字节的语言数据；其核心发现是，在上下文中学习语言的能力可以来自合成的非语言先验。

reddit · r/MachineLearning · /u/cbl007 · 10月6日 10:50

**「背景」** 先验拟合网络（Prior-Fitted Networks, PFN）是一类在从先验分布中采样的合成数据集上训练的神经网络，能够通过上下文学习直接近似后验预测分布，从而在单次前向传播中完成贝叶斯预测。这一思路最早由 2022 年提出的 TabPFN 应用于表格数据的分类与回归，其采用 Transformer 架构，主要面向中小规模数据集。本文将该范式从表格数据扩展到结构化序列，提出先验拟合语言模型（PFLM），其训练序列全部由随机采样的循环结构因果模型生成，构成一种合成的非语言先验。

**「影响」** 对语言建模研究者而言，该工作表明仅用合成非语言先验预训练的冻结权重模型也能在上下文中学习真实语言，为无需微调的上下文学习提供了新路径；但作者明确指出其在文本上的表现仍远逊于用数万亿 token 训练的经典语言模型，且测试时最多只见到一百万字节。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TabPFN">TabPFN - Wikipedia</a></li>
<li><a href="https://github.com/Cloudy1225/Awesome-Prior-Data-Fitted-Networks">GitHub - Cloudy1225/Awesome- Prior -Data- Fitted - Networks ...</a></li>
<li><a href="https://www.emergentmind.com/topics/prior-data-fitted-transformer-network-pfn">Prior -Data Fitted Transformer Network</a></li>
<li><a href="https://arxiv.org/abs/2610.05879">[2610.05879] Learning to Learn a Language - arXiv.org</a></li>
<li><a href="https://huggingface.co/papers/2610.05879">Paper page - Learning to Learn a Language</a></li>
<li><a href="https://arxiv.org/abs/2610.05879">[2610.05879] Learning to Learn a Language</a></li>

</ul>
</details>

**标签**: `#in-context learning`, `#prior-fitted networks`, `#language modeling`, `#meta-learning`, `#synthetic data`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [派拉蒙天舞完成 1100 亿美元收购华纳兄弟探索](https://arstechnica.com/tech-policy/2026/10/paramount-completes-111b-warner-merger-creating-skydance-behemoth/) ⭐️ 8.0/10

派拉蒙天舞公司于 10 月 6 日宣布完成对华纳兄弟探索公司价值约 1100 亿美元（约合 7383.13 亿元人民币）的收购，这是美国传媒行业历史上规模最大的并购交易之一。新公司简称天舞，旗下将包括派拉蒙和华纳兄弟的影视制片厂、Paramount+与 HBO Max 流媒体服务，以及 CNN 和 CBS 新闻部。

hackernews · Mgtyalx · 10月6日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=49983703)

**「背景」** 华纳兄弟探索公司由华纳媒体与探索公司于 2022 年合并而成，而华纳媒体此前曾属 AT&amp;T；派拉蒙天舞则源于 2025 年派拉蒙全球与天舞传媒的合并。据 IT 之家报道，此次交易于 10 月 6 日宣布完成，合并后公司简称“天舞”，旗下将包括派拉蒙和华纳兄弟的影视制片厂、Paramount+与 HBO Max 流媒体服务，以及 CNN 和 CBS 新闻部。

**「影响」** 合并后，新公司同时拥有派拉蒙与华纳兄弟的影视制片厂、Paramount+ 和 HBO Max 等流媒体平台，以及 CNN 和 CBS 新闻部，美国影视制作与新闻供给进一步集中于少数企业手中。

**标签**: `#media`, `#mergers-and-acquisitions`, `#antitrust`, `#corporate-consolidation`, `#entertainment`

---

<a id="item-finance-news-2"></a>
### [SpaceX 据报拟募资 400 亿美元采购英伟达芯片](https://www.ithome.com/1/010/134.htm) ⭐️ 8.0/10

据《金融时报》报道，SpaceX 计划募资 400 亿美元，其中约 100 亿美元来自银行贷款、300 亿美元来自投资级债券，由阿波罗全球管理牵头，资金用于采购英伟达 AI 芯片，交易预计 2027 年完成。上述内容来自知情人士，尚未得到公司确认。

rss · IT HOME · 10月6日 23:24

**「背景」** SpaceX 在 6 月完成 860 亿美元首次公开募股后获得 BBB 投资级信用评级（投资级中倒数第二档），随后发行 250 亿美元高等级债券，但债券价格此后下跌；其 2056 年到期债券目前交易价约为面值的 85 美分，收益率比美国国债高约 2.27 个百分点。

**「影响」** 若融资落地，SpaceX 与英伟达的合作将加深，并进一步扩大市场为 AI 数据中心和芯片筹措资金的规模；同时，保险与养老基金因该投资级评级可购买这批债券，但此前投资者曾因信息披露有限而对 SpaceX 债券持谨慎态度。

**标签**: `#SpaceX`, `#Nvidia`, `#AI infrastructure`, `#corporate financing`, `#private credit`

---

<a id="item-finance-news-3"></a>
### [谷歌与 Constellation 签署 3.59GW 长期电力协议](https://www.ithome.com/1/010/063.htm) ⭐️ 8.0/10

谷歌宣布与美国能源企业 Constellation 达成总规模 3.59GW 的长期战略能源合作，其中 890MW 为新增核电容量，预计 2028 至 2032 年上线、持续 20 年，另有 2.7GW 为任意容量、持续 15 年。

rss · IT HOME · 10月6日 11:37

**「背景」** 在谷歌资金支持下，Constellation 将升级其横跨多州的 11 座核电机组，工程建设期间预计创造约 7200 个建筑工作岗位；双方还达成五年技术联盟及评估新型清洁能源发电、储能和需求响应的战略框架协议。

**「影响」** 该协议反映数据中心用电需求推动科技公司锁定长期电力供应，并可能带动相关核电升级与新建项目。

**标签**: `#energy`, `#nuclear power`, `#big tech`, `#corporate deal`, `#data centers`

---