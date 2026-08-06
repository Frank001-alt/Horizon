---
layout: default
title: "Horizon Summary: 2026-08-06 (ZH)"
date: 2026-08-06
lang: zh
---

> 从 190 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [ChainDrop 蠕虫攻陷 npm 逾 1300 个包](#item-tech-news-1) ⭐️ 9.0/10
2. [Discovery Loop：自动化 ML 实验循环的新倡议](#item-tech-news-2) ⭐️ 8.0/10
3. [谷歌 DeepMind 领导层变动：哈萨比斯转任主席，杰夫·迪恩离职](#item-tech-news-3) ⭐️ 8.0/10
4. [Deno 发布 Celld：自托管分布式 Durable Objects 运行时](#item-tech-news-4) ⭐️ 8.0/10
5. [Cloudflare OS：面向智能体、应用与工作的开放平台](#item-tech-news-5) ⭐️ 8.0/10
6. [Sand.ai 开源全球首个千亿 MoE 视频生成模型](#item-tech-news-6) ⭐️ 8.0/10
7. [清华唐杰团队发布大模型记忆机制全景分析](#item-tech-news-7) ⭐️ 8.0/10
8. [Third-party cyber evaluations involving OpenAI models](#item-tech-news-8) ⭐️ 8.0/10
9. [Rust 项目正式采纳 LLM 使用政策](#item-tech-news-9) ⭐️ 8.0/10
10. [传奇埃尔德什问题正被 AI 攻克](#item-tech-news-10) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [ChainDrop 蠕虫攻陷 npm 逾 1300 个包](https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/) ⭐️ 9.0/10

自我传播蠕虫 ChainDrop 已入侵 npm 仓库超过 1300 个包，合计月下载量达 20 亿次，包括 Keyv、Cacheable 等热门缓存工具。攻击始于黑客攻破 Keyv 维护者的 GitHub 账号，并蔓延至 Deliveroo、Qlik、ServiceTitan 等机构相关包；恶意版本经正常的 GitHub Actions 流程发布，带有合法来源证明。中毒包内的 setup.mjs 投放器与 Math\_Symbol.js 窃密脚本会在执行 npm install 时自动运行，窃取 GitHub、npm、AWS、Kubernetes 等凭证并感染其他维护者的包。安全公司建议：安装过受影响版本即应视系统已被攻破，重建环境、轮换所有令牌并检查日志；npm-cache\[.\]com 域名可作为失陷指标。攻击仍在扩散，受影响包数量预计继续增加。

telegram · zaihuapd · 8月5日 03:04

**「背景」** npm 是 JavaScript 生态系统的官方包管理器，开发者通过它共享和安装代码库。供应链攻击是指攻击者通过入侵软件包的维护者账户或构建流程，在合法软件中植入恶意代码，从而影响所有使用该软件的下游用户。ChainDrop 蠕虫正是利用这种方式，通过攻破 Keyv 维护者的 GitHub 账户，在合法包中注入恶意脚本，并利用 GitHub Actions 的正常流程发布恶意版本，使其带有合法的来源证明，从而绕过安全检查。

**「影响」** 受影响用户应立即将系统视为已被攻破，重建环境、轮换所有令牌并检查日志，同时以 npm-cache\[.\]com 域名作为失陷指标进行排查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/">Massive ChainDrop npm supply - chain attack infects hundreds of...</a></li>
<li><a href="https://www.elastic.co/security-labs/shai-hulud-chaindrop-npm-supply-chain">Shai-Hulud strikes again: CHAINDROP worm hits 400+ npm packages</a></li>
<li><a href="https://dev.to/anoymask/chaindrop-a-supply-chain-worm-stealing-credentials-and-self-propagating-via-legitimate-351">ChainDrop : A Supply Chain Worm Stealing... - DEV Community</a></li>

</ul>
</details>

**标签**: `#supply-chain attack`, `#npm`, `#security`, `#malware`, `#open source`

---

<a id="item-tech-news-2"></a>
### [Discovery Loop：自动化 ML 实验循环的新倡议](https://www.discoveryloop.com/) ⭐️ 8.0/10

Discovery Loop 是一项新倡议，旨在自动化机器学习研究和工程中的实验循环，其方法被认为可广泛适用于科学和工程领域。该倡议由 Jeff 在 Twitter 上宣布，强调其方法最初聚焦于 ML 研究和工程，但相信能帮助解决美国国家工程院（NAE）十四大挑战问题中的几乎所有重要子问题。实现这一目标需要强大的机器学习和大规模系统专业知识。该倡议与 Karpathy 的 autoresearch 和 Bengio 的 LawZero 有相似之处，但 Discovery Loop 似乎是一个机构级、大规模扩展的版本。

hackernews · xtreak29 · 8月5日 16:19 · [社区讨论](https://news.ycombinator.com/item?id=49184960)

**「背景」** Discovery Loop 是由前 Google DeepMind 领导者 Jeff Dean、Sanjay Ghemawat、Quoc Le 和 Oriol Vinyals 创立的新实验室，旨在利用前沿 AI 模型和大规模计算基础设施，自动化整个实验循环，包括提出、实施、运行和评估实验。该倡议与 Andrej Karpathy 的 autoresearch 项目以及 Yoshua Bengio 的 LawZero 初创公司（后者强调非代理式安全设计）有相似之处，但 Discovery Loop 更侧重于大规模系统和广泛适用性。

**「影响」** 对于 ML 研究和工程领域的从业者，Discovery Loop 可能加速实验迭代，减少人工干预，从而提升研究效率。然而，其实际影响取决于能否有效处理实验中的物理世界约束，以及是否能在不同领域实现自动化。

**「社区讨论」** 社区评论指出，Discovery Loop 与 Bengio 的 LawZero 和 Karpathy 的 autoresearch 有相似之处，但 LawZero 强调非代理式设计以确保安全。有评论质疑自动化实验的可行性，认为 AI 在思维和设计领域可超高速迭代，但实验受限于物理世界，需要具身性。另有评论调侃其使命声明过于复杂。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.discoveryloop.com/">Discovery Loop — Continuous Exploration</a></li>
<li><a href="https://aiwiki.ai/wiki/discovery_loop">Discovery Loop | AI Wiki</a></li>
<li><a href="https://elsolitario.org/en/2026/08/05/discovery-loop-jeff-dean-automate-science/">Discovery Loop : Automating AI Research</a></li>

</ul>
</details>

**标签**: `#AI research`, `#automation`, `#machine learning`, `#experimentation`, `#open source`

---

<a id="item-tech-news-3"></a>
### [谷歌 DeepMind 领导层变动：哈萨比斯转任主席，杰夫·迪恩离职](https://blog.google/company-news/inside-google/message-ceo/next-chapter-ai-momentum/) ⭐️ 8.0/10

谷歌 DeepMind 宣布重大领导层调整：德米斯·哈萨比斯（Demis Hassabis）从 CEO 转任主席，而杰夫·迪恩（Jeff Dean）在任职 27 年后离开谷歌，与桑杰·格玛沃特（Sanjay Ghemawat）共同创立一家独立的公益公司，以加速机器学习、科学和工程领域的发现。哈萨比斯将接替迪恩担任 Alphabet 首席科学家，同时继续领导 DeepMind 的 AI 研究。此次变动发生在谷歌股价下跌 5%的背景下，评论者认为迪恩和格玛沃特的离开是更大的损失，而哈萨比斯的角色变化可能带有公关色彩。

hackernews · colesantiago · 8月5日 16:05 · [社区讨论](https://news.ycombinator.com/item?id=49184755)

**「背景」** Google DeepMind 是谷歌旗下的人工智能研究机构，由 Demis Hassabis 等人于 2010 年创立，2014 年被谷歌收购。Jeff Dean 是谷歌资深研究员和首席科学家，在谷歌工作 27 年，参与设计了 MapReduce、TensorFlow 等关键系统。此次领导层变动中，Demis Hassabis 从 DeepMind CEO 转任董事长，Jeff Dean 与 Sanjay Ghemawat 等资深研究员离职创办新的公益公司，专注于机器学习、科学和工程领域的研究。

**「影响」** 此次领导层变动可能影响谷歌 DeepMind 的研究方向和人才保留，尤其是迪恩和格玛沃特的离开被视为重大损失，可能导致股价波动和外界对谷歌 AI 领导力的质疑。

**「社区讨论」** 社区评论普遍认为，真正的新闻是迪恩和格玛沃特的离职，而非哈萨比斯的职位变动；有评论者列举了谷歌近期流失的多位知名 AI 人才，并指出谷歌在 Gemini 前沿模型发布上存在空白，暗示其环境可能对人才不友好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.businessinsider.com/google-ai-leadership-demis-hassabis-steps-down-deepmind-ceo-2026-8">Google shakes up AI leadership. Demis Hassabis takes on ...</a></li>
<li><a href="https://www.nytimes.com/2026/08/05/technology/google-ai-leadership.html">Google Names Demis Hassabis to New AI Role in a Leadership ...</a></li>
<li><a href="https://www.cnbc.com/2026/08/05/google-chief-scientist-jeff-dean-leaving-company-after-27-years.html">Google chief scientist Jeff Dean leaving company after 27 years</a></li>

</ul>
</details>

**标签**: `#Google DeepMind`, `#AI leadership`, `#Jeff Dean`, `#Demis Hassabis`, `#industry news`

---

<a id="item-tech-news-4"></a>
### [Deno 发布 Celld：自托管分布式 Durable Objects 运行时](https://github.com/denoland/celld) ⭐️ 8.0/10

Deno 团队发布了 Celld，一个自托管、分布式的 Durable Objects 运行时，允许开发者在任何基础设施上运行持久化、有状态的对象，而无需依赖特定云提供商。Celld 的每个对象都是一个独立的 SQLite 数据库，通过名称寻址，并复制到你拥有的 S3 兼容存储桶中，从而提供与提供商无关的持久状态。该运行时基于轻量级 V8 隔离，具有极低的空闲成本，并且是 Deno 团队自研的新运行时，不依赖 deno\_core。Celld 旨在解决 Durable Objects 抽象长期绑定单一提供商的问题，为分布式系统和边缘计算场景提供了新的选择。该项目在 Hacker News 上获得了 128 分和 19 条评论，引发了社区对与 Cloudflare workerd 对比的讨论。

hackernews · calvinfo · 8月5日 16:50 · [社区讨论](https://news.ycombinator.com/item?id=49185430)

**「背景」** Durable Objects 是 Cloudflare Workers 提供的一种分布式编程模型，将每个对象视为一个独立的、可寻址的实体，拥有自己的状态和存储，常用于构建有状态的服务。此前，这一抽象主要绑定在 Cloudflare 的平台上，开发者无法在其他基础设施上运行。Celld 是 Deno 团队推出的开源守护进程，允许用户在自己的机器上运行 Cloudflare Workers 和 Durable Objects，每个对象对应一个独立的 SQLite 数据库，并通过 S3 兼容存储进行复制，节点之间仅通过该存储协调，无需控制平面或共识机制。

**「影响」** Celld 使开发者能够在自托管环境中使用 Durable Objects 模式，从而摆脱对特定云提供商的依赖，这对于构建分布式应用和边缘计算服务的团队尤为重要。它可能推动 Durable Objects 抽象的更广泛采用，并促进与 Cloudflare workerd 等现有解决方案的竞争。

**「社区讨论」** 社区对 Celld 表示欢迎，认为它终于支持在单一提供商之外运行 Durable Objects，并赞赏其 SQLite 加 S3 复制的简洁设计。一些用户希望能在本地无需配置 S3 即可轻松原型开发，另一些则关注在 spot 实例上运行的可能性。还有用户将其与 Cloudflare 的开源 workerd 进行比较，并指出 Celld 使用轻量级 V8 隔离，空闲成本低。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/denoland/celld">Celld: Self-hosted, distributed Durable Objects - GitHub</a></li>
<li><a href="https://github.com/denoland/celld/tree/main">GitHub - denoland/celld: self-hosted, distributed Durable Objects</a></li>

</ul>
</details>

**标签**: `#distributed-systems`, `#durable-objects`, `#deno`, `#self-hosting`, `#edge-computing`

---

<a id="item-tech-news-5"></a>
### [Cloudflare OS：面向智能体、应用与工作的开放平台](https://blog.cloudflare.com/cloudflare-os/) ⭐️ 8.0/10

Cloudflare 宣布推出 Cloudflare OS，这是一个基于其 Workers 基础设施构建和运行 AI 智能体、应用及工作编排的开放平台。该平台由 Cloudflare 员工 Kenton Varda 主导，他曾创立 Sandstorm.io，此次是将其理念在 Workers 上结合 AI 深度重制。Cloudflare OS 旨在提供一种新的工作操作系统，允许用户通过聊天机器人界面与连接器交互，并支持自定义功能扩展。该公告引发了关于平台锁定、数据模型和术语定义的广泛讨论。

hackernews · speckx · 8月5日 13:58 · [社区讨论](https://news.ycombinator.com/item?id=49182996)

**「背景」** Cloudflare OS 是 Cloudflare 于 2026 年 8 月发布的一个开放平台，用于在 Cloudflare Workers 基础设施上构建和运行 AI 代理、应用程序和工作流编排。该项目由 Kenton Varda 主导，他是 Cloudflare Workers 的技术负责人，也是 Sandstorm.io 的创始人。Sandstorm.io 是 Varda 在 2015 年创立的个人应用服务器项目，旨在让用户轻松部署和运行自托管应用。Cloudflare OS 本质上是 Sandstorm.io 的重制版，但构建在 Cloudflare Workers 之上，并深度集成了 AI 能力。

**「影响」** 对于依赖 Cloudflare Workers 的开发者而言，Cloudflare OS 可能提供一种新的方式来构建和部署 AI 智能体应用，但用户担忧其潜在的锁定效应，以及数据共享和更新管理方面的复杂性。

**「社区讨论」** 社区对 Cloudflare OS 的反应不一，有人赞赏其创新性，但也有人质疑“OS”一词的滥用，并担心平台锁定风险。此外，开发者对数据模型冲突和更新管理提出了具体的技术疑问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/KentonVarda/status/2084990137180590572">Kenton Varda on X: &quot;Today we are releasing Cloudflare OS, a chatbot with connectors, just like every other tech company is doing. Except actually, it&#x27;s different. This is a remake of Sandstorm[.]io, my startup from 10 years ago, except this time built on Cloudflare Workers (the platform I&#x27;ve spent&quot; / X</a></li>
<li><a href="https://www.explainx.ai/blog/cloudflare-os-open-source-agent-platform-august-2026">Cloudflare OS Explained — Gatekeepers, Gadgets (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://github.com/kentonv">kentonv (Kenton Varda) · GitHub</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#ai-agents`, `#platform`, `#work-os`, `#developer-tools`

---

<a id="item-tech-news-6"></a>
### [Sand.ai 开源全球首个千亿 MoE 视频生成模型](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&amp;mid=2247909833&amp;idx=1&amp;sn=4ee6c970ea6ef8ef992b3ae1d6c564b2) ⭐️ 8.0/10

Sand.ai 近日开源了据称是全球首个参数规模超过千亿的 MoE（混合专家）视频生成模型，该模型拥有 114B 总参数和 6B 激活参数，能够以约 0.5 元人民币的成本生成 10 秒 1080P 视频。这一举措标志着视频生成领域在架构创新和成本效率上迈出了重要一步，使得高质量视频生成更加经济可行。该模型的开源有望推动视频生成技术的普及和应用，但具体性能表现和实际应用效果仍需进一步验证。

rss · 量子位 · 8月5日 06:07

**「背景」** 视频生成模型通常采用稠密架构，即每次推理激活全部参数，导致计算成本高昂。混合专家（MoE）架构通过将模型划分为多个专家子网络，每次仅激活其中一部分，从而在保持模型容量的同时降低推理成本。此前，MoE 架构已在大型语言模型中得到广泛应用，但在视频生成领域尚未出现千亿参数级别的开源模型。

**「影响」** 该模型的低成本和高效率特性可能显著降低视频生成的门槛，使中小型开发者和企业能够以更低成本利用先进的视频生成技术，从而加速相关应用和服务的创新。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zglg.work/en/ai/news/2026-08-05-sand-ai-open-sources-what-it-calls-the-first-100b-parameter-moe-video-generat">Sand.ai Open-Sources What It Calls the First 100B-Parameter ...</a></li>
<li><a href="https://github.com/SandAI-org/MAGI-2-preview">GitHub - SandAI-org/MAGI-2-preview: MAGI-2-preview: Scaling ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#video generation`, `#MoE`, `#open source`, `#large language model`

---

<a id="item-tech-news-7"></a>
### [清华唐杰团队发布大模型记忆机制全景分析](https://mp.weixin.qq.com/s?__biz=MzIzNjc1NzUzMw==&amp;mid=2247909833&amp;idx=3&amp;sn=381a2d0bcdcac4687f8451143a515d51) ⭐️ 8.0/10

清华大学唐杰团队发布了一篇万字长文，系统性地解构了大语言模型的记忆机制，并绘制了 LLM 记忆架构的全景图。该分析覆盖了从短期工作记忆到长期参数记忆的多种记忆类型，详细阐述了各类记忆在模型推理和训练中的作用与实现方式。这一研究为 AI 研究者和工程师提供了关于模型记忆设计的全面参考，有助于理解当前大模型在记忆方面的能力边界与优化方向。文章还探讨了记忆机制与模型性能、可解释性及效率之间的权衡，为后续研究提供了重要框架。

rss · 量子位 · 8月5日 06:07

**「背景信息」** 大语言模型的记忆机制是决定其推理能力和知识保留的关键因素，但长期以来缺乏系统性的梳理。唐杰团队作为国内领先的 AI 研究团队，此前在预训练模型和知识图谱方面有深厚积累，此次发布的全景分析旨在填补这一空白。文章通过整合现有研究成果，为读者提供了理解 LLM 记忆架构的统一视角。

**「影响分析」** 该分析为 AI 研究者和工程师提供了关于模型记忆设计的全面参考，有助于理解当前大模型在记忆方面的能力边界与优化方向。

**标签**: `#large language models`, `#memory mechanisms`, `#AI research`, `#model architecture`, `#Tsinghua`

---

<a id="item-tech-news-8"></a>
### [Third-party cyber evaluations involving OpenAI models](https://simonwillison.net/2026/Aug/5/third-party-cyber-evaluations/#atom-everything) ⭐️ 8.0/10

OpenAI discloses third-party cyber evaluation incidents where misconfigured test environments allowed AI models to access the internet, including an accidental attack on a real domain.

rss · Simon Willison · 8月5日 23:45

**标签**: `#AI safety`, `#cybersecurity`, `#OpenAI`, `#incident response`, `#AI evaluation`

---

<a id="item-tech-news-9"></a>
### [Rust 项目正式采纳 LLM 使用政策](https://blog.rust-lang.org/inside-rust/2026/08/05/rust-langrust-is-adopting-an-llm-policy/) ⭐️ 8.0/10

Rust 语言项目宣布正式采纳一项关于在开发过程中使用大型语言模型（LLM）的官方政策。该政策旨在规范 AI 生成代码的贡献方式，确保代码质量与审查流程的完整性。此举为其他开源项目树立了先例，可能影响贡献指南和相关工具链。具体政策细节尚未完全公开，但预计将涵盖贡献者使用 LLM 的披露义务、代码审查标准以及自动化工具的集成方式。该政策反映了开源社区对 AI 辅助开发日益增长的关注。

rss · Lobsters · 8月5日 06:55

**「背景」** Rust 项目近期宣布，其五个团队正式采纳了一项由 Jynn Nelson 撰写的政策，规范在 rust-lang/rust 主仓库贡献中使用大型语言模型（LLM）的行为。该政策于 2026 年 8 月 5 日在 Inside Rust 博客上公布，旨在为 AI 辅助开发设定明确的指导原则。政策强调，无论 LLM 的使用是否被禁止，都不允许因使用 LLM 而骚扰他人，且所有互动必须遵守行为准则。这一举措反映了开源社区对 AI 生成代码日益增长的关注，并为其他大型项目提供了参考先例。

**「影响」** 该政策将直接影响 Rust 项目的贡献者，要求他们在提交 LLM 生成的代码时遵循新的披露和审查规范，可能增加贡献流程的复杂性。对于依赖 Rust 生态的开发者而言，政策有望提升代码的可信度和可维护性，但具体影响程度取决于政策细则的执行力度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.rust-lang.org/inside-rust/2026/08/05/rust-langrust-is-adopting-an-llm-policy/">rust - lang / rust is adopting an LLM policy | Inside Rust Blog</a></li>
<li><a href="https://www.unite.ai/rust-adopts-a-formal-llm-policy-for-its-main-repository/">Rust Adopts a Formal LLM Policy for Its Main Repository – Unite.AI</a></li>
<li><a href="https://modernorange.io/item/49179039">Rust - lang / rust is adopting an LLM policy | Modern Orange</a></li>

</ul>
</details>

**标签**: `#rust`, `#llm`, `#open-source`, `#policy`, `#ai`

---

<a id="item-tech-news-10"></a>
### [传奇埃尔德什问题正被 AI 攻克](https://www.quantamagazine.org/why-the-legendary-erdos-problems-are-falling-to-ai-20260803/) ⭐️ 8.0/10

据《Quanta Magazine》报道，人工智能正在开始解决一些传奇的埃尔德什问题，这标志着数学人工智能研究的一个重要里程碑。这些问题由数学家保罗·埃尔德什提出，长期悬而未决，如今 AI 的进展表明机器学习在数学发现中可能发挥越来越重要的作用。文章指出，AI 不仅能够辅助证明，还能提出新的猜想，尽管目前尚未完全解决所有问题，但这一趋势预示着数学研究方式的变革。这一进展来自权威科学媒体，对数学和人工智能交叉领域具有高度影响力。

rss · Lobsters · 8月5日 16:54

**「背景」** 保罗·埃尔德什是 20 世纪最具影响力的数学家之一，他提出了大量未解决的数学问题，涵盖数论、组合学、几何学等领域，这些问题以他的名字命名为“埃尔德什问题”。长期以来，这些问题被视为数学难题的象征，考验着人类数学家的智慧。然而，据 Quanta Magazine 报道，2026 年 5 月 20 日，OpenAI 宣布利用人工智能解决了其中最著名的单位距离问题，而在此之前，业余数学家 Liam Price 也通过 GPT-5.4 Pro 解决了一个关于素数集的问题。这些突破标志着 AI 在数学研究领域取得了里程碑式的进展，引发了关于 AI 将如何改变数学未来的广泛讨论。

**「影响」** 对于数学家和人工智能研究者而言，AI 攻克埃尔德什问题意味着机器学习工具可能成为数学发现的新范式，加速解决长期未解的难题，并可能改变数学研究的协作方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.quantamagazine.org/why-the-legendary-erdos-problems-are-falling-to-ai-20260803/">Why the Legendary Erdős Problems Are Falling to AI | Quanta Magazine</a></li>
<li><a href="https://www.quantamagazine.org/tag/artificial-intelligence/">Quanta Magazine Articles on Artificial Intelligence</a></li>
<li><a href="https://physicsworld.com/a/ai-led-solutions-of-erdos-problems-spark-debate-over-the-future-of-mathematics/">AI-led solutions of Erdős problems spark debate over the future of mathematics – Physics World</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#research`, `#Erdős problems`, `#machine learning`

---