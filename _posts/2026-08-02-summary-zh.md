---
layout: default
title: "Horizon Summary: 2026-08-02 (ZH)"
date: 2026-08-02
lang: zh
---

> 从 33 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [Go 1.27 交互式导览：泛型、标准库与 HTTP 变更](#item-tech-news-1) ⭐️ 8.0/10
2. [KataGo 围棋网络内部对称性研究](#item-tech-news-2) ⭐️ 8.0/10
3. [微软确认今年推出 Copilot「超级应用」](#item-tech-news-3) ⭐️ 8.0/10
4. [ByteDance 推出 Seedance 2.5：单次拍摄创作与灵活引用](#item-tech-news-4) ⭐️ 7.0/10
5. [Diátaxis：技术文档组织的实用框架](#item-tech-news-5) ⭐️ 7.0/10
6. [Lean 内核健全性缺陷 \#14576 事后分析](#item-tech-news-6) ⭐️ 7.0/10
7. [开放信争议：微软与 Anthropic 就开放权重模型立场分歧](#item-tech-news-7) ⭐️ 7.0/10
8. [OpenAI 称用内部模型攻克十个数学难题](#item-tech-news-8) ⭐️ 7.0/10
9. [AI 芯片每 9 个月翻番，2028 年底全球将达 2 亿颗](#item-tech-news-9) ⭐️ 7.0/10
10. [苹果限制漏洞报告提交以应对 AI 垃圾报告](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [高盛股票交易业务 Q2 收入跃升 72%，创纪录](#item-finance-news-1) ⭐️ 8.0/10
2. [美国将 43 家中国企业列入 UFLPA 实体清单](#item-finance-news-2) ⭐️ 8.0/10
3. [公积金条例拟修订：灵活就业者可缴存，装修和物业费可提取](#item-finance-news-3) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Go 1.27 交互式导览：泛型、标准库与 HTTP 变更](https://victoriametrics.com/blog/go-1-27/index.html) ⭐️ 8.0/10

这是由 VictoriaMetrics 团队发布的 Go 1.27 交互式导览，重点介绍了该版本的关键变化，包括泛型语法改进、标准库更新，以及一个有争议的 HTTP 响应体自动排空变更。分析认为这次发布对广泛使用的语言具有重要价值，能够帮助软件工程师了解新技术细节，但并非范式转变。评论中还提到 Go 1.27 修复了 runtime.findnull\(\) 与 Android 上 MTE 的兼容性问题，使得使用 gomobile 的应用能够在 GrapheneOS 等支持 MTE 的系统上启用该功能。由于本次来源仅提供了分析摘要，具体 API 细节和版本号未能在原文中进一步确认。

hackernews · Hixon10 · 8月2日 01:35 · [社区讨论](https://news.ycombinator.com/item?id=49140218)

**「背景」** Go 1.27 是 Go 语言继 1.26 之后的重要版本，其发布说明已于 2026 年 5 月完成整合，并进入 RC1/RC2 候选测试阶段，其中 RC2 还包含两个安全修复。该版本的主要变化包括泛型语法、标准库更新，以及一个有争议的 HTTP 响应体自动排空行为。这些改动对大量使用 Go 标准库（尤其是加密包）的开发者具有实际影响。

**「影响」** 对使用 Go 开发 HTTP 服务的开发者来说，默认自动排空响应体可能改变依赖旧行为的应用语义；对通过 gomobile 构建 Android 应用的开发者，MTE 兼容性修复为在 GrapheneOS 等系统启用 MTE 扫清了障碍。

**「社区讨论」** 评论区对 Go 标准库（尤其是 crypto 包）表示肯定，同时提醒自动排空 HTTP 响应体是一个危险的静默行为变化；也有开发者认为泛型方法签名（如 \`\(b Box\[T\]\) Map\[U any\]...\`）增加了认知负担，并批评文章使用了“LLM 式”措辞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://repojournal.com/showcase/golang/2026-05-29/go-1-27-release-notes-finalized-typeparams-deprecation-begins">Go 1.27 release notes finalized, typeparams deprecation begins · Go</a></li>
<li><a href="https://releasebot.io/updates/google/golang">Go Updates by Google - July 2026 - Releasebot</a></li>

</ul>
</details>

**标签**: `#Go`, `#programming-languages`, `#release`, `#standard-library`, `#HTTP`

---

<a id="item-tech-news-2"></a>
### [KataGo 围棋网络内部对称性研究](https://www.reddit.com/r/MachineLearning/comments/1vcrki2/how_symmetric_are_the_insides_of_a_go_network_r/) ⭐️ 8.0/10

KataGo 维护者在 Reddit r/MachineLearning 发布了一项小规模神经网络的解释性研究，考察围棋 AI 内部表征对旋转/反射对称性的利用程度。这些模型并未在架构上强制对称性，仅依靠训练时对每个批次进行随机 8 倍空间方向的数据增强；研究试图弄清超人类水平网络是将棋盘表示学习为方向无关，还是按方向分别记忆。研究发现之一出乎预料，但原文未透露具体内容；文章还说明其撰写主要由 AI 完成，但有人类详细指导和反馈，且附有可复现代码。这项研究面向 ML 圈外读者，属于解释性研究的“沧海一粟”，而非范式转变。

reddit · r/MachineLearning · /u/icosaplex · 8月1日 16:18

**「研究背景」** KataGo 是由维护者 lightvector 开发的开源围棋程序，通过神经网络的自我对弈和训练达到超人水平（tool-1-2 展示了其 GTP 引擎与安装方式，tool-1-1 也提供了其训练得到的网络文件）。围棋规则对棋盘旋转和镜像完全对称，但 KataGo 的训练并不在模型结构上强制这种对称，而是通过每批数据随机施加 8 种旋转/翻转的数据增强来处理。这项研究正是利用该模型的内部表示，检验神经网络在多大程度上自动学到与朝向无关的“对称”概念，而不是为每个朝向分别记忆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://katagotraining.org/extra_networks/">KataGo - Extra Networks</a></li>
<li><a href="https://github.com/lightvector/KataGo">GitHub - lightvector/ KataGo : GTP engine and self-play learning in Go</a></li>
<li><a href="https://gomagic.org/katago-leela-zero-go-ai/">KataGo , Leela Zero — Installing Software for AI Go Game Review</a></li>

</ul>
</details>

**标签**: `#interpretability`, `#neural networks`, `#Go`, `#symmetry`, `#deep learning`

---

<a id="item-tech-news-3"></a>
### [微软确认今年推出 Copilot「超级应用」](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 8.0/10

微软 CEO 萨蒂亚·纳德拉在周三的财报电话会议上确认，公司计划于今年推出一款 AI「超级应用」，将 Copilot 的聊天、编程和智能体能力整合到一起，同时覆盖消费者和商用场景。纳德拉表示，Copilot 正从聊天工具演进到 Cowork 再到 Autopilot，本季度将把这些体验（包括代码功能）合并进该应用。此前《财富》报道微软在打造融合 Copilot 聊天机器人、GitHub Copilot、Copilot Cowork 和 Autopilot 系统的应用，而 OpenAI 近期也推出了整合 ChatGPT 与 Codex 的 ChatGPT Work 应用。微软上季度营收增至 900 亿美元，主要由 AI 与云业务推动。

telegram · zaihuapd · 8月1日 13:18

**「背景」** Copilot 是微软的 AI 助手，此前以聊天、编程（GitHub Copilot）、Cowork 和 Autopilot 等分散形态提供给消费者和商业用户。微软 CEO 萨蒂亚·纳德拉在 7 月 29 日财报电话会议上确认，公司计划在今年晚些时候把这些能力整合为一款独立的“超级应用”。此前有报道称微软正在打造这样一款融合多种 AI 功能的应用，OpenAI 也已推出整合 ChatGPT 与 Codex 的 ChatGPT Work 应用。

**「影响」** 对于现有及潜在的 Copilot 用户与开发者，若该超级应用如期推出，聊天、代码补全和智能体工作流将统一到一个入口，可能降低在不同工具间切换的成本并加速 AI 编程与自动化流程；但微软尚未公布具体上线时间与功能兼容性，正式影响仍取决于实际发布后的落地情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsforum.com/windows-news.4/microsoft-copilot-super-app-to-unite-chat-code-and-agents-in-2026.440876/">Microsoft Copilot Super App to Unite Chat, Code and Agents in 2026</a></li>
<li><a href="https://www.digitaltrends.com/computing/microsoft-is-making-a-copilot-super-app-to-end-your-ai-app-juggling/">Microsoft is making a Copilot super app to end your AI app juggling</a></li>
<li><a href="https://valueaddvc.com/pulse/microsoft-copilot-super-app-announcement-2026">Nadella Confirms Microsoft Copilot &#x27;Super App&#x27; Plan</a></li>
<li><a href="https://www.analyticsinsight.net/news/microsoft-confirms-copilot-super-app-launch-this-year-combining-chat-coding-ai-agents">Microsoft Confirms Copilot ‘Super App’ Launch this Year ...</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Copilot`, `#AI super app`, `#AI assistants`, `#software engineering`

---

<a id="item-tech-news-4"></a>
### [ByteDance 推出 Seedance 2.5：单次拍摄创作与灵活引用](https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5) ⭐️ 7.0/10

字节跳动（ByteDance）正式发布新一代 AI 视频生成模型 Seedance 2.5，重点增强了“一次性拍摄创作”（one-take creation）和“灵活引用”（flexible referencing）能力。该发布正值 AI 视频生成赛道快速演进，社区讨论活跃，对创作者和 AI/ML 从业者具有实际意义。公告来自 Seedance 官网博客，但具体技术参数和测试数据在现有材料中尚未披露。

hackernews · njaremko · 8月1日 20:45 · [社区讨论](https://news.ycombinator.com/item?id=49138302)

**「背景」** Seedance 是字节跳动推出的 AI 视频生成模型系列，Seedance 2.0 曾被广泛视为 AI 视频领域的重大突破。2026 年 7 月，字节跳动正式发布 Seedance 2.5，成为该系列的最新版本，能够生成最长 30 秒的高质量视频片段。

**「影响」** Seedance 2.5 使视频创作者能够单次生成 30 秒的完整高质量音视频片段，并通过更强的镜头转换和场景变化支持广告、产品演示和多镜头叙事等连续叙事场景；对内容创作者而言，这降低了生成稳定、长时长视频所需的多次生成与后期拼接成本。

**「社区讨论」** 评论者普遍认可 Seedance 2.5 的生成质量，但指出其方向更侧重动作/高特效类文生视频，与美国电影制作者希望保留演员表演细节的视频到视频（v2v）需求不一致；也有用户认为最新模型使用成本高，并预告 MiniMax H3 即将开源，可能会是更低成本、更高控制性的替代选择。另有声音质疑音视图生成工具弊大于利，认为其造成伤害多于正面用途。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://technode.com/2026/07/31/bytedance-launches-seedance-2-5-video-generation-model/">ByteDance launches Seedance 2.5 video-generation model · TechNode</a></li>
<li><a href="https://www.theinformation.com/briefings/bytedance-unveils-seedance-2-5-video-model">ByteDance Unveils Seedance 2.5 Video Model — The Information</a></li>
<li><a href="https://www.seedance.tv/seedance-2-5">Seedance 2.5 AI Video Generator — 30s 4K Model Guide</a></li>
<li><a href="https://seeddance.ai/seedance-2-5">Seedance 2.5 — 30s One-Take AI Video with Multimodal ...</a></li>

</ul>
</details>

**标签**: `#video generation`, `#AI models`, `#ByteDance`, `#machine learning`, `#generative media`

---

<a id="item-tech-news-5"></a>
### [Diátaxis：技术文档组织的实用框架](https://diataxis.fr/) ⭐️ 7.0/10

Diátaxis 是一个将技术文档划分为教程、操作指南、参考和解释四类的写作框架，其官网 diataxis.fr 近期受到关注。框架作者 DanieleProcida 正在推进多语言翻译，并已在 readthedocs 提供部分译文预览。社区成员还发布了基于 Diátaxis 的 LLM 技能（alpha 版），用于辅助生成初版文档。有团队在大型代码库交接文档中实际使用后认为，虽然前期规划页面标题需要投入精力，但写作时对内容和“语气”的定位非常清晰，能够显著提升文档质量。

hackernews · ryanseys · 8月1日 20:33 · [社区讨论](https://news.ycombinator.com/item?id=49138188)

**「背景」** Diátaxis 是由 Daniele Procida 提出的一套系统性技术文档编写框架，其名称来自古希腊语 διάταξις，意为“跨越”（dia）与“排列”（taxis）。该框架的核心思路是通过清晰、逻辑化的方式组织文档，以满足不同用户在不同场景下的需求。它常被用于改善文档结构，让教程、操作指南、参考说明和解释性内容各得其所。

**「影响」** 采用 Diátaxis 框架的文档团队可以将技术文档按教程、操作指南、技术参考和解释四类组织，围绕用户需求而非作者视角来提升文档的清晰度和可用性；社区反馈表明，该框架已在大型代码库交接等实际场景中成功应用，并已有翻译项目和 LLM 技能等配套工具出现，体现出切实的工程采纳基础。

**「社区讨论」** 评论中，有开发者分享团队用 Diátaxis 完成复杂代码库交接文档并获得良好体验，也有人半开玩笑地警告“一旦读过就再也无法容忍现有文档的混乱”。还有用户表示在“vibe coding”时直接让 LLM 按 Diátaxis 生成初稿很方便，相关 LLM 技能项目已开源并征询反馈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@arshika/improving-technical-documentation-with-the-di%C3%A1taxis-framework-322c078f97f0">Improving Technical Documentation with the Diátaxis Framework</a></li>
<li><a href="https://tudat-developer-new.readthedocs.io/en/latest/reference/documentation-modes/">Diátaxis Framework - Tudat Developer</a></li>
<li><a href="https://diataxis.fr/">Diátaxis</a></li>
<li><a href="https://diataxis.fr/">Diátaxis</a></li>
<li><a href="https://documentation.ai/blog/diataxis-framework">Diátaxis Framework: Organize Documentation for Users, Not Authors</a></li>
<li><a href="https://diataxis-translated.readthedocs.io/">Diátaxis ¶</a></li>

</ul>
</details>

**标签**: `#documentation`, `#technical-writing`, `#software-engineering`, `#diataxis`, `#developer-tools`

---

<a id="item-tech-news-6"></a>
### [Lean 内核健全性缺陷 \#14576 事后分析](https://leodemoura.github.io/blog/2026-8-1-postmortem-for-kernel-soundness-bug-14576/) ⭐️ 7.0/10

2026 年 8 月 1 日，Lean 定理证明器主要作者 Leo de Moura 发布了针对内核健全性缺陷 \#14576 的事后分析，探讨了该缺陷的成因及其对形式化验证社区的影响。该缺陷允许构造破坏内核健全性的证明，但评论指出，若使用独立内核进行交叉验证，则必须同时利用两个不同实现中的两个不同缺陷才能实际利用，因此依赖这一做法的用户需要确保两个版本都是最新的。社区强调，验证结果应被视为极强而非绝对的保证，并提到即使是 Rust 这类更简单的类型检查器偶尔也会出现健全性问题。由于源文正文未完整提供，本摘要基于现有讨论和背景信息。

hackernews · juhopitk · 8月1日 18:32 · [社区讨论](https://news.ycombinator.com/item?id=49137060)

**「背景」** Lean 是一种依赖类型定理证明器，其内核负责验证证明的有效性；若内核存在实现漏洞，就可能接受本应无效的证明，破坏系统的可靠性（soundness）。2026 年 7 月 25 日，Ramana Kumar 发布了一个看似无公理（sorry-free）的 Collatz 猜想“反证明”，该证明借助 AI 辅助生成，实际上利用了 Lean 内核在处理嵌套归纳类型时的漏洞。该问题被编号为 \#14576，并在 7 月 27 日那一周被报告和修复。

**「影响」** 使用 Lean 或依赖独立内核检查来验证关键证明的用户应升级到最新版本，以降低因该缺陷产生的风险；不过由于利用通常需要多个实现同时存在各自缺陷，实际影响有限。

**「社区讨论」** 评论普遍认为健全性缺陷并不代表验证体系整体失效，但提醒不应将验证结果视为绝对保证；也有评论将 Lean 与 Metamath 等更简单的内核对比，认为后者的元理论可能更不易受实现缺陷影响，并担忧 AI 自动生成形式化证明时此类问题会更频繁出现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-02-lean-kernel-soundness-bug-14576-postmortem-of-the-ai-assisted-collatz-conjecture-disproof-and-fix">Lean Kernel Bug #14576: Postmortem and Technical Analysis</a></li>
<li><a href="https://tildes.net/~comp/1vep/postmortem_for_lean_kernel_soundness_bug_14576">Postmortem for Lean kernel soundness bug #14576 - ~comp</a></li>
<li><a href="https://news.ycombinator.com/item?id=49137060">Postmortem for Kernel Soundness Bug #14576 | Hacker News</a></li>

</ul>
</details>

**标签**: `#Lean`, `#formal-verification`, `#soundness-bug`, `#proof-assistant`, `#type-theory`

---

<a id="item-tech-news-7"></a>
### [开放信争议：微软与 Anthropic 就开放权重模型立场分歧](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 7.0/10

西蒙·威利森总结了最近几周关于 AI 发展的开放信。微软于 7 月 24 日牵头发布了《开放权重与美国 AI 领导力》，获得包括 NVIDIA、亚马逊、Y Combinator、Linux 基金会以及后来的 OpenAI 在内的 235 家 AI 相关企业签署。该信明确反对美国政府以“安全”为由禁止或限制开放权重模型，并指出仅依赖封闭模型并不天然安全，同时支持蒸馏技术。Anthropic 没有签署这封信，并于三天后发布了自己的立场，CEO 达里奥·阿莫迪呼吁打击“工业规模蒸馏操作”，但表示 Anthropic 从未主张禁止开放权重模型。7 月 28 日，1324 名前沿 AI 公司员工签署《Pacing the Frontier》公开信，要求美国政府支持国际努力，以刻意放缓自动化 AI 开发的步伐。

rss · Simon Willison · 8月2日 04:16

**「背景」** 开放权重 AI 模型允许开发者访问和修改模型权重，但美国政府可能出于安全担忧对其施加限制。这一动向引发了行业内的争论，微软等公司认为开放权重有助于安全研究和竞争，而 Anthropic 则强调蒸馏等技术可能被滥用于复制模型能力。

**「影响」** 微软联合 235 家企业的公开信意味着美国科技行业主流反对限制开放权重模型，可能影响政策制定者的立场。同时，Anthropic 的缺席和公开反对蒸馏操作凸显了行业内部在安全监管上的深刻分歧。

**标签**: `#AI policy`, `#open source`, `#open weights`, `#artificial intelligence`, `#technology industry`

---

<a id="item-tech-news-8"></a>
### [OpenAI 称用内部模型攻克十个数学难题](https://simonwillison.net/2026/Aug/1/ten-advances-in-mathematics/#atom-everything) ⭐️ 7.0/10

OpenAI 宣布，其下一代主要模型的内部版本 Astra 已解决十个数学与理论计算机科学问题，这些问题的主要结果至少十年没有进展；该公司称，按 GPT-5.6 Sol token 价格计算，每个问题花费不到 2000 美元。OpenAI 公开了 Lean 4 形式化证明的 GitHub 仓库、描述解决方案的论文，以及由 LLM 生成的推理回顾 PDF，但未说明在多少个未成功的问题上也花费了约 2000 美元。这一公告引发了数学界类似“深蓝时刻”的讨论，并与陶哲轩提出的“大数学”愿景相关联。由于 OpenAI 没有披露失败的尝试，实际成功率和提示词的透明度仍有待验证。

rss · Simon Willison · 8月1日 20:34

**「背景」** 这些数学难题长期缺乏主要进展，而 AI 辅助证明近年来逐渐兴起。陶哲轩在 IEEE Spectrum 上提出“大数学”愿景：人类与机器进行大规模、去中心化的协作，人类承担创造性部分，AI 完成大量技术性工作。OpenAI 的成果被视为这一趋势的又一例证。

**「影响」** 该公告可能加剧数学家对 AI 改变学科节奏的焦虑，同时也为 AI 辅助数学研究提供了成本和透明度方面的新参考；但由于 OpenAI 未披露失败尝试的数量，其宣称的成功率仍存在不确定性。

**标签**: `#artificial intelligence`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#AI research`

---

<a id="item-tech-news-9"></a>
### [AI 芯片每 9 个月翻番，2028 年底全球将达 2 亿颗](https://www.nytimes.com/interactive/2026/07/29/technology/ai-chips-data-center-boom.html) ⭐️ 7.0/10

据《纽约时报》互动报道，全球 AI 芯片数量当前约 2000 万颗，Epoch AI 估算这一数字每 9 个月翻一番，到 2028 年底将达约 2 亿颗，是当前的 10 倍。IDC 预测，全球 AI 基础设施投资将从去年的 3180 亿美元增至 2029 年的逾 1 万亿美元。推动这一增长的是“规模定律”，即算力越大，AI 能力越强；美国控制全球约 80%的 AI 算力，仅 Google 一家的 AI 芯片数量据信是中国所有公司的四倍，中国正通过自研半导体和 AI 基础设施加速追赶。大规模建设引发电价上涨与环境争议，经济学家警告当前支出可能超过盈利，历史上基建狂热常伴随泡沫破裂。

telegram · zaihuapd · 8月2日 01:01

**「背景」** 规模定律是 AI 领域的一种经验法则：模型能力随训练计算量、数据和参数规模的增大而提升，因此科技公司竞相扩建 AI 数据中心、增加专用 AI 芯片（如 GPU 和 TPU）。随着部署规模扩大，电力消耗和基建投入成为关键约束，促使行业关注芯片增速与投资回报是否可持续。

**「影响」** 对云服务商、芯片厂商和数据中心运营商而言，这一扩张意味着巨大的市场机会，但也将使电力成本与产能建设成为竞争关键；若盈利速度跟不上投资，部分项目可能面临重新定价或泡沫风险。

**标签**: `#AI chips`, `#data center`, `#infrastructure`, `#scaling laws`, `#industry trends`

---

<a id="item-tech-news-10"></a>
### [苹果限制漏洞报告提交以应对 AI 垃圾报告](https://www.ft.com/content/4532122d-90f2-4433-9df6-ca99d8a141d2?syn-25a6b1a6=1) ⭐️ 7.0/10

苹果承认已于今年 6 月限制研究人员可同时提交的漏洞报告数量，并设置 30 天冷却期，以应对大量借助 AI 模型生成的低质量安全报告。意大利安全初创公司 Bynario 称，其用 ChatGPT 在三周内于最新 macOS 中发现 50 多个漏洞，包括可让攻击者完全控制电脑的提权漏洞链，但因提交限额无法向苹果报告。苹果表示已与 Bynario 取得联系并审核其提交，同时也在用 AI 加强自身防御：本周发布的系统安全更新修复数量约为以往的五倍，并致谢 Anthropic 和 OpenAI 的工具协助发现漏洞。

telegram · zaihuapd · 8月2日 05:50

**「背景」** 苹果公司自今年 6 月起限制了安全研究人员可同时提交的漏洞报告数量，并引入了 30 天冷却期，以应对大量由 AI 辅助生成的低质量或虚构安全报告对审核系统造成的压力。据相关报道，研究人员在需要时仍可申请更高的提交配额。与此同时，意大利安全初创公司 Bynario 声称使用 ChatGPT 在最新版 macOS 中发现了 50 多个漏洞，包括提权漏洞链，但因提交限额而无法向苹果报告。

**「影响」** 漏洞研究者和安全团队向苹果提交 macOS 漏洞的通道受到更严限制，可能延迟真实漏洞的修复，同时苹果借助 AI 加强防御导致安全更新数量激增，修复规模约为以往的五倍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://byte.eco/post/apple-limits-bug-report-submissions-amid-ai-surge">Apple Limits Bug Report Submissions Amid AI Surge - byte.eco</a></li>

</ul>
</details>

**标签**: `#apple`, `#security`, `#vulnerability-reporting`, `#ai`, `#macos`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [高盛股票交易业务 Q2 收入跃升 72%，创纪录](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

高盛第二季度股票交易收入跃升 72%，达到创纪录的 74.2 亿美元，超出市场预期；该行交易业务正有望创下全年纪录。上述数字为公司披露的实际业绩，但报道未明确说明 72%的比较基准。

rss · CNBC Finance · 8月1日 20:22

**「背景」** 高盛近年调整其全球银行与市场部门策略，推动投行和财富管理领域的大客户使用其股票交易服务，并持续投资相关业务，以更好把握市场波动带来的机遇。

**标签**: `#Goldman Sachs`, `#equities trading`, `#earnings`, `#investment banking`, `#market volatility`

---

<a id="item-finance-news-2"></a>
### [美国将 43 家中国企业列入 UFLPA 实体清单](https://companies.caixin.com/2026-08-01/102470547.html) ⭐️ 8.0/10

美国国土安全部 7 月 31 日宣布将 43 家中国企业列入 UFLPA（《维吾尔强迫劳动预防法》）实体清单，新增名单于 8 月 3 日生效；相关企业向美国出口的货物将被推定为涉及强迫劳动并受到进口限制。

telegram · zaihuapd · 8月2日 05:23

**「背景」** 美国《维吾尔强迫劳动预防法》（UFLPA）规定，若企业无法证明其供应链不涉及新疆强迫劳动，相关货物将被推定为禁止进口。被列入 UFLPA 实体清单后，自 2026 年 8 月 3 日起，美国海关与边境保护局将对这 43 家中国企业生产的产品适用这一可反驳推定；此次新增后，UFLPA 实体清单上共有 187 家实体。

**「影响」** 涉及福建七匹狼、洽洽食品、郑州思念食品等企业，其美国订单和供应链将直接受阻，美国进口商也需要调整采购来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dhs.gov/news/2026/07/31/dhs-announces-addition-43-companies-uflpa-entity-list">DHS Announces the Addition of 43 Companies to the UFLPA ...</a></li>
<li><a href="https://www.kharon.com/resources/article/forced-labor/dhs-uflpa-entity-list-additions">DHS Added 43 Chinese Firms to the UFLPA Entity List. Kharon ...</a></li>
<li><a href="https://www.thompsonhinesmartrade.com/2026/07/dhs-updates-uflpa-entity-list-with-43-additional-chinese-companies/">DHS Updates UFLPA Entity List with 43 Additional Chinese ...</a></li>

</ul>
</details>

**标签**: `#UFLPA`, `#entity list`, `#trade policy`, `#Chinese companies`, `#supply chain`

---

<a id="item-finance-news-3"></a>
### [公积金条例拟修订：灵活就业者可缴存，装修和物业费可提取](https://weibo.com/1642634100/RbwfKezfq) ⭐️ 8.0/10

住房城乡建设部近日就《住房公积金管理条例（修订征求意见稿）》公开征求意见，拟允许个体工商户、外卖员、快递员、网约车司机等灵活就业人员自愿缴存公积金，并把自住住房装修、物业费纳入可提取情形。该文件目前仍是征求意见稿，尚未正式生效。

telegram · zaihuapd · 8月2日 06:32

**「背景」** 《住房公积金管理条例》此前在 2002 年和 2019 年修订过两次；本次的修订征求意见稿由住建部于 2026 年 6 月 5 日公布，面向社会公开征求意见，截止时间为 2026 年 7 月 5 日，目前仍属草案，尚未生效。

**「影响」** 若修订最终通过，灵活就业人员将有机会自愿参与公积金缴存，缴存者在住房装修、缴纳物业费时也可申请提取，跨地区互认互贷则有助于流动就业人员异地使用账户资金。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.toutiao.com/article/7648082700527550985/">住房公积金管理条例修订征求意见：支持交物业费，灵活就业人员自愿参加</a></li>
<li><a href="https://www.sohu.com/a/1033784479_121745188">住房公积金管理条例修订征求意见稿公示_需求_审批结果_资金</a></li>
<li><a href="https://finance.sina.cn/2026-06-07/detail-iniapryw9989024.d.html?vt=4">《住房公积金管理条例》拟修订 专家解读四大新变化|住房和城乡建设部|征求意见|房地产|制度|物业费_手机新浪网</a></li>

</ul>
</details>

**标签**: `#housing provident fund`, `#China policy`, `#gig economy`, `#housing consumption`, `#regulation`

---