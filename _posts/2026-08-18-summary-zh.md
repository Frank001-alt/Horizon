---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 197 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Mojo 编程语言正式开源](#item-tech-news-1) ⭐️ 9.0/10
2. [GitLab 紧急修复严重漏洞，可未授权删除项目](#item-tech-news-2) ⭐️ 9.0/10
3. [Linux 7.3 提升 VRAM 超量使用性能](#item-tech-news-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B 基准测试得分 52，媲美更大模型](#item-tech-news-4) ⭐️ 8.0/10
5. [Asana 用 Codex 两周完成五年工作量](#item-tech-news-5) ⭐️ 8.0/10
6. [Rust GPU 卸载：可移植、安全且高效](#item-tech-news-6) ⭐️ 8.0/10
7. [中国要求部分政府机构提前卸载定制版 Windows 10](#item-tech-news-7) ⭐️ 8.0/10

**科技博客**
1. [基准测试的泛滥：批判与反思](#item-tech-blog-1) ⭐️ 9.0/10
2. [用 20 美元工具修复变砖的 Framework 笔记本](#item-tech-blog-2) ⭐️ 8.0/10
3. [CSS：收件箱中的炸弹](#item-tech-blog-3) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Mojo 编程语言正式开源](https://www.modular.com/blog/mojo-open-source) ⭐️ 9.0/10

Modular 公司宣布其面向 AI/ML 的编程语言 Mojo 现已正式开源，编译器及工具链以 Apache 2 许可证发布。此前 Mojo 曾承诺在 2023 年 5 月开源，并在上周发布 1.0 版本后兑现了这一承诺。Mojo 最初的目标是成为 Python 的超集，但自 2025 年 8 月起，官方调整了方向，不再强求完全兼容 Python，而是定位为一种独立的语言，专注于简化 GPU 编程，并采用受 Python 启发的语法。这一开源举措有望推动 Mojo 生态系统的快速发展，并可能对 AI/ML 开发工具链产生重要影响。

rss · Lobsters · 8月18日 16:34

**「背景」** Mojo 是由 Modular 公司开发的一种面向 AI/ML 的编程语言，旨在结合 Python 的易用性与 C/C++ 的性能，特别优化了 GPU 编程体验。自 2023 年 5 月首次发布以来，Mojo 一直承诺开源，但直到 2025 年 8 月左右，其发展路线图从“成为 Python 的超集”调整为“可能不会完全兼容 Python”，转而强调借助 AI 辅助工具迁移现有 Python 代码。此前，Modular 已于 2024 年 3 月开源了 Mojo 标准库，而此次开源的是完整的编译器与工具链。

**「影响」** 对于 AI/ML 开发者而言，Mojo 的开源意味着可以自由使用、修改和贡献这一高性能语言，从而可能加速其在 GPU 编程和 AI 工作负载中的采用，并促进社区驱动的工具和库的涌现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_%28programming_language%29">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.modular.com/blog/mojo-open-source">Modular: Mojo🔥 is now open source!</a></li>

</ul>
</details>

**标签**: `#programming-languages`, `#ai`, `#open-source`, `#mojo`, `#machine-learning`

---

<a id="item-tech-news-2"></a>
### [GitLab 紧急修复严重漏洞，可未授权删除项目](https://www.ithome.com/0/991/362.htm) ⭐️ 9.0/10

GitLab 于 2026 年 8 月 17 日发布紧急安全更新，修复了社区版（CE）和企业版（EE）中的两个安全漏洞。其中严重漏洞 CVE-2026-19478（CVSS 评分 9.4）允许未认证攻击者远程修改或删除公共项目及用户数据，甚至可对开源项目发起供应链攻击；高危漏洞 CVE-2026-19650（CVSS 评分 7.1）是 GraphQL 多路复用查询处理器中的 CSRF 漏洞，可允许攻击者通过 GET 请求执行 GraphQL 变更操作。两个漏洞影响 GitLab CE/EE 从 18.2 开始至 18.11.11 之前、19.0 至 19.0.8 之前、19.1 至 19.1.6 之前、以及 19.2 至 19.2.4 之前的所有版本，修复版本为 19.2.4、19.1.6、19.0.8 和 18.11.11。官方强烈建议所有自托管 GitLab 实例立即升级。目前 PoC 和技术细节已公开，据奇安信鹰图资产测绘平台数据，国内风险资产总数为 108658 个，全球风险资产总数为 401607 个。官方尚未发现漏洞已被在野利用的证据。

rss · IT HOME · 8月18日 15:52

**「背景」** GitLab 是一个广泛使用的 DevOps 平台，提供代码托管、CI/CD 等功能，分为社区版（CE）和企业版（EE）。GraphQL 是 GitLab 用于 API 的查询语言，允许客户端灵活请求数据。CVE-2026-19478 是 GitLab GraphQL 层在处理 @gl\_introduced 指令时存在的代码注入漏洞，攻击者可通过构造恶意 GraphQL 指令，在无需认证的情况下修改或删除公共项目及用户数据。该漏洞被归类为 CWE-94（代码注入），CVSS 评分为 9.4，影响 GitLab CE/EE 从 18.2 到 19.2.4 之前的多个版本。

**「影响」** 所有自托管 GitLab 实例（包括社区版和企业版）在受影响的版本范围内均面临严重风险：未认证攻击者可利用 CVE-2026-19478 远程删除或修改公共项目及用户数据，甚至可能对开源项目发起供应链攻击；CVE-2026-19650 则允许在用户交互条件下通过 GET 请求执行 GraphQL 变更操作。据奇安信鹰图资产测绘平台数据，全球约有 401607 个风险资产，其中中国国内有 108658 个。官方已发布修复版本 19.2.4、19.1.6、19.0.8 和 18.11.11，建议所有自托管实例立即升级，以消除被利用的风险。

**「社区讨论」** 无社区评论可用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/gitlab-graphql-vulnerability/">Critical GitLab GraphQL Vulnerability Allow Attackers to ...</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-19478">CVE-2026-19478 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://threataft.com/articles/gitlab-graphql-code-injection-data-manipulation-cve-2026-19478">CVE-2026-19478 — Critical GitLab GraphQL Vulnerability ...</a></li>
<li><a href="https://www.securityweek.com/gitlab-patches-critical-code-injection-vulnerability/">GitLab Patches Critical Code Injection Vulnerability</a></li>
<li><a href="https://cybersecuritynews.com/gitlab-graphql-vulnerability/">Critical GitLab GraphQL Vulnerability Allow Attackers to ...</a></li>
<li><a href="https://www.techtimes.com/articles/324811/20260818/gitlab-emergency-patch-third-graphql-flaw-2026-lets-unauthenticated-attackers-delete-projects.htm">GitLab Emergency Patch: Third GraphQL Flaw of 2026 Lets ...</a></li>

</ul>
</details>

**标签**: `#GitLab`, `#security`, `#CVE`, `#vulnerability`, `#supply chain`

---

<a id="item-tech-news-3"></a>
### [Linux 7.3 提升 VRAM 超量使用性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux 内核 7.3 版本引入了针对 VRAM 超量使用（overcommit）的性能改进，旨在缓解 GPU 内存压力问题。该改进通过优化内核在显存不足时的内存管理策略，提升了 GPU 工作负载下的系统响应速度和稳定性。文章指出，这一改进对于依赖大显存的应用程序（如机器学习和游戏）尤为重要，但具体实现细节和性能提升幅度尚未完全公开。社区用户对此表示期待，并希望该改进能尽快合并到主线内核中。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**「背景」** Linux 内核的 VRAM（显存）管理历来面临挑战，尤其是在 GPU 显存不足时，系统性能会显著下降。此前，内核缺乏有效的显存超卖（overcommit）处理机制，导致在显存压力下出现卡顿或崩溃。Linux 7.3 版本将引入由 Vock 等人开发的补丁，旨在改进 GPU 驱动程序的显存管理行为，提升显存超卖时的性能。这些补丁已合并到上游，并计划在 Linux 7.3 中发布。

**「影响」** 对于使用 Linux 7.3 及以上内核的 GPU 密集型用户（如游戏玩家、AI 研究人员），该改进有望减少因显存不足导致的性能下降或崩溃，提升整体体验。然而，由于 NVIDIA 驱动目前不支持显存分页，该改进对 NVIDIA 用户的实际效果可能有限。

**「社区讨论」** 社区普遍对该改进持积极态度，认为内核在内存分配上的优化方向正确，但同时也指出应用程序自身应更好地告知内核显存需求。部分用户提到 NVIDIA 驱动缺乏显存分页支持，可能限制该改进的效果，并希望内核能进一步解决内存碎片化问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management ...</a></li>
<li><a href="https://www.nitin-rachabathuni.com/blog/linux-kernel-vram-overcommit-performance">Optimizing VRAM Overcommit: How Linux Kernel Improvements ...</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM</a></li>

</ul>
</details>

**标签**: `#linux`, `#kernel`, `#vram`, `#gpu`, `#performance`

---

<a id="item-tech-news-4"></a>
### [Qwen 3.8 27B 基准测试得分 52，媲美更大模型](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B 在 Artificial Analysis Intelligence Index 上获得 52 分，与 GPT-5.6 Luna（最大配置）得分相同，仅比 GLM-5.2（最大配置）和 DeepSeek V4 Pro 0813（最大配置）低 1 分。值得注意的是，GLM-5.2 拥有 7530 亿参数，DeepSeek V4 Pro 0813 拥有 1.7 万亿参数，而 Luna 的规模未知但可能远大于 27B。这一成绩凸显了紧凑型 27B 模型在效率上的显著优势，Simon Willison 称其为“真正令人惊叹的模型”。该消息通过 Hacker News 传播，并标注了 AI、生成式 AI、LLM、Qwen 以及中国 AI 等相关标签。

rss · Simon Willison · 8月17日 23:58

**「背景」** Qwen 3.8 27B 是阿里巴巴 Qwen 系列中的一款 270 亿参数稠密视觉语言模型，专为编码、专业工作、研究及长时程智能体任务而设计，支持可配置推理和原生 262K token 上下文窗口。该模型以部署友好的规模提供较强的规划能力，并能更好地处理工具和环境反馈，从而实现更可靠的多步骤任务完成。

**「影响」** 对于依赖本地或低成本部署的开发者而言，Qwen 3.8 27B 的基准测试成绩表明，小型模型可以在性能上媲美甚至接近巨型模型，从而可能降低先进 AI 能力的硬件门槛和运营成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers-ai/models/qwen3.8-27b/">qwen3.8-27b (Qwen) · Cloudflare AI docs · Cloudflare Workers ...</a></li>
<li><a href="https://www.jetson-ai-lab.com/models/qwen3-8-27b/">Qwen3.8 27B - Jetson AI Lab</a></li>
<li><a href="https://lmstudio.ai/models/qwen3.8">Qwen3.8 - lmstudio.ai</a></li>

</ul>
</details>

**标签**: `#qwen`, `#llm`, `#benchmark`, `#ai`, `#efficiency`

---

<a id="item-tech-news-5"></a>
### [Asana 用 Codex 两周完成五年工作量](https://openai.com/index/asana) ⭐️ 8.0/10

Asana 使用 OpenAI 的 Codex 在两周内替换了一个过时的测试系统，完成了原本预计需要五年才能完成的工作，成本约为 12,000 美元。这一案例展示了 AI 编程工具在真实工程组织中的显著生产力提升，具体表现为时间缩短和成本降低。Codex 是 OpenAI 开发的 AI 编程助手，能够自动生成和修改代码。该案例表明，AI 编程工具可以大幅加速大型代码库的现代化改造，但需要注意的是，这是一个案例研究，而非普遍适用的突破。

rss · OpenAI Blog · 8月18日 07:00

**「背景」** Asana 是一家项目管理软件公司，其测试系统因技术债务而变得过时，需要大规模重写。OpenAI Codex 是一种基于 GPT 的 AI 编程工具，能够理解自然语言指令并生成代码，从而帮助开发者自动化编码任务。

**「影响」** 对于 Asana 的工程团队而言，这一案例意味着他们能够以极低的成本快速完成技术债务清理，从而将资源重新分配到其他高优先级项目上。然而，这一结果可能依赖于特定代码库和任务类型，其他组织未必能复制同样的效率。

**标签**: `#AI coding`, `#OpenAI Codex`, `#software engineering`, `#productivity`, `#case study`

---

<a id="item-tech-news-6"></a>
### [Rust GPU 卸载：可移植、安全且高效](https://arxiv.org/pdf/2608.13759) ⭐️ 8.0/10

一篇论文介绍了内置于 Rust 编译器（rustc）和 LLVM 后端的零开销、多供应商 GPU 卸载框架，旨在解决 GPU 编程中内存安全与性能之间的权衡。该框架利用 Rust 的类型系统、所有权系统和严格别名保证（noalias）来高效管理数据转移，并解决了跨供应商 ABI 降低不匹配的问题，引入了两遍编译流水线以安全处理手动和编译器生成的内存移动。在 RAJAPerf 基准上的评估表明，该基于 rustc 的解决方案能够生成具有竞争力的 LLVM IR，内核性能接近原生、手工优化的 CUDA 和 HIP C++ 基线。这项工作为 Rust 在 GPU 计算领域的应用提供了新的可能性，可能影响未来的 Rust GPU 开发。

rss · Lobsters · 8月18日 12:16

**「背景」** 传统上，高性能 GPU 编程需要在执行效率和内存安全之间做出妥协。虽然 Rust 通过严格的所有权模型在主机 CPU 上保证了编译时内存安全，但将这些约束应用于大规模并行 GPU 执行环境，此前要么需要供应商锁定的领域特定语言（DSL），要么需要显式使用不安全的原始指针。该论文提出的框架旨在将 Rust 的安全保证扩展到 GPU 编程，同时保持性能。

**「影响」** 该框架可能使 Rust 开发者能够编写安全、可移植的 GPU 内核，而无需依赖特定供应商的 DSL 或不安全代码，从而降低 GPU 编程的复杂性并提高代码的可移植性。然而，其实际采用程度取决于该框架是否被整合到主流的 rustc 和 LLVM 版本中，以及其在更广泛工作负载上的性能表现。

**标签**: `#Rust`, `#GPU programming`, `#compilers`, `#LLVM`, `#memory safety`

---

<a id="item-tech-news-7"></a>
### [中国要求部分政府机构提前卸载定制版 Windows 10](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 8.0/10

中国国家安全部已要求部分政府相关机构卸载定制版 Windows 10，将原定于 2027 年 2 月的停用计划提前数月。知情人士称，此举源于数据安全担忧，但未指明具体漏洞。微软回应称，未发现影响该产品的安全事件，且该产品仍在定期获得安全更新。这一行动可能影响微软在中国政府市场的布局，并凸显数据安全在政府采购中的重要性。

telegram · zaihuapd · 8月18日 06:22

**「背景」** 中国政府长期以来推动在政府机构中使用国产操作系统和软件，以减少对外国技术的依赖。此次涉及的定制版 Windows 10 是微软与中国政府合作开发的政府专用版本，旨在满足中国的安全和合规要求。然而，出于数据安全担忧，中国国家安全部已要求部分政府相关机构提前卸载该版本，原定于 2027 年 2 月的停用计划被提前。微软表示未发现影响该产品的安全事件，且该产品仍在定期获得安全更新。

**「影响」** 受影响的政府机构将需要提前迁移至替代操作系统，可能增加短期运维成本；微软在中国政府市场的信誉可能受到一定影响，但具体影响程度尚待观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>
<li><a href="https://thenextweb.com/news/china-removes-microsoft-windows-10-state-agencies">China is removing Microsoft’s Windows 10 from state agencies</a></li>
<li><a href="https://wccftech.com/china-state-agencies-uninstall-windows-10-cmit-government-edition/">China’s State-Linked Firms Are Moving Away From Windows 10 Due To Security Concerns, Despite The Custom OS Developed By Microsoft Under Stringent Supervision</a></li>

</ul>
</details>

**标签**: `#China`, `#Windows 10`, `#government policy`, `#data security`, `#Microsoft`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [基准测试的泛滥：批判与反思](https://danluu.com/benchpocalypse/) ⭐️ 9.0/10

rss · Lobsters · 8月18日 00:47

**「背景」** 在技术行业中，基准测试被广泛用于评估性能和指导决策，但作者指出，基准测试的泛滥可能导致工程团队过度优化指标而忽视真实用户需求。这种对量化指标的盲目信任，往往源于对可测量性的偏好，却可能扭曲了工程优先级。

**「方案」** 作者通过具体案例展示了基准测试如何引发“过度拟合”现象，即团队针对特定基准进行优化，却在实际场景中表现不佳。他分析了基准测试背后的激励机制，指出当基准成为衡量成功的唯一标准时，工程师可能会牺牲代码可维护性、系统灵活性等长期价值。为了应对这一问题，作者提出了一种更细致的评估方法：不仅关注基准分数，还要结合真实工作负载、用户反馈和系统整体行为进行综合判断。他强调，基准测试应作为参考工具而非绝对真理，并建议团队定期审视基准的相关性和局限性，避免陷入“基准军备竞赛”。

**「启示」** 作者的核心论点是，基准测试虽然有用，但过度依赖会扭曲工程决策，导致资源错配和短期思维。他呼吁工程师和领导者以批判性眼光看待基准，将评估重点放在实际用户价值和系统长期健康上，而非盲目追求数字上的提升。

**标签**: `#benchmarks`, `#engineering culture`, `#incentives`, `#evaluation`, `#critical thinking`

---

<a id="item-tech-blog-2"></a>
### [用 20 美元工具修复变砖的 Framework 笔记本](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 8.0/10

hackernews · Lobsters · 8月18日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49345220)

**「背景」** 作者的一台 AMD 7040 系列 Framework 13 笔记本在 BIOS 更新后变砖，无法启动。官方支持无法解决，而送修或更换主板成本高昂，且可能失去数据。作者决定自行修复，但面临缺乏官方固件恢复工具和文档的挑战。

**「方案」** 作者使用了一个约 20 美元的 SPI 闪存编程器，直接读取并重写主板上的 BIOS 芯片。他首先拆机找到芯片，用编程器备份原固件，然后从网上获取正确的固件镜像，通过编程器写入。过程中需要小心处理芯片引脚，避免损坏。作者还讨论了其他方案，如使用树莓派或 Arduino，但认为专用编程器更简单可靠。他强调了备份固件的重要性，并指出官方不提供恢复工具，导致用户只能依赖第三方方案。最终，笔记本成功恢复，但作者也提醒读者，此操作有风险，且可能使保修失效。

**「启示」** 作者认为，厂商在 BIOS 更新失败后缺乏官方恢复途径，迫使用户自行解决，这暴露了维修权问题。他呼吁厂商提供更开放的固件恢复工具，并建议用户学习基本的硬件维修技能，以应对类似情况。

**标签**: `#Framework laptop`, `#BIOS recovery`, `#SPI flash`, `#firmware`, `#hardware repair`

---

<a id="item-tech-blog-3"></a>
### [CSS：收件箱中的炸弹](https://portswigger.net/research/css-the-bomb-inside-your-inbox) ⭐️ 8.0/10

rss · Lobsters · 8月18日 13:30

**「背景」** 电子邮件客户端通常允许使用 CSS 来美化邮件，但这种看似无害的功能却可能被滥用，成为攻击者窃取数据或进行界面伪装（UI redressing）的武器。作者指出，尽管现代 Web 安全措施日益完善，但邮件客户端对 CSS 的宽松处理仍然为攻击者留下了可乘之机。

**「方案」** 作者详细展示了如何利用 CSS 在邮件客户端中实施攻击。例如，通过 CSS 选择器和背景图片请求，攻击者可以探测用户属性或窃取敏感信息；通过精心构造的样式，可以覆盖邮件界面，诱导用户点击恶意链接。文章提供了具体的代码示例和攻击场景，并分析了这些攻击之所以成功的原因——邮件客户端对 CSS 的解析和执行往往比浏览器更为宽松，且缺乏严格的沙箱隔离。作者还讨论了缓解措施，如限制 CSS 属性和使用内容安全策略（CSP），但指出这些措施在邮件客户端中的实施并不完善，且可能影响用户体验。

**「启示」** 作者的核心论点是，CSS 在邮件客户端中的滥用是一个被低估的安全威胁，其攻击面比人们通常认为的要大得多。这一研究提醒安全从业者，即使在看似受限的环境中，也需要重新审视 CSS 的潜在风险，并推动邮件客户端加强安全防护。

**标签**: `#CSS`, `#email security`, `#client-side attacks`, `#web security`, `#exploitation`

---