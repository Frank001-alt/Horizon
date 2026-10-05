---
layout: default
title: "Horizon Summary: 2026-10-05 (ZH)"
date: 2026-10-05
lang: zh
---

> 从 154 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [华为麒麟 9050 Pro 裸片首曝：双裸片垂直堆叠](#item-tech-news-1) ⭐️ 8.0/10
2. [泛林集团提出 SA-CFET 架构，SRAM 单元面积较 N3 缩小 52.7%](#item-tech-news-2) ⭐️ 8.0/10
3. [微软将 Rust 提升为内部一级编程语言](#item-tech-news-3) ⭐️ 8.0/10

**财经新闻**
1. [FieldAI 拟融资 7 亿美元，投后估值达 100 亿美元](#item-finance-news-1) ⭐️ 7.0/10
2. [英伟达 AI 芯片走私案嫌疑人被捕，涉案金额超 3 亿美元](#item-finance-news-2) ⭐️ 7.0/10
3. [台积电先进晶圆据报 2027 年一季度再涨价 6%~8%](#item-finance-news-3) ⭐️ 7.0/10
4. [国庆前三天以旧换新带动销售额 196.3 亿元](#item-finance-news-4) ⭐️ 7.0/10
5. [韩国多家银行遭黑客攻击泄露客户信息，总统李在明下令彻查](#item-finance-news-5) ⭐️ 7.0/10
6. [白宫成立 AI 特别工作组，120 天内提交风险报告](#item-finance-news-6) ⭐️ 7.0/10
7. [央视曝光外卖“明厨亮灶”造假，湖北、云南等地立案核查](#item-finance-news-7) ⭐️ 6.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [华为麒麟 9050 Pro 裸片首曝：双裸片垂直堆叠](https://www.ithome.com/1/009/739.htm) ⭐️ 8.0/10

半导体分析机构 Kurnal Insights 于 9 月 30 日发布华为麒麟 9050 Pro 的裸片显微照，首次从物理层面展示其内部结构：该芯片由两颗尺寸完全相同的裸片垂直堆叠而成，整体尺寸 11.13 × 10.84 mm，每颗裸片面积约 120.65mm²，略小于前代麒麟 9030S 的 122mm²。两颗裸片分工明确，一颗负责核心计算逻辑，另一颗专用于 SRAM 和缓存，通过高密度垂直互连技术连接，这是华为韬定律“逻辑折叠”（LogicFolding）技术的首次商业化落地。据何庭波在 ChinaXiv 发表的署名论文，麒麟 9050 Pro 的等效晶体管密度从麒麟 9030 Pro 的每平方毫米约 1.55 亿个提升至约 2.38 亿个，增幅约 55%，相当于此前三年依靠几何尺寸缩小所取得的成果总和；在性能对齐条件下，NPU 功耗降低 66%、GPU 功耗降低 58%、CPU 性能核功耗降低 41%。@Taog\_1575 依据极客湾资料及 Die Shot 解析称，逻辑裸片采用中芯国际 N+3 工艺，SRAM 裸片采用 N+2 工艺，单颗裸片良率应高于麒麟 9030 Pro，但该芯片仅用于 Mate 90 Pro Max 及以上版本，整体封装良率可能仍然偏低。

rss · IT HOME · 10月4日 23:26

**「背景」** 华为半导体业务负责人何庭波在中国科学院科技论文预发布平台 ChinaXiv 上发表了“韬定律”（《面向多层级电子系统的时间缩微理论》）论文，其 V2 版本新增了 LogicFolding（逻辑折叠）架构与实测数据，交银国际证券研报将其视为韬定律的核心工程实践。该理论主张以“时间（τ）缩微”替代传统的“几何缩微”，即通过垂直堆叠与缩短互连来压缩信号传播时延，而非单纯依赖制程微缩。此次引发讨论的裸片显微照由半导体分析机构 Kurnal Insights 于 2026 年 9 月 30 日发布，其数据库显示该芯片代号 Kirin 9050，尺寸 11.13 × 10.84 mm、面积 120.65 mm²，代工方为中芯国际。

**「影响」** 伯恩斯坦指出，麒麟 9050 Pro 将华为移动芯片与苹果的技术差距缩小至约三年，上一代约为四年，并称其 Geekbench 6 多核成绩超过苹果 3nm 的 A17 Pro。不过该芯片仅用于 Mate 90 Pro Max 及以上版本，3D 堆叠的整体封装良率与散热仍是量产中需持续解决的工程挑战。

<details><summary>参考链接</summary>
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

**标签**: `#semiconductor`, `#chip-design`, `#huawei-kirin`, `#advanced-packaging`, `#hardware`

---

<a id="item-tech-news-2"></a>
### [泛林集团提出 SA-CFET 架构，SRAM 单元面积较 N3 缩小 52.7%](https://www.ithome.com/1/009/737.htm) ⭐️ 8.0/10

泛林集团（Lam Research）于 9 月 29 日提出自对准互补场效应晶体管（SA-CFET）架构，目标将 CMOS 晶体管推进至 10 Å（1nm）及以下节点。该架构包含 SA-BPR（自对准埋入式电源轨）、SA-CT（自对准触点）和 SA-TSV（自对准硅通孔）三个自对准工艺模块，采用非金属栅极切割设计和中间介质隔离（MDI）实现功函数分离，并保持与 N3 规范（42nm 接触栅极间距、21nm 金属间距）的兼容性。其 Semiverse Solutions 团队利用 SEMulator3D 数字孪生工艺建模验证，结果显示 6T SRAM 位单元面积达 0.0094 μm²，相比 N3 缩小 52.7%，相比 A7 CFET 设计缩小 19%，并可构建 NOT、NAND、NOR 等逻辑单元。模型还显示所有关键触点层具有至少 10nm 的套刻窗口，且仿真中未出现开路或短路故障。不过，上述结果均来自数字孪生建模与设计验证，并不意味着 SA-CFET 已进入量产阶段。

rss · IT HOME · 10月4日 22:55

**「背景」** 随着先进制程向 1nm 及以下推进，传统 GAA 纳米片晶体管在漏电、迁移率、寄生电阻和制造波动等方面面临挑战。CFET（互补型场效应晶体管）通过垂直堆叠 NMOS 和 PMOS，可在相同平面面积内提高器件密度并改善静电控制，但存在金属栅极隔离复杂、接触区域拥挤等集成难题。比利时微电子研究中心（imec）在 7 月路线图中预测 2038 年有望实现 0.3 纳米（A3）工艺，并在 9 月更新中指出从 A7 逻辑节点开始行业可能转向基于 CFET 的架构。

**「影响」** 若 SA-CFET 的自对准工艺路径在后续硬件验证中成立，其与 N3 设计规则的兼容性及更大的套刻窗口可能降低 CFET 集成的制造难度，为 10 Å 及以下节点的 SRAM 面积缩放提供一种潜在方案。但当前结论仅基于数字孪生仿真，距离量产验证仍需硬件数据支撑。

**标签**: `#semiconductor manufacturing`, `#transistor architecture`, `#advanced nodes`, `#SRAM scaling`, `#process modeling`

---

<a id="item-tech-news-3"></a>
### [微软将 Rust 提升为内部一级编程语言](https://www.ithome.com/1/009/672.htm) ⭐️ 8.0/10

据 Rust 基金会消息，Rust 现已成为微软公司内部的“一级编程语言（Tier-1）”，与 C++、C\# 和 TypeScript 并列。这里的 Tier-1 是微软内部使用的分类，并非 Rust 项目自身的支持等级；对微软内部开发团队而言，这意味着无需再自行搭建 Rust 开发和生产环境，微软将提供从代码编写、构建、测试到发布和长期维护的一整套标准流程，并将 Rust 项目纳入现有的软件安全、合规等开发流程。微软表示 Rust 已被应用于固件、驱动程序、内核、虚拟机监控程序、微服务和应用程序等多种软件，但由于 C++ 已在微软内部使用多年并广泛存在于 Windows 等大型项目中，未来很长一段时间内两者仍将并行使用。为促进协同，微软开发了 rustc\_codegen\_utc 项目，让 Rust 编译器直接连接 Windows 平台 MSVC 工具链使用的代码生成后端，从而与现有工具链及应用程序二进制接口（ABI）协同工作，并继续使用安全功能、调试工具、崩溃转储分析、性能分析、诊断、代码覆盖率、热补丁和编译优化能力。微软强调该项目并非实验性项目，从 2026 年初开始已具备生产环境使用条件，从 Rust 1.90 版本开始已能完成自身编译，目前已有超过 100 个微软项目代码库使用这一后端。

rss · IT HOME · 10月4日 08:43

**「背景」** Rust 是由 Mozilla 发起、现由 Rust 基金会维护的系统级编程语言，以内存安全著称。微软多年来在 Windows 等大型项目中主要依赖 C++，同时内部也使用 C\# 和 TypeScript。此前微软工程师虽已用 Rust 开发固件、驱动、内核等组件，但多由各团队自行适配环境，缺乏统一支持。

**「影响」** 微软内部团队今后可直接使用受支持的 Rust 标准开发流程，无需自行搭建环境；同时包含 Rust 和 C++ 的大型项目可共享同一套底层工具链与基础设施，减少重复维护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://www.sohu.com/a/1083976260_122066679">Rust正式成为微软Tier-1编程语言，与C++并列_项目_生产_支持</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#编程语言`, `#编译器工具链`, `#Windows`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [FieldAI 拟融资 7 亿美元，投后估值达 100 亿美元](https://www.ithome.com/1/009/746.htm) ⭐️ 7.0/10

据《商业内幕》报道，知情人士称机器人软件公司 FieldAI 正融资 7 亿美元，投后估值 100 亿美元，约为其上一轮 20 亿美元估值的五倍；该公司已签署投资条款清单，但交易可能尚未正式完成。

rss · IT HOME · 10月5日 00:15

**「背景」** FieldAI 成立于 2023 年，研发可跨人形机器人、机器狗、无人机和工业移动作业车运行的“通用大脑”软件；其上一轮融资超过 4 亿美元，投资方包括贝索斯家族办公室、Emerson Collective 和 Khosla Ventures。

**「影响」** 若交易完成，FieldAI 的估值将接近同行 Physical Intelligence（约 110 亿美元）和 Skild AI（超过 140 亿美元），反映资本持续流入可在现实世界执行动作的“物理人工智能”领域。

**标签**: `#robotics`, `#venture capital`, `#physical AI`, `#startup financing`, `#valuation`

---

<a id="item-finance-news-2"></a>
### [英伟达 AI 芯片走私案嫌疑人被捕，涉案金额超 3 亿美元](https://www.ithome.com/1/009/741.htm) ⭐️ 7.0/10

美国司法部指控大地智造计算机公司（Earthmade Computer）首席执行官格雷格·刘（Greg Lui）使用虚假文件，将货值超过 3 亿美元、含受出口管制的英伟达 AI 芯片的服务器走私至中国，他已被捕并面临合谋违反出口管制、走私和洗钱三项指控。

rss · IT HOME · 10月4日 23:40

**「背景」** 美国以国家安全为由限制英伟达 A100、H100 等可用于训练大语言模型的芯片对华出口，司法部称该走私活动从 2023 年 10 月持续至 2026 年 8 月，联邦大陪审团于 9 月 29 日正式提交起诉书。

**「影响」** 此案显示美国出口管制执法正延伸至通过马来西亚、新加坡等第三地转运的渠道，可能加大相关货运代理和服务器转售企业的合规压力。

**标签**: `#Nvidia`, `#export controls`, `#AI chips`, `#US-China tech`, `#smuggling`

---

<a id="item-finance-news-3"></a>
### [台积电先进晶圆据报 2027 年一季度再涨价 6%~8%](https://www.ithome.com/1/009/740.htm) ⭐️ 7.0/10

据韩媒 ddaily 报道，台积电计划在 2027 年第一季度将最先进晶圆出货价格再次上调约 6%~8%，理由为制造成本和电力费用上涨；此前已有一次 10%~20%的涨价决定。

rss · IT HOME · 10月4日 23:29

**「背景」** 报道称台积电 2 纳米制程订单激增，已将晶圆订单目标较原计划提高 15%至 20%，新竹宝山和高雄等地 5 座 2 纳米专用量产工厂转入全面运转，先进制程产能集中使部分客户难以获得新增晶圆配额。

**「影响」** 报道称高通、AMD 等芯片设计企业面临制造成本上升与单一供应链风险，部分客户开始寻求台积电以外的供应来源，三星代工业务因此获得潜在订单机会；三星正推进第 2 代 2 纳米制程 SF2P，目标将良率提升至 70%以上。

**标签**: `#TSMC`, `#semiconductor`, `#pricing`, `#foundry`, `#Samsung`

---

<a id="item-finance-news-4"></a>
### [国庆前三天以旧换新带动销售额 196.3 亿元](https://www.ithome.com/1/009/725.htm) ⭐️ 7.0/10

据新华社报道，商务部数据显示，国庆假期前三天（10 月 1 日至 3 日），消费品以旧换新带动销售额 196.3 亿元，惠及 348.3 万人次，其中汽车以旧换新 4.6 万辆、数码和智能产品购新 170.9 万件。国家发展改革委会同财政部已下达今年第四批 625 亿元超长期特别国债资金，全年 2500 亿元以旧换新资金全部下达完毕。

rss · IT HOME · 10月4日 12:46

**「背景」** 以旧换新是国家用财政补贴鼓励消费者淘汰旧车、旧家电和旧数码产品并购买新品的政策；今年 1 至 8 月，相关商品销售额已达 1.55 万亿元，补贴惠及 2.08 亿人次。

**「影响」** 全年补贴资金已全部到位，意味着后续政策支持规模不再增加，汽车、家电和数码产品零售商及消费者可获得的补贴将取决于各地已下达资金的使用进度。

**标签**: `#China consumption`, `#trade-in subsidy`, `#auto sales`, `#consumer electronics`, `#fiscal policy`

---

<a id="item-finance-news-5"></a>
### [韩国多家银行遭黑客攻击泄露客户信息，总统李在明下令彻查](https://www.ithome.com/1/009/674.htm) ⭐️ 7.0/10

韩国总统李在明 10 月 4 日就新韩银行、KB 国民银行、韩亚银行、BNK 釜山银行等金融机构遭黑客攻击、客户个人信息泄露一事，要求有关部门彻底调查并制定对策。据韩联社报道，新韩银行有 25729 名客户信息可能泄露，国民银行和韩亚银行分别涉及 119 名和 89 名客户。

rss · IT HOME · 10月4日 08:48

**「背景」** 新韩银行用于贷款代理机构查询业务的系统自 9 月 28 日起连续 3 天遭攻击，国民银行、韩亚银行的员工业务支持系统也发生信息泄露，BNK 釜山银行则有 11 名外包开发人员信息外泄；金融委员会委员长和金融监督院院长当天下午召集金融机构协会会长及涉事公司首席执行官召开紧急会议。

**「影响」** 韩国金融监管机构表示将把 IT 系统检查范围扩大到员工业务系统和外部合作方，并要求排查外部暴露系统漏洞、强化身份验证和访问控制，同时分享攻击 IP 及手法。

**标签**: `#cybersecurity`, `#banking`, `#data breach`, `#South Korea`, `#financial regulation`

---

<a id="item-finance-news-6"></a>
### [白宫成立 AI 特别工作组，120 天内提交风险报告](https://www.wsj.com/tech/ai/new-ai-task-force-to-report-on-risks-of-technology-after-public-and-industry-concerns-b6308bef) ⭐️ 7.0/10

据《华尔街日报》报道，白宫新设名为“超级智能力量”（Super Intelligence Force）的人工智能特别工作组，由国家情报总监 Jay Clayton 领导，负责评估 AI 风险及联邦政府应承担的责任，并须在 120 天内提交报告。一名白宫高级官员称，这让 Clayton 实际上成为特朗普政府的“AI 沙皇”。

telegram · zaihuapd · 10月4日 02:37

**「背景」** 特朗普政府此前已拒绝出台新的 AI 监管，优先保持对华领先，并支持包含外部安全审计和更强内部管控的自愿框架。

**「影响」** 该工作组采用自愿框架而非新监管，意味着美国 AI 企业短期内不会面临新的强制性合规要求，但参与外部安全审计和内部管控可能成为行业惯例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techbuzz.ai/articles/house-speaker-johnson-pushes-voluntary-ai-guardrails-over-regulation">House Speaker Johnson Pushes Voluntary AI ... | The Tech Buzz</a></li>
<li><a href="https://www.calcalistech.com/ctechnews/article/rjwzyq95me">Trump and tech executives agree to voluntary AI safety standards</a></li>
<li><a href="https://www.youtube.com/watch?v=vgHMXsmfMfk">The AI constitution? Inside Trump ’s four-step accord on... - YouTube</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#US government`, `#technology regulation`, `#national security`

---

<a id="item-finance-news-7"></a>
### [央视曝光外卖“明厨亮灶”造假，湖北、云南等地立案核查](https://www.ithome.com/1/009/692.htm) ⭐️ 6.0/10

央视《每周质量报告》调查发现，长沙、武汉、丽江 15 家标注“明厨亮灶”的外卖商户中，14 家监控未覆盖切配、烹饪、洗消等关键区域，6 家标称堂食店实际为纯外卖。市场监管总局已部署湖南、湖北、云南等地核查处置，武汉对曝光商户立案调查并督促下架、暂停网络经营，丽江对 4 家涉事商户停业整顿并立案调查。

rss · IT HOME · 10月4日 10:06

**「背景」** “明厨亮灶”是市场监管总局推广的餐饮透明化措施，要求餐饮服务提供者通过透明或视频方式向公众展示后厨操作过程，以保障消费者知情权并接受社会监督。

**「影响」** 此次整治直接波及被曝光的外卖商户及所在平台，涉事商家面临下架、停业和立案调查；市场监管总局表示将推动修订《食品安全法》，进一步明确外卖平台和入网餐饮服务提供者的食品安全主体责任，并压实平台审核把关责任，对公示信息不真实的商家一律下线。

**标签**: `#food safety regulation`, `#food delivery platforms`, `#China market regulation`, `#consumer protection`, `#restaurant industry`

---