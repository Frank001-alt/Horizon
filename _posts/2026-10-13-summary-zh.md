---
layout: default
title: "Horizon Summary: 2026-10-13 (ZH)"
date: 2026-10-13
lang: zh
---

> 从 193 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [黑客远程触发欧洲超市冷柜除霜，暴露物联网安全隐患](#item-tech-news-1) ⭐️ 8.0/10
2. [开发者将 WiFi 7 路由器改造为 320Msps SDR 接收器](#item-tech-news-2) ⭐️ 8.0/10
3. [80 岁供体血细胞重编程为分子年龄低于 20 岁的干细胞](#item-tech-news-3) ⭐️ 8.0/10
4. [Python 3.15 发布：PEP 810 惰性导入与采样分析器](#item-tech-news-4) ⭐️ 8.0/10
5. [谷歌基础设施中 90,000 美元远程代码执行漏洞](#item-tech-news-5) ⭐️ 8.0/10
6. [华为首次公布麒麟 9050 Pro 芯片架构图](#item-tech-news-6) ⭐️ 8.0/10
7. [微软发布 Maia 300 自研 AI 芯片，明年拟部署超百万颗](#item-tech-news-7) ⭐️ 8.0/10
8. [英伟达开放 Vera Rubin 机架设计并发布多项 AI 基础设施标准](#item-tech-news-8) ⭐️ 8.0/10
9. [SK 海力士发布 SSD 专用处理器架构 H-TPU](#item-tech-news-9) ⭐️ 8.0/10
10. [英伟达与思科发布首款 400G/lane 可插拔光模块规范 USFP](#item-tech-news-10) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [黑客远程触发欧洲超市冷柜除霜，暴露物联网安全隐患](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

据路透社、BBC 和《世界报》报道，法国超市连锁 Intermarche 等欧洲零售商遭遇网络攻击，黑客入侵联网的制冷控制器，远程激活自动除霜功能，导致冷柜被迫停机，约 150 家门店受影响。攻击还波及配送环节和门店价格显示系统。安全研究机构 Claroty 的 Team82 此前披露了 Danfoss 制冷控制器中的多个漏洞，涉事设备包括已停止支持的旧型号，如 Danfoss SM800（2021 年终止支持）和 SC355（2016 年终止支持）。该事件凸显了零售关键基础设施中 OT/IoT 设备联网带来的安全风险。

hackernews · Zeekaas · 10月12日 12:16 · [社区讨论](https://news.ycombinator.com/item?id=50055304)

**「背景」** Danfoss 的 AK-SM 800A 系列是超市制冷系统中广泛使用的联网控制器平台，用于远程监控、诊断和启动除霜等操作。2026 年 8 月，Claroty 的 Team82 研究团队披露了该平台存在的多个漏洞，Danfoss 随后发布了安全公告并建议安装 4.3.1 版本补丁。此次欧洲超市冰箱遭攻击事件，正是在这一已公开的漏洞背景下发生的。

**「影响」** 此次攻击直接冲击欧洲超市的冷链运营，并波及客户数据：Intermarché 的 Drive 配送服务遭攻击，约 287,605 名客户（占其 200 万用户的一部分）的姓名、电话、送货地址、出生日期和订单号被泄露。对仍在使用已停止支持（EOS）的 Danfoss SM800、SC355 等控制器的零售企业而言，这一事件表明将制冷控制器接入互联网会同时带来运营中断与数据泄露风险。

**「社区讨论」** 评论者指出，涉事设备多为 15 至 20 年前的旧控制器，因缺乏预算而长期未更换，并认为轮班劳动群体难以获得安全审查和定期设备更新等资源。有评论者以医院实验室设备需付费订阅才能运行、因而必须联网为例，反驳“为何要把冷柜连上互联网”的质疑。还有人提到 Danfoss 官方曾宣传联网可远程诊断和节能，并猜测此次攻击可能与 2026 年 8 月美国军事基地冷柜事件相关，或为同一团伙所为。

<details><summary>参考链接</summary>
<ul>
<li>Uncovering Vulnerabilities in Danfoss Refrigeration Controllers | Claroty</li>
<li>DSA-2025-08-01 - Danfoss</li>
<li><a href="https://www.connexionfrance.com/news/intermarche-cyberattack-affects-nearly-300000-customers/806317">Intermarché cyberattack 2026 : Nearly 300,000 customers&#x27; data stolen...</a></li>
<li><a href="https://torwire.com/news/cybersecurity/intermarche-drive-service-data-breach/">Cyberattack on Intermarché Drive Service Exposes Data of... - TorWire</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#IoT/OT security`, `#embedded systems`, `#critical infrastructure`, `#vulnerability disclosure`

---

<a id="item-tech-news-2"></a>
### [开发者将 WiFi 7 路由器改造为 320Msps SDR 接收器](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

开发者 h0m3us3r 在 GitHub 上发布项目 w1700k-sdr，演示如何将一台 WiFi 7 路由器改造成 320 Msps 的软件定义无线电（SDR）接收器。该项目在 Hacker News 上引发强烈关注，被认为在低成本硬件改造方面具有较高价值。社区评论指出，由于采用相同芯片组，这一方案很可能同样适用于内置 PCIe（用于 NVMe）的 Banana Pi R4。有评论者表示，在 5 GHz 频段实现 320 Msps 接收，目前很难找到更便宜的方案。该开发者此前还曾用 ESP32 Wi-Fi 微控制器做出过 SDR（eSpDR）。

hackernews · djfergus · 10月12日 12:41 · [社区讨论](https://news.ycombinator.com/item?id=50055593)

**「背景」** 软件定义无线电（SDR）用可编程数字信号处理替代传统模拟射频电路，让同一套硬件通过软件切换频段与调制方式。此前低成本 SDR 方案多基于 RTL-SDR（RTL2832U）等专用接收芯片，采样率通常仅数 Msps，而该项目利用 WiFi 7 路由器芯片实现 320 Msps 接收，属于对通用无线芯片的再利用。

**「影响」** 该项目的实际影响集中在低成本 SDR 与硬件改造社区：开发者可将同款 WiFi 7 芯片组的路由器（如社区指出的 Banana Pi R4）改造成 320 Msps 接收机，从而以远低于传统方案的成本获得 5 GHz 频段的高采样率接收能力。不过其适用性目前主要基于社区对同芯片组的推断，尚未见官方兼容性验证。

**「社区讨论」** 社区普遍对该项目表示赞赏，认为它有望推动更多常见 Wi-Fi 网卡被改造成低成本 SDR，让普通笔记本也能承担相关应用。有评论者根据芯片组相同这一点推测该方案可用于 Banana Pi R4，并强调这是目前 5 GHz 下 320 Msps 接收的低成本途径。也有评论者由此延伸讨论手机 FM 收音机是否因软件定义而受到厂商限制，以及用桌面 CNC、廉价 PCB 和常见元件自制业务监测设备的可能性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://radiohooligan.ru/hdsdr-dlya-rtl-sdr/">HDSDR — установка и настройка программы для приемника...</a></li>
<li><a href="https://www.rtl-sdr.com/foxsdr-updates-node-canvas-single-map-display-linuxandroid-builds-locating-air-traffic-radar-positions/comment-page-100/">FoxSDR Updates: Node Canvas, Single Map Display, Linux+Android...</a></li>
<li><a href="https://wiki.banana-pi.org/Banana_Pi_BPI-R4">Banana Pi BPI- R 4 - Banana Pi Wiki</a></li>

</ul>
</details>

**标签**: `#SDR`, `#WiFi 7`, `#hardware hacking`, `#open source`, `#wireless`

---

<a id="item-tech-news-3"></a>
### [80 岁供体血细胞重编程为分子年龄低于 20 岁的干细胞](https://doi.org/10.1111/acel.70751) ⭐️ 8.0/10

一项发表于《Aging Cell》的研究报告称，来自 80 岁供体的血细胞被重编程为诱导多能干细胞，其分子年龄低于 20 岁。该结果在细胞重编程与衰老研究领域引发关注，因为它提示衰老相关的分子特征可能在一定程度上被逆转。研究涉及的具体重编程方法、分子年龄评估指标、样本量及可重复性等细节需以同行评议论文为准。目前这仍属早期实验室发现，尚不能直接等同于组织或机体层面的衰老逆转，也未证明临床安全性或有效性。

hackernews · arunc · 10月12日 23:34 · [社区讨论](https://news.ycombinator.com/item?id=50064536)

**「背景」** 细胞重编程技术可将成体细胞（如血细胞）转化为诱导多能干细胞（iPSC）等具有分化潜能的细胞，是再生医学与衰老研究的重要工具。表观遗传时钟通过检测 DNA 甲基化等分子标记来估算细胞的“分子年龄”，常被用于衡量重编程或抗衰老干预的效果。此前研究多关注胚胎干细胞或年轻供体细胞，而本次研究由德国波恩大学团队主导，将 80 岁供体的红细胞前体直接重编程为神经干细胞，并在超过 100 天的过程中观察到表观遗传时钟从约 80 岁逐步重置到 20 岁以下。

**「影响」** 该结果为将衰老供体细胞用于再生医学和疾病建模提供了概念验证，但尚属早期研究，距离体内组织再生或抗衰老疗法仍有距离。

**「社区讨论」** Hacker News 评论者对此反应不一：有人表示受此类新闻激励而更关注自身健康，希望活到衰老干预成熟之时；也有人将其类比为灯塔水母的细胞重置机制，并指出该过程可能对遗传缺陷高度敏感。另有评论提到 Michael Levin 关于生物电与细胞重编程的研究作为相关背景，同时有人担忧此类技术若被用于组织层面可能带来伦理与权力风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medicalxpress.com/news/2026-10-blood-cells-year-donor-stem.html">Blood cells from 80-year-old donor become stem cells with ...</a></li>
<li><a href="https://nautil.us/blood-cells-from-an-80-year-old-transformed-into-young-brain-cells-1285722">Blood Cells From an 80-Year-Old Transformed into Young Brain ...</a></li>
<li><a href="https://bioengineer.org/blood-cells-from-80-year-olds-rejuvenated-into-brain-cells-with-molecular-age-under-20/">Blood Cells From 80-Year-Olds Rejuvenated Into Brain Cells ...</a></li>
<li><a href="https://www.cell.com/trends/molecular-medicine/fulltext/S1471-4914%2826%2900011-0">Cellular reprogramming beyond pluripotency: Trends in ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1568163725000832">Conserved biological processes in partial cellular ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1471491426000110">Cellular reprogramming beyond pluripotency - ScienceDirect</a></li>

</ul>
</details>

**标签**: `#stem cells`, `#aging research`, `#cellular reprogramming`, `#biotechnology`, `#longevity`

---

<a id="item-tech-news-4"></a>
### [Python 3.15 发布：PEP 810 惰性导入与采样分析器](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 8.0/10

Python 3.15 已正式发布，官方 What&\#x27;s New 指南由 3.14 和 3.15 发布经理 Hugo van Kemenade 整理。本次最受关注的新特性是 PEP 810 显式惰性导入，允许使用 \`lazy import json\` 和 \`lazy from pathlib import Path\` 语法，模块会在符号首次被使用时才真正导入，直接缓解了插件等场景的启动开销。此外，PEP 798 为推导式引入了解包语法，例如 \`\[\*L for L in lists\]\` 等价于 \`\[x for L in lists for x in L\]\`，该语法是 2015 年 Python 3.5 中 PEP 448 解包特性的延伸。标准库还新增了名为 Tachyon 的高频统计采样分析器 \`profiling.sampling\`，原有追踪分析器从 \`cProfile\` 更名为 \`profiling.tracing\`。性能方面，Miguel Grinberg 基于 3.15.0rc3 的测试显示 3.15 与 3.14 基本持平，仅实验性 JIT 在 Fibonacci 测试中带来约 1.2 倍提升。

rss · Simon Willison · 10月12日 18:15

**「背景」** Python 每年发布一个新的大版本，社区通常需要等待旧版本结束支持后才能采用新语法特性。PEP 810 的惰性导入针对的是模块导入在进程启动时产生的固定成本，这一问题在依赖重型库（如 sentence\_transformers）的插件生态中尤为明显。采样分析器通过周期性抓取运行中进程的调用栈来估算各函数耗时，相比需要预先插桩的追踪分析器开销更低，此前开发者多依赖 py-spy 等第三方工具实现类似能力。

**「影响」** 维护需要兼容多个 Python 版本的开源库的开发者，现在可以告别 Python 3.10 并开始采用 3.11 的特性；而插件作者可借助 PEP 810 惰性导入消除重型依赖带来的启动延迟，无需再手动实现延迟加载。

**标签**: `#python`, `#programming-languages`, `#open-source`, `#language-releases`, `#pep-810`

---

<a id="item-tech-news-5"></a>
### [谷歌基础设施中 90,000 美元远程代码执行漏洞](https://simonkoeck.com/writeups/google-devsite-flask-session-pickle-rce) ⭐️ 8.0/10

安全研究员 Simon Koeck 发布了一份技术报告，详细描述了在谷歌基础设施中发现的一个远程代码执行漏洞，该漏洞获得了 90,000 美元的漏洞赏金。该漏洞源于 Flask 会话的 pickle 反序列化机制，攻击者可能借此在目标服务器上执行任意代码。报告指出，Flask 默认使用签名 Cookie 存储会话数据，若应用在反序列化会话内容时未做充分校验，攻击者便可构造恶意 pickle 载荷触发代码执行。该漏洞属于高严重性级别，对使用 Flask 框架的 Web 应用开发者具有重要警示意义。

rss · Lobsters · 10月12日 14:40

**「背景」** Flask 是一个 Python Web 框架，其默认的客户端会话机制使用签名 Cookie 存储会话数据。当应用配置了 SECRET\_KEY 后，Flask 会使用 Python 的 pickle 模块对会话内容进行序列化；若密钥泄露或可被猜测，攻击者即可构造恶意 pickle 数据，在服务器反序列化时触发远程代码执行（RCE）。pickle 模块本身设计用于序列化与反序列化 Python 对象，但反序列化不可信数据时存在已知的代码执行风险，这一特性在 Flask 会话场景中常被安全研究者用于演示漏洞利用。

**「影响」** 该漏洞表明，当 Flask 应用使用 pickle 序列化会话数据时，攻击者可通过构造恶意 pickle 对象在反序列化阶段执行任意代码，从而危及受影响服务及其数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/CalfCrusher/Python-Pickle-RCE-Exploit">GitHub - CalfCrusher/Python- Pickle - RCE -Exploit: Python Pickle RCE ...</a></li>
<li><a href="https://davidhamann.de/2020/04/05/exploiting-python-pickle/">Exploiting Python pickles | David Hamann</a></li>
<li><a href="https://www.sourcery.ai/vulnerabilities/python-flask-security-insecure-deserialization">Flask Insecure Deserialization Vulnerability | Security ... | Sourcery</a></li>
<li><a href="https://github.com/deepanshhooda/flask-kvsession-pickle-rce">GitHub - deepanshhooda/ flask -kvsession- pickle -rce: PoC...</a></li>
<li><a href="https://vulmon.com/vulnerabilitydetails?qid=CVE-2021-33026">CVE-2021-33026 - Remote Code Execution in Flask -Caching</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#remote-code-execution`, `#web-frameworks`, `#bug-bounty`

---

<a id="item-tech-news-6"></a>
### [华为首次公布麒麟 9050 Pro 芯片架构图](https://www.ithome.com/1/012/196.htm) ⭐️ 8.0/10

华为于 10 月 13 日在上海练秋湖举办 2026 麒麟媒体沟通会，华为半导体业务无线终端芯片产品管理部部长徐松余发表演讲，首次公布麒麟 9050 Pro 芯片的详细架构图（发布会上展示的是简要版本）。该芯片搭载新一代灵犀 CPU、新一代马良 GPU、新一代达芬奇架构 NPU、新一代麒麟 AI ISP，以及灵犀微核、FFTS 函数流任务调度器和安全处理器等组件。徐松余同时确认，首款逻辑折叠芯片麒麟 9050 系列在中国半导体产业界的支持下已成功量产。他同时指出该技术路径仍面临工具链与方法论、工艺差异补偿、跨层互联开销优化、能耗控制、基准测试方法等挑战，并呼吁半导体产业界与学术界加强合作，称未来属于开放合作，没有一家企业可以独自解答所有答案。

rss · IT HOME · 10月13日 02:34

**「背景」** 麒麟是华为旗下用于智能手机等终端设备的自研芯片系列，其架构通常包含 CPU、GPU、NPU 和 ISP 等模块。此次提到的“逻辑折叠”是华为在芯片设计上采用的一种新路径，旨在通过跨层设计与互联来提升集成度或性能，但该路径在工具链、工艺补偿和能耗控制等方面仍不成熟。华为此次公开架构图并确认量产，是其对外展示自研芯片进展的一部分。

**「影响」** 若麒麟 9050 系列确已量产，将意味着华为在逻辑折叠芯片路径上迈出从设计到落地的关键一步，但该技术的实际性能、良率与能效表现仍有待独立验证。

**标签**: `#semiconductors`, `#Huawei Kirin`, `#chip architecture`, `#AI hardware`, `#open source collaboration`

---

<a id="item-tech-news-7"></a>
### [微软发布 Maia 300 自研 AI 芯片，明年拟部署超百万颗](https://www.ithome.com/1/012/191.htm) ⭐️ 8.0/10

微软于当地时间周一发布第三代自研 AI 芯片 Maia 300，专门用于代码生成、代表用户执行复杂商业任务等 AI 数据运算，并计划从明年开始开展多吉瓦级规模部署、部署超百万颗芯片以支撑内部 AI 业务。该芯片采用与英伟达不同的 chiplet 架构，核心计算芯粒使用台积电 2 纳米工艺，负责数据传输与系统内调度的芯粒使用成本更低的 3 纳米工艺。Maia 300 服务器单机柜内置 96 颗芯片、整机功耗约 167 千瓦，而英伟达最新 GB300 机柜搭载 72 颗 GPU、功耗 142 千瓦。微软称 Maia 300 每兆瓦电力的有效计算量比“主流 GPU 系统”高出约 40%，但未指明具体对比产品；微软 Azure 硬件系统与基础设施总裁拉尼·博卡表示，通过全栈优化，该芯片能在每瓦功耗、每单位成本和每字节内存上输出更强智能处理能力。微软预计本自然年度资本开支超过 1,750 亿美元（约合 1.17 万亿元人民币）。

rss · IT HOME · 10月13日 02:25

**「背景」** 微软自研 AI 芯片 Maia 系列已迭代至第三代，上一代 Maia 芯片此前已用于运行微软自研模型以及 Azure 云平台上承载的 OpenAI 模型。当前各大云厂商与 OpenAI 等 AI 企业密集推出自研芯片，目标是打破英伟达在 AI 计算市场的主导地位。在架构路线上，英伟达 AI 加速器采用一颗巨型主计算芯片搭配高带宽内存，而微软 Maia 300 改用 chiplet 架构，将核心计算、内存控制器与 I/O 等功能拆分为多颗芯粒封装在一起。

**「影响」** 若微软明年按计划部署超百万颗 Maia 300，其内部 AI 算力将更多转向自研芯片，从而降低对英伟达 GPU 的采购依赖与算力成本；但该芯片能否拓展至 Anthropic 等外部客户仍不确定，目前报道仅基于厂商发布与单一高管表态，缺乏独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/1/012/115.htm">微软 Maia 300 AI 芯片发布：台积电 N2P 工艺，288GB HBM4 内存、带宽...</a></li>
<li><a href="https://technews.tw/2026/10/13/microsoft-maia-300-to-begin-production-deployments-in-2027/">微软 Maia 300 新晶片明年量产，关键运算 Chiplet 采台积电 N2P 制程 ...</a></li>
<li><a href="https://xueqiu.com/4885703643/404468806">深度解读如下｜ 微 软 Maia 300 寻求 台积电 30 万 枚产能，云厂商自研AI...</a></li>

</ul>
</details>

**标签**: `#AI 芯片`, `#微软`, `#数据中心硬件`, `#chiplet`, `#算力成本`

---

<a id="item-tech-news-8"></a>
### [英伟达开放 Vera Rubin 机架设计并发布多项 AI 基础设施标准](https://www.ithome.com/1/012/120.htm) ⭐️ 8.0/10

在开放计算项目（OCP）全球峰会上，英伟达宣布通过 NVIDIA MGX 架构向 OCP 贡献 Vera Rubin 机架与计算托架设计，并与 Cisco、Google、Meta、Microsoft、Visionbay 等联合发布多项 AI 基础设施开放标准。更新后的 MGX 1.2 规范新增机架级盲插式液冷、可互操作机架互连、液冷 5000A 母线及原生 19 英寸设备支持，支持最高 250kW 的机架部署。英伟达同时发布 DSX AI Factory 的 4 个开源软件组件，覆盖交换机配置、GPU 集群压力测试、机架固件管理和裸机部署，源自 DGX Cloud 运营经验。此外，英伟达与 AMD、Google、Meta 发布 Open Data Center Specification v0.7，统一 AI 工厂的供电、散热与物理布局设计；Google、Meta、Microsoft 与英伟达另发布电网弹性规范，要求大规模 AI 设施在电网扰动时保持连接并在不到 2 秒内恢复至接近满载。

rss · IT HOME · 10月13日 02:12

**「背景」** 开放计算项目（OCP）是推动数据中心硬件与固件开放标准的行业组织，英伟达此前已通过 MGX 架构向 OCP 贡献服务器设计。随着 AI 集群功耗与规模快速上升，机架级液冷、高电流供电和统一物理布局成为下一代 AI 工厂的关键工程问题。

**「影响」** 系统厂商可依据开放的 Vera Rubin 机架与计算托架设计开发下一代 AI 工厂基础设施，云服务商则有望借助 DSX 开源组件在数小时内将硬件部署为生产集群。

**标签**: `#AI infrastructure`, `#open standards`, `#datacenter hardware`, `#NVIDIA`, `#liquid cooling`

---

<a id="item-tech-news-9"></a>
### [SK 海力士发布 SSD 专用处理器架构 H-TPU](https://www.ithome.com/1/012/160.htm) ⭐️ 8.0/10

SK 海力士于 10 月 12 日正式推出名为 H-TPU（海力士事务处理单元）的 SSD 专用处理器架构，旨在克服传统通用 CPU 在功耗和面积上的限制。该架构并非用于 AI 计算的张量加速器，而是可编程处理器，专门控制 SSD 数据平面和处理事务，其核心思路是将控制功能拆解为功能单元，分布到数十个小型 TPU 集群中。SK 海力士 SoC 设计副总裁구인재在韩国仁川松岛举行的 ISOCC 2026 会议上表示，H-TPU 采用简化的四级流水线，排除了超标量和非顺序执行设备，占用面积仅为通用 CPU 核心的 1/25（约占总 CPU 面积的 4%），功耗仅约为 1/25%（约 2.5%）。只有与特定任务相关的功能模块才会工作，未使用的模块切换到最低功耗模式，从而大幅节省整个控制器的功耗。SK 海力士计划将该技术应用于包括下一代企业级 SSD（eSSD）控制器在内的各类 NAND 产品线，之后用于下一代 AI 存储架构 Storage Next，并预计与明年发布的新一代高带宽闪存 HBF 结合产生协同效应。

rss · IT HOME · 10月13日 01:15

**「背景」** 随着 AI 普及，数据中心性能瓶颈逐渐转移到内存和存储层。SK 海力士指出，虽然每一代 GPU 性能和 PCIe 带宽都在翻倍，但 SSD 控制器内部通用 CPU 的频率和控制能力已达到极限，传统单体 CPU 架构难以处理存储控制所需的数百个细节功能，并导致功耗浪费和不可预测的流水线延迟。

**「影响」** 若 H-TPU 的功耗和面积数据在实际产品中成立，下一代企业级 SSD 控制器有望显著降低控制功耗，并为 AI 存储架构 Storage Next 及明年发布的 HBF 高带宽闪存提供更高效的配套控制方案。目前尚无独立基准测试或商用产品验证这些指标。

**标签**: `#storage`, `#hardware-architecture`, `#ssd`, `#ai-infrastructure`, `#sk-hynix`

---

<a id="item-tech-news-10"></a>
### [英伟达与思科发布首款 400G/lane 可插拔光模块规范 USFP](https://www.ithome.com/1/012/155.htm) ⭐️ 8.0/10

英伟达与思科于当地时间 10 月 12 日宣布联合推出业界首款支持 400Gbps/lane 高速信号的可插拔光模块规范 USFP。该规范与 OSFP 光模块尺寸相当，首批产品集成 16 条全双工通道，后续可扩展至 32 条乃至更多通道，从而实现 12.8 Tb/s 的吞吐量。其带宽可达现有 200G/lane 可插拔光模块的 4 倍，在 400G SerDes 技术支持下能效为后者的 1.3 倍。USFP 采用新型二维阵列连接器，两步插入设计可在模块插入后才接合高速触点，从而减少触点磨损、提高信号完整性并使插入力更可预测，同时支持 100W 功耗以简化交换机设计。

rss · IT HOME · 10月13日 00:55

**「背景」** 可插拔光模块是数据中心与网络设备中用于光电信号转换的关键部件，其规范由多厂商共同制定以保障互操作性。OSFP 是当前广泛使用的可插拔光模块封装形式之一，而 200G/lane 是此前较高速率的信号标准。随着 AI 与云计算对带宽需求上升，业界正推动单通道速率向 400G/lane 演进。

**「影响」** 该规范为交换机和光模块厂商提供了向 400G/lane 及 12.8 Tb/s 吞吐量演进的统一接口参考，但作为规范发布，其实际产品落地与生态采用情况尚待观察。

**标签**: `#optical networking`, `#hardware`, `#NVIDIA`, `#Cisco`, `#data center interconnect`

---