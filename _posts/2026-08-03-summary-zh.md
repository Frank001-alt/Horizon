---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> 从 30 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [Karpathy 推文引发“生成可玩弹球游戏”LLM 基准讨论](#item-tech-news-1) ⭐️ 7.0/10
2. [Kakehashi：在 Linux ARM 上运行 macOS 二进制的实验用户态兼容层](#item-tech-news-2) ⭐️ 7.0/10
3. [eBay 骚扰批评者致 5600 万美元赔偿与入狱](#item-tech-news-3) ⭐️ 7.0/10
4. [开放权重模型之争：企业反对禁令，员工呼吁放缓前沿](#item-tech-news-4) ⭐️ 7.0/10

**财经新闻**
1. [高盛二季度股票交易收入创纪录，全年交易业务有望创新高](#item-finance-news-1) ⭐️ 8.0/10
2. [AI 芯片数量预计 2028 年底达 2 亿颗](#item-finance-news-2) ⭐️ 7.0/10
3. [住房公积金条例拟修订：灵活就业者可缴存、装修物业费可提取](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Karpathy 推文引发“生成可玩弹球游戏”LLM 基准讨论](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Karpathy 的一条推文引发讨论，社区提出把“只凭提示词生成可玩的弹球游戏”作为评估 LLM 对物理世界理解的新基准。很多前沿模型仍会失败，例如把墙壁放在发射滑道前挡住弹球、挡板翻转方向错误，或让弹球从底部漏洞直接掉出而够不到挡板。据社区评论，Anthropic 的 Opus 5 首次在某个测试框架中“一次成功”完成该任务。讨论还指出，这类定性基准虽然主观，但比单纯生成图像更能暴露模型对真实世界物理规则的理解。

hackernews · delichon · 8月2日 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**「背景」** “制作一个弹球游戏”已经成为评估前沿大语言模型对物理世界理解能力的新型基准：模型往往能生成正确组件，却因碰撞、轨道或挡板方向等物理逻辑错误导致游戏无法真正运行。据社区讨论，Anthropic 的 Opus 5 首次在该提示的“单次生成”测试中成功，而 Andrej Karpathy 也曾用 Claude Opus 5 的 100 万 token 预算生成《指环王》开篇段落的 Three.js 渲染。

**「影响」** 对于模型评估者和开发者，这个非正式基准提供了一个可观察的定性测试，未来可能被用来比较前沿模型在物理世界建模方面的进展。

**「社区讨论」** 评论中有共识认为“生成可玩弹球游戏”是暴露物理世界理解的新基准，但也有人担心 Anthropic 模型被专门训练过 three.js 代码生成，因而这类演示不能反映通用能力；另有开发者分享了自己为 3D 场景生成做大量定制调优的经验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techstacks.io/posts/18035/karpathy-s-pelican">Karpathy’s Pelican - techstacks.io</a></li>

</ul>
</details>

**标签**: `#LLM`, `#benchmark`, `#AI evaluation`, `#physical world`, `#frontier models`

---

<a id="item-tech-news-2"></a>
### [Kakehashi：在 Linux ARM 上运行 macOS 二进制的实验用户态兼容层](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi 是一个实验性的用户态兼容层，目标是在 Linux ARM 机器上原生运行 macOS 命令行二进制文件。当前工作原型包括 7-Zip，它在包含 8k 个文件的目录树上通过了多线程压缩测试，但性能比原生 Linux 执行慢约 5.2 倍；curl 则有超过 200 个命令和选项通过自动化 Docker 测试脚本。项目还展示了 Xcode 自带的 Git 工具的基本版本控制功能。该方案仍处于早期阶段，但社区评论认为其长期前景类似于 Wine/Proton，并建议与已开放 ARM64 支持的 Darling 项目合作。这项工作的意义在于，它可能让 Linux ARM 用户在不依赖 Apple 系统的情况下运行更多 macOS 软件。

hackernews · vlad\_kalinkin · 8月2日 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**「背景」** Kakehashi 是一个实验性用户态兼容层，目标是在 Linux aarch64 上直接运行 macOS ARM64 的命令行二进制文件。它采用无 JIT 的翻译方式，负责加载 Darwin 的 Mach-O 可执行文件，并通过独立的 libSystem 实现将 BSD 系统调用转换为 Linux 调用。这一思路与 Darling 项目类似，但 Kakehashi 专注于 Linux ARM 环境，目前已有 7-Zip、curl 等工具的原型验证。

**「影响」** 对于 Linux ARM 用户和开发者来说，Kakehashi 目前证明了 macOS 命令行工具（如 7-Zip、curl 和 Git）可以在该平台上运行，但 5.2 倍的性能差距和实验性质量意味着它尚不能作为实用的日常替代方案。

**「社区讨论」** Hacker News 评论普遍持积极态度，多位用户表示长期期待此类项目并会持续关注。同时，他们也指出项目仍非常早期、复杂度较高，并提到了 Darling 项目的 ARM64 支持 PR；还有人希望未来能出现类似 yabridge 的桥接，让 Linux 上可以运行 macOS 的 Audio Unit 插件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">wie- project / kakehashi : Userspace macOS translation layer for Linux ...</a></li>
<li><a href="https://savepearlharbor.com/?p=489422">Kakehashi : запуск macOS бинарников на Linux ARM . Часть...</a></li>

</ul>
</details>

**标签**: `#macOS`, `#Linux`, `#ARM`, `#compatibility`, `#open source`

---

<a id="item-tech-news-3"></a>
### [eBay 骚扰批评者致 5600 万美元赔偿与入狱](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay 因旗下全球安全团队对一对批评公司的夫妇（Steiners）实施骚扰与恐吓，最终支付 5600 万美元赔偿，多名涉案员工被判刑。具体判决中，eBay 前安全与安保高级总监 Jim Baugh 被判处 57 个月监禁，前特别行动高级经理 Brian Gilbert 获判已服刑时间、一年监督释放及 2 万美元罚款。检察官称，包括前警长在内的七名 eBay 安全团队成员参与了这场针对 Steiners 夫妇的骚扰行动。这起案件凸显了企业安全部门对网络批评者进行非法报复可能带来的严重法律后果。

hackernews · JumpCrisscross · 8月2日 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**「背景」** eBay 全球安全团队的多名成员（包括前高级警务人员）于 2019 年对马萨诸塞州纳蒂克夫妇 Ina 和 David Steiner 实施骚扰、监视和恐吓，起因是这对夫妇经营电商新闻网站 eCommerceBytes 并曾发文批评 eBay。相关刑事案件已导致多名前高管和员工被判刑，其中前安全与安保高级总监 Jim Baugh 被判 57 个月监禁。夫妇随后提起民事索赔，最终与 eBay 及数名前高管达成约 5570 万美元（报道中常写作 5600 万美元）的和解。

**「影响」** 对科技企业而言，该案确立了内部安全团队针对批评者的骚扰行为可能带来巨额民事赔偿和刑事处罚的明确后果。

**「社区讨论」** 评论中有人质疑此案是否只是冰山一角，认为应彻查这些前警长是否还针对其他批评者；另有用户借机抱怨 eBay 费用高昂，约为含运费和税总价的 13%，而法国 Leboncoin 只收 5%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bostonglobe.com/2026/07/27/business/ebay-harassed-ina-david-steiner-settlement/">Natick couple gets eBay and former execs to pay $ 56 million</a></li>
<li><a href="https://easternherald.com/2026/07/30/ebay-steiners-settlement-56-million-stalking-harassment/">eBay Pays $55.7M to Settle Harassment Campaign Against Journalists</a></li>
<li><a href="https://tribune.com.pk/story/2621354/ebay-to-pay-56m-after-shocking-harassment-campaign-against-blogger-couple">eBay to pay $ 56 m after shocking harassment campaign against...</a></li>

</ul>
</details>

**标签**: `#security`, `#tech industry`, `#legal`, `#eBay`, `#ethics`

---

<a id="item-tech-news-4"></a>
### [开放权重模型之争：企业反对禁令，员工呼吁放缓前沿](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 7.0/10

微软牵头的一份于 7 月 24 日发布的公开信《开放权重与美国 AI 领导力》已获得 235 家 AI 相关企业签署，包括英伟达、亚马逊、YC 和 Linux 基金会，OpenAI 随后也加入，信中明确反对美国政府出于“安全”考虑禁止或限制开放权重模型，并认为完全依赖封闭模型会形成单点故障并削弱竞争。该信还罕见地为蒸馏技术辩护，称政策制定者不应将这种合法模型开发技术等同于盗用。Anthropic 未参与签署，并在三天后发布了自己的立场，CEO Dario Amodei 虽表示从未主张全面禁止开放权重模型，但呼吁打击工业规模的蒸馏行为，并担心开放模型被独裁政府用于网络攻击或生物攻击。7 月 28 日，另一封名为《Pacing the Frontier》的公开信由 1324 名前沿 AI 公司员工签署，包括 OpenAI 首席科学家 Jakub Pachocki、Ilya Sutskever 和 Dario Amodei，呼吁美国政府支持国际合作，以开发技术和治理工具来“有意识地控制自动化 AI 开发的前沿节奏”。这些信件反映了 AI 产业在开放权重模型监管和 AI 发展速度问题上的重大分歧。

rss · Simon Willison · 8月2日 04:16

**「背景」** 开放权重模型允许开发者下载、检查和修改模型权重，是当前 AI 开源生态的核心，但美国政策制定者出于安全担忧可能对其施加限制或禁令。与此同时，自动化 AI 研究被认为可能大幅加速 AI 进步，引发对竞争压力失控的担忧，促使产业界通过公开信表达立场以影响政策走向。

**「影响」** 若美国政策制定者采纳这封公开信的立场，依赖开放权重模型的开发者、研究机构和开源生态可免受禁令影响，继续使用和迭代这些模型；但 Anthropic 等方的反对意见仍可能促使政府加强对蒸馏等模型开发技术的针对性监管。

**标签**: `#AI policy`, `#open weights`, `#open source`, `#Microsoft`, `#industry`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [高盛二季度股票交易收入创纪录，全年交易业务有望创新高](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

高盛公布第二季度股票交易收入同比增长 72%，达到创纪录的 74.2 亿美元，推动公司交易业务有望创下历年最佳年度表现。

rss · CNBC Finance · 8月2日 13:52

**「背景」** 高盛的全球银行与市场部门是该行最大业务板块，上季度收入 155 亿美元，占总收入逾 75%；该部门涵盖投资银行、股票、固定收益、外汇和大宗商品交易。

**「影响」** 其他大型华尔街银行同样受益于市场波动和 AI 资本开支，许多也有望创下历年最佳交易收入，显示整个投行交易板块正因此受益。

**标签**: `#Goldman Sachs`, `#earnings`, `#trading revenue`, `#investment banking`, `#financial sector`

---

<a id="item-finance-news-2"></a>
### [AI 芯片数量预计 2028 年底达 2 亿颗](https://www.nytimes.com/interactive/2026/07/29/technology/ai-chips-data-center-boom.html) ⭐️ 7.0/10

据 Epoch AI 估算，全球 AI 芯片数量每 9 个月翻一番，将从目前约 2000 万颗增至 2028 年底约 2 亿颗；IDC 预测 2029 年全球 AI 基础设施投资将突破 1 万亿美元，而去年为 3180 亿美元。

telegram · zaihuapd · 8月2日 01:01

**「背景」** “规模定律”是指 AI 模型能力通常随计算规模扩大而增强，这也是科技公司大规模投资数据中心的原因。Epoch AI 和 IDC 分别追踪 AI 芯片出货与基础设施支出，并给出上述估算和预测。

**「影响」** 科技巨头的大规模数据中心建设可能推高电价并引发环境争议，经济学家提醒当前支出可能超过盈利，相关行业与投资者需关注成本与回报风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/news/story/ai-chip-production-is-set-to-double-every-9-months-8385353/">AI chip production is set to double every 9 months | LinkedIn</a></li>
<li><a href="https://www.idc.com/resource-center/blog/ai-infrastructure-spending-holds-near-90-billion-in-q1-2026-as-arm-overtakes-x86-in-accelerated-servers-2026-forecast-raised-to-497-billion/">AI Infrastructure Spending Holds Near $90 Billion in Q1 2026 as ARM Overtakes x86 in Accelerated Servers; 2026 Forecast Raised to $497 Billion</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#data center investment`, `#Epoch AI`, `#IDC forecast`, `#technology infrastructure`

---

<a id="item-finance-news-3"></a>
### [住房公积金条例拟修订：灵活就业者可缴存、装修物业费可提取](https://weibo.com/1642634100/RbwfKezfq) ⭐️ 7.0/10

住建部就《住房公积金管理条例（修订征求意见稿）》公开征求意见，拟允许灵活就业人员自愿缴存，并将自住住房装修和物业费纳入公积金提取范围。目前这仍是征求意见稿，尚未正式生效。

telegram · zaihuapd · 8月2日 06:32

**「背景」** 现行公积金制度主要面向单位职工、用于购房和租房；此次修订试图扩大覆盖群体和使用场景，并推动公积金互认互贷。

**「影响」** 若最终通过，该政策有望覆盖外卖员、快递员等灵活就业人员，并支持有房居民用公积金支付装修和物业费，从而降低相关家庭的住房支出压力。

**标签**: `#housing provident fund`, `#policy revision`, `#flexible employment`, `#housing consumption`, `#China`

---