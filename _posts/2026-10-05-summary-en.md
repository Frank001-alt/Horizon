---
layout: default
title: "Horizon Summary: 2026-10-05 (EN)"
date: 2026-10-05
lang: en
---

> From 154 items, 10 important content pieces were selected

---

**Technology News**
1. [华为麒麟 9050 Pro 裸片照曝光：双裸片垂直堆叠](#item-tech-news-1) ⭐️ 8.0/10
2. [Lam Research Proposes SA-CFET Architecture for Sub-1nm Nodes](#item-tech-news-2) ⭐️ 8.0/10
3. [Rust 成为微软内部一级编程语言](#item-tech-news-3) ⭐️ 8.0/10

**Financial News**
1. [FieldAI 拟以 100 亿美元估值融资 7 亿美元](#item-finance-news-1) ⭐️ 7.0/10
2. [US Arrests CEO Accused of Smuggling Over $300 Million in Nvidia AI Chips to China](#item-finance-news-2) ⭐️ 7.0/10
3. [台积电据报拟2027年一季度再上调先进晶圆价格6%~8%](#item-finance-news-3) ⭐️ 7.0/10
4. [China Trade-In Subsidies Drive 196.3 Billion Yuan in Holiday Sales](#item-finance-news-4) ⭐️ 7.0/10
5. [South Korea&\#x27;s President Orders Probe After Data Breaches at Major Banks](#item-finance-news-5) ⭐️ 7.0/10
6. [White House Creates AI Task Force to Report on Risks Within 120 Days](#item-finance-news-6) ⭐️ 7.0/10
7. [CCTV Exposes Fake &\#x27;Open Kitchen&\#x27; Livestreams at Food-Delivery Merchants; Hubei and Yunnan Launch Probes](#item-finance-news-7) ⭐️ 6.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [华为麒麟 9050 Pro 裸片照曝光：双裸片垂直堆叠](https://www.ithome.com/1/009/739.htm) ⭐️ 8.0/10

半导体分析机构 Kurnal Insights 于 9 月 30 日发布华为麒麟 9050 Pro 的裸片显微照，首次从物理层面展示其内部结构：两颗尺寸完全相同的裸片垂直堆叠，单颗尺寸 11.13 × 10.84 mm、面积约 120.65mm²，略小于前代麒麟 9030S 的 122mm²。两颗裸片分工明确，一颗负责核心计算逻辑，另一颗专用于 SRAM 和缓存，通过高密度垂直互连连接，这是华为韬定律“逻辑折叠”（LogicFolding）技术的首次商业化落地。何庭波在 ChinaXiv 署名论文中称，该芯片等效晶体管密度从麒麟 9030 Pro 的约 1.55 亿个/mm² 提升至约 2.38 亿个/mm²，增幅约 55%，相当于此前三年几何尺寸缩小成果的总和；在性能对齐条件下，NPU 功耗降低 66%、GPU 功耗降低 58%、CPU 性能核功耗降低 41%。据 @Taog\_1575 依据极客湾资料及 Die Shot 解析，逻辑裸片采用中芯国际 N+3 工艺，SRAM 裸片采用 N+2 工艺；单颗裸片面积缩小使其良率应高于麒麟 9030 Pro，但该芯片仅用于 Mate 90 Pro Max 及以上版本，整体封装良率可能仍然偏低。伯恩斯坦称其为“被低估的突破”，并指出良率与散热仍是 3D 堆叠大规模量产的工程挑战，同时认为该芯片将移动芯片与苹果的技术差距缩小至约三年（上一代约四年）。

rss · IT HOME · Oct 4, 23:26

**「Background」** Huawei semiconductor chief He Tingbo published a V2 version of her &quot;Tao&\#x27;s Law&quot; paper on ChinaXiv, adding the LogicFolding architecture and measured data; LogicFolding is described as the core engineering practice of that framework. The die-shot analysis was published by Kurnal Insights, a semiconductor intelligence platform that covers die shots, packaging, CMOS process, and process-node research. The Kirin 9050 Pro is a mobile SoC listed by Kurnal Insights as codename Hi36E0, with dimensions 11.13 × 10.84 mm, area 120.65 mm², and foundry SMIC.

**「Impact」** Bernstein estimates the Kirin 9050 Pro narrows Huawei&\#x27;s mobile-chip gap with Apple to about three years, down from roughly four, and reports it beats Apple&\#x27;s 3nm A17 Pro in Geekbench 6 multicore despite a 7nm-class node and no EUV. Yield and heat remain unresolved engineering challenges for large-scale 3D stacking.

<details><summary>References</summary>
<ul>
<li><a href="https://www.msn.com/zh-cn/news/other/%E4%BD%95%E5%BA%AD%E6%B3%A2%E5%8F%91%E5%B8%83%E5%8D%8E%E4%B8%BA-%E9%9F%AC%E5%AE%9A%E5%BE%8B-v2%E7%89%88%E8%AE%BA%E6%96%87-%E6%96%B0%E5%A2%9Elogicfolding%E6%9E%B6%E6%9E%84%E4%B8%8E%E5%AE%9E%E6%B5%8B%E6%95%B0%E6%8D%AE/ar-AA27i3I5">何 庭 波 发布 华 为 “ 韬 定 律 ”V2版 论 文 ，新增 LogicFolding 架构与实测数据</a></li>
<li><a href="https://www.cls.cn/detail/2417485">华 为 何 庭 波 发布V2版“ 韬 定 律 ” 论 文 这两个方向或迎最大增量机遇</a></li>
<li><a href="https://news.qq.com/rain/a/20260706A02G8L00">news.qq.com/rain/a/20260706A02G8L00</a></li>
<li><a href="https://kurnal-insights.com/en/">Kurnal Insights · Semiconductor Intelligence Platform</a></li>
<li><a href="https://kurnal-insights.com/en/dieshot/hisilicon-hi36e0-kirin-9050/">Hisilicon Hi36E0 (Kirin 9050) · Kurnal Insights</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2p3Z3AyR0VoRklmZFZPNkE2SHdDZ0FQAQ?hl=en-PK&amp;gl=PK&amp;ceid=PK:en">Google News - Bernstein analyzes Huawei Kirin 9050 Pro processor...</a></li>
<li><a href="https://www.scmp.com/tech/tech-trends/article/3368404/chinas-huawei-trims-mobile-chip-gap-apple-tau-scaling-law-pays-bernstein">China’s Huawei trims mobile chip gap with Apple as Tau Scaling Law...</a></li>
<li><a href="https://pandaily.com/bernstein-kirin-9050-pro-multicore-a17-pro-tau-scaling">Bernstein : Kirin 9050 Pro Multicore Tops A17 Pro as Huawei ...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#chip-design`, `#huawei-kirin`, `#advanced-packaging`, `#hardware`

---

<a id="item-tech-news-2"></a>
### [Lam Research Proposes SA-CFET Architecture for Sub-1nm Nodes](https://www.ithome.com/1/009/737.htm) ⭐️ 8.0/10

Lam Research has proposed a self-aligned complementary FET \(SA-CFET\) architecture aimed at extending CMOS transistors to 10 Å \(1nm\) and below, addressing challenges that conventional GAA nanosheet transistors face in leakage, mobility, parasitic resistance, and process variability. The architecture relies on three self-aligned process modules—SA-BPR \(self-aligned buried power rail\), SA-CT \(self-aligned contact\), and SA-TSV \(self-aligned through-silicon via\)—along with a non-metal gate cut design and middle dielectric isolation \(MDI\) for work-function separation, while maintaining compatibility with N3 specifications such as a 42nm contact gate pitch and 21nm metal pitch. Using SEMulator3D digital-twin process modeling, Lam Research&\#x27;s Semiverse Solutions team validated the flow and device structures, showing the architecture can build 6T SRAM cells and NOT, NAND, and NOR logic cells. The modeled 6T SRAM bit cell area is 0.0094 μm², which is 52.7% smaller than N3 and 19% smaller than an A7 CFET design. The results come from simulation-based design verification, not production hardware, and all critical contact layers reportedly have at least a 10nm overlay window with no open or short failures in the simulations.

rss · IT HOME · Oct 4, 22:55

**「Background」** As advanced process nodes push toward 1nm and below, silicon-based GAA nanosheet transistors are expected to face physical and manufacturing limits, including source-drain tunneling, mobility degradation, and rising contact and parasitic resistance. CFET architectures vertically stack NMOS and PMOS devices to increase density without relying solely on planar scaling, but they introduce complex metal gate isolation and contact crowding issues. Lam Research&\#x27;s SA-CFET proposal is a modeling study exploring self-aligned process integration for this direction, while imec&\#x27;s July roadmap predicts a 0.3nm \(A3\) node by 2038 and its September CFET update suggests the industry may shift to CFET-based transistors starting at the A7 logic node.

**「Impact」** If validated in hardware, SA-CFET could offer a path to smaller SRAM and logic cells for sub-1nm nodes while relaxing overlay requirements, but the current evidence is limited to digital-twin simulation and does not demonstrate production readiness.

**Tags**: `#semiconductor manufacturing`, `#transistor architecture`, `#advanced nodes`, `#SRAM scaling`, `#process modeling`

---

<a id="item-tech-news-3"></a>
### [Rust 成为微软内部一级编程语言](https://www.ithome.com/1/009/672.htm) ⭐️ 8.0/10

据 Rust 基金会，Rust 现已成为微软公司内部的“一级编程语言（Tier-1）”，与 C++、C\# 和 TypeScript 并列。这里的 Tier-1 是微软内部使用的分类，并非 Rust 项目自身的支持等级；对微软内部开发团队而言，这意味着无需再自行搭建 Rust 相关的开发和生产环境，微软将提供从代码编写、构建、测试到发布和长期维护的一整套标准流程，并将 Rust 项目纳入现有的软件安全、合规等开发流程。微软表示 Rust 已被应用于固件、驱动程序、内核、虚拟机监控程序、微服务和应用程序等多种软件，但由于 C++ 已在微软内部使用多年并广泛存在于 Windows 等大型项目中，未来很长一段时间内两者仍将并行使用。为促进协同，微软开发了 rustc\_codegen\_utc 项目，提供新的代码生成方式，让 Rust 编译器直接连接 Windows 平台 MSVC 工具链使用的代码生成后端，从而更好地与现有工具链及应用程序二进制接口（ABI）协同，并继续使用安全功能、调试工具、崩溃转储分析、性能分析、诊断、代码覆盖率、热补丁和编译优化能力。微软强调该项目并非实验性项目，从 2026 年初开始已具备生产环境使用条件，从 Rust 1.90 版本开始已能完成自身编译，目前已有超过 100 个微软项目代码库使用这一后端。

rss · IT HOME · Oct 4, 08:43

**「Background」** Rust is a systems programming language originally developed at Mozilla and now maintained by the Rust Foundation. Microsoft has used Rust in some teams for years, but those efforts were largely self-supported rather than part of a company-wide standard toolchain. The rustc\_codegen\_utc project connects the Rust compiler to the MSVC code-generation backend used by Microsoft&\#x27;s Windows toolchain, allowing Rust and C++ to share underlying infrastructure.

**「Impact」** Microsoft teams can now adopt Rust without building their own toolchains, since Rust is a fully supported standard option integrated with MSVC, security, compliance, and supply-chain processes. The rustc\_codegen\_utc backend lets Rust and C++ share one Windows-native infrastructure, reducing duplicated engineering for mixed-language projects.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://www.sohu.com/a/1083976260_122066679">Rust正式成为微软Tier-1编程语言，与C++并列_项目_生产_支持</a></li>
<li><a href="https://www.ithome.com/1/009/672.htm">Rust 正式成为微软内部一级编程语言，与 C++、C#、TypeScript 并列 - ...</a></li>
<li><a href="https://rust-lang.org/tools/install/">Install Rust - Rust Programming Language</a></li>
<li><a href="https://linux.do/t/topic/2977263">微软：加大 rust 力度， rust 现在是一级语言 - 前沿快讯 - LINUX DO</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Microsoft`, `#编程语言`, `#编译器工具链`, `#Windows`

---

## Financial News

<a id="item-finance-news-1"></a>
### [FieldAI 拟以 100 亿美元估值融资 7 亿美元](https://www.ithome.com/1/009/746.htm) ⭐️ 7.0/10

据《商业内幕》援引一位知情人士报道，机器人软件公司 FieldAI 正在融资 7 亿美元，投后估值达 100 亿美元，较其上一轮 20 亿美元的估值在一年多内增长约五倍。该人士称 FieldAI 已签署投资条款清单，但交易可能尚未正式完成，领投方未知。

rss · IT HOME · Oct 5, 00:15

**「背景」** FieldAI 成立于 2023 年，正在研发一套可跨人形机器人、机器狗、无人机和工业移动作业车等不同机型运行的“通用型大脑”软件；其上一轮融资超过 4 亿美元，投资方包括贝索斯家族办公室、Emerson Collective 和 Khosla Ventures。

**「影响」** 若交易完成，FieldAI 的估值将接近同行 Physical Intelligence（约 110 亿美元）和 Skild AI（超过 140 亿美元），显示资本正持续流入可在现实世界执行动作的“物理人工智能”领域。

**Tags**: `#robotics`, `#venture capital`, `#physical AI`, `#startup financing`, `#valuation`

---

<a id="item-finance-news-2"></a>
### [US Arrests CEO Accused of Smuggling Over $300 Million in Nvidia AI Chips to China](https://www.ithome.com/1/009/741.htm) ⭐️ 7.0/10

US authorities arrested Greg Lui, 38, CEO of Earthmade Computer, on charges of conspiring to violate export-control laws, smuggling, and money laundering for allegedly using false documents to ship more than $300 million worth of export-controlled Nvidia AI chips and servers to China, according to a Justice Department press release. The indictment, filed by a federal grand jury on September 29 in the US District Court for the Central District of California, alleges the scheme ran from October 2023 to August 2026.

rss · IT HOME · Oct 4, 23:40

**「Background」** The US restricts exports of advanced AI chips such as Nvidia&\#x27;s A100 and H100 to China, citing national-security concerns that China could use them to accelerate AI or military development; the indictment alleges Lui routed servers through Malaysia, Singapore, and Hong Kong using falsified documents and a purchased identity to conceal the true destination.

**「Impact」** The case signals heightened US enforcement against alleged diversion of export-controlled AI chips, a risk for chipmakers, server vendors, and freight forwarders whose products are subject to US export rules.

**Tags**: `#Nvidia`, `#export controls`, `#AI chips`, `#US-China tech`, `#smuggling`

---

<a id="item-finance-news-3"></a>
### [台积电据报拟2027年一季度再上调先进晶圆价格6%~8%](https://www.ithome.com/1/009/740.htm) ⭐️ 7.0/10

据韩媒ddaily 10月2日报道，台积电计划在2027年第一季度将最先进晶圆出货价格再上调约6%~8%，理由为制造成本和电力费用上涨；此前该公司已决定上调10%~20%。报道还称，台积电2纳米制程订单激增，已将晶圆订单目标较原计划提高15%至20%。

rss · IT HOME · Oct 4, 23:29

**「背景」** 台积电将新竹宝山和高雄等地的5座2纳米专用量产工厂转入全面运转，先进制程产能集中使部分客户难以获得新增晶圆配额，高通、AMD等芯片设计企业因此面临成本上升和单一供应链风险，部分客户开始寻求台积电以外的供应来源。

**「影响」** 三星电子代工业务获得潜在订单机会，其正在推进第2代2纳米制程SF2P，目标将良率提升至70%以上；若良率稳定性获得验证，三星有望承接因台积电涨价和产能紧张而转移的先进制程订单。

**Tags**: `#TSMC`, `#semiconductor`, `#pricing`, `#foundry`, `#Samsung`

---

<a id="item-finance-news-4"></a>
### [China Trade-In Subsidies Drive 196.3 Billion Yuan in Holiday Sales](https://www.ithome.com/1/009/725.htm) ⭐️ 7.0/10

China&\#x27;s Ministry of Commerce reported that consumer trade-in subsidies generated 196.3 billion yuan in sales during the first three days of the National Day holiday \(October 1-3\), including 46,000 vehicle trade-ins and 1.709 million digital and smart device purchases. The government also said the full 250 billion yuan in annual trade-in funding has now been allocated to local governments.

rss · IT HOME · Oct 4, 12:46

**「Background」** The trade-in program subsidizes consumers who replace old cars, appliances, and electronics with new ones; from January to August, related sales reached 1.55 trillion yuan and subsidies reached 208 million people, according to the Ministry of Commerce.

**「Impact」** The program has supported demand for automakers, appliance makers, and consumer electronics sellers in China, with new-energy passenger vehicles accounting for more than 60% of new passenger car retail sales for five consecutive months, the ministry said.

**Tags**: `#China consumption`, `#trade-in subsidy`, `#auto sales`, `#consumer electronics`, `#fiscal policy`

---

<a id="item-finance-news-5"></a>
### [South Korea&\#x27;s President Orders Probe After Data Breaches at Major Banks](https://www.ithome.com/1/009/674.htm) ⭐️ 7.0/10

South Korean President Lee Jae-myung ordered a thorough investigation and countermeasures after customer data breaches were reported at Shinhan, KB Kookmin, Hana, and BNK Busan banks, according to the presidential office. Shinhan said 25,729 customers may have been affected by a three-day attack on its loan-agency inquiry system starting Sept. 28, while KB Kookmin reported 119 customers and Hana 89.

rss · IT HOME · Oct 4, 08:48

**「Background」** The breaches hit employee or external-partner systems rather than core banking platforms, and financial regulators called an emergency meeting with bank CEOs and industry association heads to review IT security across the sector.

**「Impact」** South Korea&\#x27;s financial regulator plans to expand IT inspections to employee business systems and external partners, requiring checks for exposed system vulnerabilities and stronger authentication and access controls, which could raise compliance costs for banks and their vendors.

**Tags**: `#cybersecurity`, `#banking`, `#data breach`, `#South Korea`, `#financial regulation`

---

<a id="item-finance-news-6"></a>
### [White House Creates AI Task Force to Report on Risks Within 120 Days](https://www.wsj.com/tech/ai/new-ai-task-force-to-report-on-risks-of-technology-after-public-and-industry-concerns-b6308bef) ⭐️ 7.0/10

The White House has created an AI task force called the &quot;Super Intelligence Force,&quot; led by Director of National Intelligence Jay Clayton, to assess AI risks and report within 120 days, according to The Wall Street Journal. A senior White House official said this makes Clayton effectively the Trump administration&\#x27;s &quot;AI czar,&quot; and Clayton said the president wants the group to keep the U.S. leading in superintelligence while prioritizing Americans&\#x27; interests.

telegram · zaihuapd · Oct 4, 02:37

**「Background」** The task force follows a White House meeting between President Donald Trump and top AI company executives, and Trump has rebranded AI as &quot;super intelligence.&quot; The administration has favored voluntary safety frameworks over new regulation while prioritizing keeping ahead of China.

**「Impact」** The task force&\#x27;s voluntary-framework approach means AI companies would face external safety audits and internal controls rather than binding federal rules, based on the administration&\#x27;s stated preference. The 120-day report could shape whether Congress or agencies pursue legislation later, but the source does not specify any enforcement mechanism.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/trump-jay-clayton-artificial-intelligence-task-force-b8689ea07de9102a52bd1cd2049b5901">Trump names national intelligence director Jay Clayton to ...</a></li>
<li><a href="https://www.techbuzz.ai/articles/house-speaker-johnson-pushes-voluntary-ai-guardrails-over-regulation">House Speaker Johnson Pushes Voluntary AI ... | The Tech Buzz</a></li>
<li><a href="https://www.calcalistech.com/ctechnews/article/rjwzyq95me">Trump and tech executives agree to voluntary AI safety standards</a></li>
<li><a href="https://www.youtube.com/watch?v=vgHMXsmfMfk">The AI constitution? Inside Trump ’s four-step accord on... - YouTube</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#US government`, `#technology regulation`, `#national security`

---

<a id="item-finance-news-7"></a>
### [CCTV Exposes Fake &\#x27;Open Kitchen&\#x27; Livestreams at Food-Delivery Merchants; Hubei and Yunnan Launch Probes](https://www.ithome.com/1/009/692.htm) ⭐️ 6.0/10

After CCTV reported that food-delivery merchants were faking &\#x27;open kitchen&\#x27; livestreams by pointing cameras away from key kitchen areas, market regulators in Wuhan and Lijiang launched investigations and suspended the merchants involved. China&\#x27;s State Administration for Market Regulation said it will push to revise the Food Safety Law to clarify platform and merchant responsibilities, and will tighten platform oversight.

rss · IT HOME · Oct 4, 10:06

**「Background」** China promotes &\#x27;open kitchen&\#x27; livestreams as a way for restaurants to show customers their food preparation, but CCTV found that in 15 delivery merchants in Changsha, Wuhan and Lijiang, 14 had cameras that did not cover key areas such as cutting, cooking and washing, and 6 listed as dine-in were actually delivery-only.

**「Impact」** The suspensions and investigations directly affect the named delivery merchants in Wuhan and Lijiang, while the proposed Food Safety Law revision and tighter platform vetting could raise compliance costs for delivery platforms and restaurants nationwide if enacted.

**Tags**: `#food safety regulation`, `#food delivery platforms`, `#China market regulation`, `#consumer protection`, `#restaurant industry`

---