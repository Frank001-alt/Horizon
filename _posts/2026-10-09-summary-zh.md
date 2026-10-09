---
layout: default
title: "Horizon Summary: 2026-10-09 (ZH)"
date: 2026-10-09
lang: zh
---

> 从 236 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Lean 验证 AI 数学形式化不保证原自然语言证明正确](#item-tech-news-1) ⭐️ 8.0/10
2. [Let&\#x27;s Encrypt 将于 2027 年 2 月启用 64 天证书有效期](#item-tech-news-2) ⭐️ 8.0/10
3. [FAST 发现首例演化中脉冲星原生三体系统](#item-tech-news-3) ⭐️ 8.0/10
4. [陶哲轩质疑 OpenAI 的 719 篇 AI 数学证明](#item-tech-news-4) ⭐️ 8.0/10
5. [字节 Seed 团队揭示 DeepSeek 长上下文“抽风”源于相位敏感性](#item-tech-news-5) ⭐️ 8.0/10

**财经新闻**
1. [人社部就新就业形态劳动者权益保障办法征求意见](#item-finance-news-1) ⭐️ 8.0/10
2. [OpenAI 年化收入据报约 500 亿美元，低于此前报道](#item-finance-news-2) ⭐️ 8.0/10
3. [巴西大选：博索纳罗家族及其盟友大获全胜](#item-finance-news-3) ⭐️ 7.0/10
4. [欧洲如何应对新一轮“中国冲击”](#item-finance-news-4) ⭐️ 7.0/10
5. [京东拟 25 亿美元收购德国 Ceconomy，欧盟 11 月 4 日前作最终裁决](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Lean 验证 AI 数学形式化不保证原自然语言证明正确](https://arxiv.org/abs/2610.08144) ⭐️ 8.0/10

一篇 arXiv 文章指出，用 Lean 对 AI 自动形式化的数学文本进行验证，并不能保证原始自然语言证明的正确性，因为语义忠实的翻译在可解复杂度指数（SCI）层级中处于任意高的位置（SCI = ∞）。文章强调，解决数学自然语言文本中的歧义是实现语义忠实翻译的必要条件，而这一问题的难度高于包括停机问题（SCI = 1）在内的任何计算问题。作者给出了多个 AI 将自然语言陈述和证明误译为 Lean 的实例，导致自然语言证明与其 Lean“验证”之间出现不匹配，其中包括 OpenAI 宣布的 Navier-Stokes 方程解爆破证明。文章特别指出，形式化的 Lean 证明与 Navier-Stokes 方程解爆破的自然语言证明并不对应。

rss · Lobsters · 10月8日 17:16

**「背景」** 自动形式化（autoformalisation）指用 AI 系统将自然语言数学文本翻译为 Lean 等形式化语言，随后由机器机械地验证形式化论证。OpenAI 曾公布关于 Navier-Stokes 方程解爆破（blow-up）的证明，并公开了手稿与 Lean 形式化版本，该结果针对 Clay 问题选项 C 和 D（光滑外力情形），目前仍存在争议。本文作者为 Alexander Bastounis 等三人，其核心论点是：由于自然语言数学文本中的歧义消解在可解性复杂度指数（SCI）层级中处于任意高的位置（SCI = ∞），语义忠实的翻译在计算上比停机问题（SCI = 1）还要困难。

**「影响」** 该结果直接削弱了以 Lean 形式化验证作为 AI 生成数学证明正确性依据的可信度，尤其针对 OpenAI 所宣称的 Navier-Stokes 方程解爆破证明：论文指出其 Lean 形式化证明与原始自然语言证明并不对应。对依赖 autoformalisation 验证 AI 数学输出的研究者与机构而言，这意味着形式化通过不能替代对自然语言论证本身的审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.08144">[2610.08144] Navier - Stokes lost in translation: Why Lean verification...</a></li>
<li><a href="https://dev.to/axrisi/navier-stokes-solved-what-openais-proof-shows-and-why-its-disputed-4a31">Navier - Stokes solved? What OpenAI &#x27;s proof ... - DEV Community</a></li>
<li><a href="https://www.datacamp.com/blog/openai-navier-stokes-math-problem">Did AI Solve Navier - Stokes ? OpenAI &#x27;s Claim, Explained | DataCamp</a></li>
<li><a href="https://arxiv.org/pdf/2610.08144">Navier-Stokes lost in translation: Why Lean verification of AI...</a></li>
<li><a href="https://jbenartzi.github.io/papers/SCI_STOC_Final.pdf">The Solvability Complexity Index - Computer Science and Logic</a></li>
<li><a href="https://www.youtube.com/watch?v=HxidCCh6eIM">Anders Hansen: What is the Solvability Complexity Index ... - YouTube</a></li>

</ul>
</details>

**标签**: `#autoformalisation`, `#Lean`, `#AI for mathematics`, `#formal verification`, `#Navier-Stokes`

---

<a id="item-tech-news-2"></a>
### [Let&\#x27;s Encrypt 将于 2027 年 2 月启用 64 天证书有效期](https://letsencrypt.org/2026/10/07/64-day-certs.html) ⭐️ 8.0/10

Let&\#x27;s Encrypt 宣布计划于 2027 年 2 月起将 TLS 证书有效期缩短至 64 天。这一变化对 Web PKI 生态具有重要影响，因为 Let&\#x27;s Encrypt 为大量网站提供证书，任何有效期调整都会直接波及依赖其证书的站点与自动化续期流程。对于手动管理证书或续期自动化不完善的运维者而言，64 天的周期意味着更新频率显著提高，需要提前调整部署与监控策略。目前该消息本身仅包含公告链接与评论入口，未提供更多技术细节。

rss · Lobsters · 10月8日 19:06

**「背景」** TLS 证书用于加密网站与用户之间的连接，其有效期历来由证书颁发机构（CA）设定，早期常见为一年甚至更长。缩短证书有效期被视为降低密钥泄露和证书误签发风险的手段，但代价是站点必须更频繁地续期，因此自动化续期协议 ACME 成为关键基础设施。Let&\#x27;s Encrypt 是提供免费证书的主要 CA 之一，其此次调整还伴随验证时间线的压缩：授权复用期将从 30 天缩短至 10 天，并计划到 2028 年进一步降至 7 小时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/gadgets/2026/10/lets-encrypt-cuts-certificate-lifetimes-to-64-days-starting-february-2027/">Let &#x27; s Encrypt cuts certificate lifetimes to 64 days starting February ...</a></li>
<li><a href="https://www.geekslop.com/technology-articles/computers-programming/hacking-and-security-technology-articles/2026/lets-encrypt-64-day-ssl-certs">Let &#x27; s Encrypt Cuts SSL Cert Lifetimes To 64 Days ... - Geek Slop</a></li>

</ul>
</details>

**标签**: `#TLS certificates`, `#Let&\#x27;s Encrypt`, `#web PKI`, `#infrastructure`, `#security`

---

<a id="item-tech-news-3"></a>
### [FAST 发现首例演化中脉冲星原生三体系统](https://www.ithome.com/1/010/830.htm) ⭐️ 8.0/10

中国科学院国家天文台韩金林研究员团队结合 FAST 射电观测与国际光学、伽马射线望远镜的多波段数据，确认脉冲星 J0435+3233 属于首例尚在演化阶段的原生三体系统，这也是第二例被确认的脉冲星三体系统，成果于 2026 年 10 月 9 日发表于《天体物理学杂志快报》（ApJL）。该脉冲星于 2020 年 6 月 8 日由 FAST 漂移扫描巡天发现，自转周期仅 3.2 毫秒；新疆天文台团队利用 FAST 持续监测五年，获得 192 次测量结果，发现它与一颗白矮星以 8 天周期沿圆形轨道互绕，且自转周期每年增加 1 纳秒，比同类脉冲星高出两个量级，该阶段成果已于 2026 年 4 月刊发于《自然·天文》。第二伴星是一颗质量与太阳几乎相同、仍在演化的类太阳恒星，以 73.5 年周期、偏心率 0.6 的偏心轨道环绕脉冲星-白矮星双星系统，正是它引发了此前观测到的自转周期异常增大。研究还结合 Gaia、2MASS、PanSTARRS 档案数据以及费米卫星 18 年累积的 160 个有效伽马光子，精准锁定了光学伴星并证实三体结构；欧洲团队独立分析类似数据得出相同结论，但中国团队因充分考虑三星系统内引力交互与多种相对论效应，确定的几何构型和轨道参数精度高出一个量级，并精确测定了三体成员质量。

rss · IT HOME · 10月9日 02:30

**「背景」** 脉冲星三体系统指一颗脉冲星与两颗伴星在引力作用下相互绕转的系统，此前人类确认的唯一一例由一颗脉冲星和两颗白矮星构成，三颗恒星均已演化终结。原生三体系统则指三颗恒星源于同一云团、如同“三胞胎”般共同形成，其演化阶段和轨道构型能反映恒星形成与演化的完整历史。FAST（中国天眼）是目前世界上最大的单口径射电望远镜，其高灵敏度使探测毫秒脉冲星及其微弱伴星信号成为可能。

**「影响」** 该原生演化三体系统具有清晰显著的三体引力交互效应，可作为验证强等效原理等基础引力理论的优质天然观测平台，为研究三星系统复杂演化机制和极端环境天体物理规律提供珍贵样本。

**标签**: `#astronomy`, `#FAST telescope`, `#pulsars`, `#scientific research`, `#multi-band observation`

---

<a id="item-tech-news-4"></a>
### [陶哲轩质疑 OpenAI 的 719 篇 AI 数学证明](https://www.ithome.com/1/010/795.htm) ⭐️ 8.0/10

OpenAI 于 10 月 6 日在 GitHub 发布 722 份 AI 生成数学手稿，涵盖 372 个数学结果族并涉及数百项开放研究问题，后因一处符号错误及其连锁影响于 10 月 7 日撤回 3 份，现公开目录为 719 份。OpenAI 称发布前曾咨询普林斯顿高等研究院主持的“数学与人工智能顾问小组”（AGMAI）并参考其公开建议，但该小组此前要求前沿 AI 实验室停止在专有、外界无法访问的模型上测试高难度数学问题，并披露模型名称、提示词、推理链、耗时及计算成本；此次 OpenAI 仍使用专有模型，且仅 10 份手稿附有模型推理链，约 42% 的证明未经形式化处理，也未提供将自然语言证明与形式化产物关联的机器可读元数据。AGMAI 声明其咨询角色不构成对 OpenAI 获取或发布这些结果的认可，最终仍需由数学界评估相关建议是否得到充分执行。菲尔兹奖得主陶哲轩于 10 月 7 日在 mathstodon 发帖表示不反对 AI 做数学，但强烈反对把“用 AI 快速攻克著名难题”当成主要目标或产品展示，认为这会破坏数学共同体赖以运转的理解、教学、合作与开放探索机制，并称当前状况为数学界的“证明消化不良”。

rss · IT HOME · 10月9日 01:40

**「背景」** “数学与人工智能顾问小组”（AGMAI）是一个就前沿 AI 用于数学研究向实验室提供建议的咨询机构，数学家陶哲轩与 Martin Hairer 等均参与其中；AGMAI 明确表示其咨询角色不构成对 OpenAI 获取或发布这些结果的认可，最终评估需由数学界完成。陶哲轩是加州大学洛杉矶分校（UCLA）数学教授、2006 年菲尔兹奖得主，长期积极使用 AI 辅助研究，此前曾借助 AI 工具将 Green-Tao 定理推广到高次多项式。

**「影响」** 对数学界而言，这批成果的可审查性受限：约 42%的证明已翻译为 Lean 形式化验证，但其余部分缺乏形式化处理，且仅 10 份手稿附有推理链，数学家难以据此复核或学习。AGMAI 明确其咨询角色不构成对 OpenAI 发布行为的认可，最终评估权仍在数学界，这意味着 OpenAI 的发布流程可能面临持续的方法论质疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agmai.org/">agmai .org</a></li>
<li><a href="https://proofsandprompts.com/2026/09/22/why-i-agreed-to-join-agmai/">Why I agreed to join AGMAI – Proofs and Prompts</a></li>
<li><a href="https://terrytao.wordpress.com/2026/09/22/why-i-agreed-to-join-agmai/">Why I agreed to join AGMAI | What&#x27;s new</a></li>
<li><a href="https://mathstodon.xyz/@tao">Terence Tao (@ tao @ mathstodon .xyz) - Mathstodon</a></li>
<li><a href="https://www.webpronews.com/terence-tao-extends-green-tao-theorem-to-polynomials-with-ai/">Terence Tao Extends Green- Tao Theorem to Polynomials with AI</a></li>
<li><a href="https://www.implicator.ai/openai-372-math-results-mathematicians-race-to-read/">OpenAI &#x27;s 372 AI Math Results Leave Mathematicians Racing</a></li>
<li><a href="https://www.zerohedge.com/political/bunker-mode-openais-jaw-dropping-math-blitz-draws-boycott-warning-over-crypto-wallets">&#x27;Bunker Mode&#x27;: OpenAI &#x27;s Jaw-Dropping Math Blitz Draws... | ZeroHe...</a></li>

</ul>
</details>

**标签**: `#AI for mathematics`, `#OpenAI`, `#formal verification`, `#research transparency`, `#peer review`

---

<a id="item-tech-news-5"></a>
### [字节 Seed 团队揭示 DeepSeek 长上下文“抽风”源于相位敏感性](https://www.ithome.com/1/010/780.htm) ⭐️ 8.0/10

字节 Seed 团队于今年 9 月底在预印本平台 arXiv 提交论文，指出分块 KV 缓存压缩引入的“相位敏感性”是 DeepSeek 长上下文表现不稳定的原因。研究评估了基础版与后训练版的 DeepSeek-V4-Flash、DeepSeek-V4-Pro，以及后训练后的 DeepSeek-V4.1-Flash。分块 KV 缓存压缩以固定步幅将连续标记窗口压缩为更少缓存条目，可降低长上下文推理的内存与注意力成本，但同时引入 Token 相位这一新位置坐标，即其相对于压缩窗口边界的位置。团队发现此类模型存在系统性不对称：相同信息在某一相位易于检索，在另一相位则难以检索，这种周期性变化即相位敏感性；在采用该压缩的大型开放权重模型中，长上下文检索准确度在不同相位间可相差高达 40 个百分点，说明平均基准分数可能掩盖周期性弱点。

rss · IT HOME · 10月9日 00:49

**「背景」** 字节跳动是一家总部位于北京海淀区的中国互联网技术公司，由张一鸣、梁汝波等人于 2012 年创立，旗下拥有抖音/TikTok、今日头条、剪映等内容平台。其 Seed 团队是公司从事前沿人工智能研究的团队，此次在 arXiv 上提交的预印本论文即出自该团队。KV 缓存是 Transformer 类大模型在推理时用于存储历史键值对、避免重复计算的核心机制，而分块 KV 缓存压缩通过将连续 token 窗口压缩为更少缓存条目来降低长上下文推理的内存与注意力开销，是当前长上下文优化的重要方向之一。

**「影响」** 对采用分块 KV 缓存压缩的长上下文服务而言，平均基准分数可能掩盖高达 40 个百分点的相位性检索波动，使依赖长文档检索的应用在特定 token 位置上出现难以预测的准确率下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/ByteDance">ByteDance - Wikipedia</a></li>
<li><a href="https://www.bytedance.com/en/">ByteDance - Inspire Creativity, Enrich Life</a></li>
<li><a href="https://jaehun.me/en/posts/paper-2610-02953v1/">SlimKV: Joint Token-Feature KV Cache Compression ... | Jaehun&#x27;s Blog</a></li>
<li><a href="https://www.linkedin.com/pulse/turboquant-next-phase-llm-inference-near-optimal-online-krish-gupta-3cgec">TurboQuant and the next phase of LLM inference: near-optimal online...</a></li>

</ul>
</details>

**标签**: `#long-context`, `#KV-cache`, `#DeepSeek`, `#LLM inference`, `#research paper`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [人社部就新就业形态劳动者权益保障办法征求意见](https://mp.weixin.qq.com/s/saqkOXlhe0wX7qD83vdkRw) ⭐️ 8.0/10

10 月 8 日，人力资源社会保障部发布《新就业形态劳动者权益保障办法（征求意见稿）》，即日起至 11 月 8 日公开征求意见。办法覆盖网约车司机、外卖骑手、网络主播等群体，规定正常劳动报酬不得低于当地最低工资标准，连续工作 4 小时应保障适当休息，停止派单、封禁账号等重大决定须经人工审核，不得滥用罚款等惩罚性措施。

telegram · zaihuapd · 10月8日 09:23

**「背景」** 新就业形态劳动者通常指通过平台接单、而非与平台签订传统劳动合同的网约车司机、外卖骑手和网络主播等群体。此次人社部发布的是征求意见稿，并非最终生效的法律，公众可在 11 月 8 日前提出意见。

**「影响」** 若该征求意见稿最终落地，网约车司机、外卖骑手、网络主播等新就业形态劳动者的报酬、休息和账号封禁将受最低工资、连续工作 4 小时休息及人工审核等规则约束，相关平台企业的派单、算法和罚款管理方式也需相应调整。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.17173.com/content/10082026/180506121.shtml">news.17173.com/content/10082026/180506121.shtml</a></li>

</ul>
</details>

**标签**: `#labor policy`, `#gig economy`, `#regulation`, `#China`, `#platform workers`

---

<a id="item-finance-news-2"></a>
### [OpenAI 年化收入据报约 500 亿美元，低于此前报道](https://www.ft.com/content/b66a9858-f8fb-46cb-b506-44bfe26fca2a?syn-25a6b1a6=1) ⭐️ 8.0/10

据《金融时报》报道，投资者获得的财务文件显示，OpenAI 截至 9 月底的年化收入接近 500 亿美元，比此前广泛报道的 700 亿美元少约 200 亿美元。报道称，这一差异部分源于计算口径不同：Anthropic 计入通过 AWS、谷歌云等云伙伴销售的收入，OpenAI 则未计入；OpenAI 拒绝置评。

telegram · zaihuapd · 10月8日 17:22

**「背景」** 此前多家媒体报道称，OpenAI 的年化收入已接近 700 亿美元，其中 Axios 援引知情人士称企业销售自 7 月以来翻了一倍以上。年化收入是把某一时段的收入按全年折算的估算值，并非经审计的全年实际收入。

**「影响」** 消息公布后，英伟达、甲骨文、CoreWeave 等 AI 相关股票下跌，显示投资者正据此重新评估 AI 需求预期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.axios.com/2026/09/29/scoop-openais-annual-recurring-revenue-nears-70b">Scoop: OpenAI &#x27;s annual recurring revenue nears $ 70 B</a></li>
<li><a href="https://www.pymnts.com/news/artificial-intelligence/2026/openai-annualized-revenue-nears-70-billion-amid-enterprise-growth/">PYMNTS | OpenAI Annualized Revenue Nears $ 70 B Amid Enterprise...</a></li>
<li><a href="https://www.rkjdev.com/blog/openai-revenue-run-rate-nears-70-billion/">OpenAI Revenue Run Rate Nears $ 70 B as Sales Surge | rkj dev</a></li>
<li><a href="https://www.cnbc.com/2026/10/08/open-ai-revenue-nvidia-oracle-coreweave.html">Nvidia, Oracle, other AI stocks sink on OpenAI revenue report</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI industry`, `#revenue reporting`, `#private company financials`, `#investor sentiment`

---

<a id="item-finance-news-3"></a>
### [巴西大选：博索纳罗家族及其盟友大获全胜](https://www.economist.com/the-americas/2026/10/08/brazil-falls-into-magas-orbit) ⭐️ 7.0/10

据《经济学人》报道，巴西大选由博索纳罗家族及其盟友横扫获胜。该报道未提供具体席位、得票率或政策细节。

rss · The Economist · 10月8日 13:01

**「背景」** 博索纳罗家族长期活跃于巴西政坛：雅伊尔·博索纳罗自 1991 年起连续担任联邦众议员，后于 2019 年至 2023 年出任巴西总统。据《卫报》报道，其子、参议员弗拉维奥·博索纳罗在 2026 年 10 月首轮总统选举中意外领先现任总统卢拉·达席尔瓦，进入第二轮投票。

**「影响」** 若博索纳罗阵营及其盟友在选举中获胜并主导政策方向，巴西与美国、中国的贸易和外交关系可能面临调整；博索纳罗方面已表示愿同时与美中合作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jair_Bolsonaro">Jair Bolsonaro - Wikipedia</a></li>
<li><a href="https://www.theguardian.com/world/2026/oct/05/flavio-bolsonaro-brazilian-presidency-election-shock-first-round-victory">Flávio Bolsonaro poised to win Brazilian presidency... | The Guardian</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-08/brazil-election-bolsonaro-says-he-d-work-with-us-china-as-president">Brazil Election : Bolsonaro Says He’d Work With US... - Bloomberg</a></li>

</ul>
</details>

**标签**: `#Brazil`, `#elections`, `#politics`, `#emerging markets`, `#Bolsonaro`

---

<a id="item-finance-news-4"></a>
### [欧洲如何应对新一轮“中国冲击”](https://www.economist.com/leaders/2026/10/08/how-europe-should-deal-with-the-new-china-shock) ⭐️ 7.0/10

《经济学人》在一篇社论中指出，欧洲应对新一轮来自中国的经济压力，仅靠囤积“二次打击”式的贸易反制武器是不够的。该文认为欧盟需要一套更完整的对华贸易战略。

rss · The Economist · 10月8日 13:01

**「背景」** 《经济学人》这篇社论以“新一轮中国冲击”为背景，讨论欧盟应如何应对来自中国的经济压力。文章标题下的副题指出，仅靠积累“二次打击”式的贸易反制武器并不足够，但现有材料只有标题和副题，未提供具体数据或详细政策方案。

**「影响」** 若欧盟动用其从未启用的“反胁迫工具”，可对中国的商品与服务出口实施限制，这将对依赖中国稀土和磁铁等关键供应的欧洲制造商构成直接风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ft.com/content/4416101f-5072-4ee0-aa12-5b1daf25b31b?syn-25a6b1a6=1">Germany and France agree on last-resort tool against trade threats</a></li>
<li><a href="https://www.euractiv.com/news/von-der-leyen-hints-at-trade-bazooka-against-chinas-rare-earth-chokehold/">Von der Leyen hints at ‘ trade bazooka’ against China &#x27;s rare... | Euractiv</a></li>

</ul>
</details>

**标签**: `#EU trade policy`, `#China`, `#trade tensions`, `#industrial policy`

---

<a id="item-finance-news-5"></a>
### [京东拟 25 亿美元收购德国 Ceconomy，欧盟 11 月 4 日前作最终裁决](https://www.ithome.com/1/010/783.htm) ⭐️ 7.0/10

京东以约 25 亿美元收购德国电子产品零售商 Ceconomy 的交易已获德国、法国和意大利监管机构批准，目前等待欧盟委员会依据《外国补贴条例》在 11 月 4 日前作出最终决定。京东于 2025 年 7 月以每股 4.60 欧元发出自愿现金收购要约，对 Ceconomy 估值约 22 亿欧元，要约完成后预计持股约 85.2%。

rss · IT HOME · 10月9日 01:03

**「背景」** Ceconomy 旗下拥有 MediaMarkt、Saturn 等欧洲消费电子零售品牌；欧盟委员会 2026 年 5 月启动深入调查，7 月向京东发出异议声明，关注京东是否曾获得可能扭曲欧盟市场竞争的优惠融资、税收优惠或政府补助，京东随后提出并优化了补救方案。

**「影响」** 若交易获批，京东将获得 Ceconomy 在欧洲的零售网络，并承诺以市场价格向 Ceconomy 开放其在欧洲的物流和技术能力，同时允许规模较小的竞争对手以公平、非歧视条件使用相关服务。

**标签**: `#M&amp;A`, `#EU regulation`, `#retail`, `#cross-border investment`, `#JD.com`

---