---
layout: default
title: "Horizon Summary: 2026-10-13 (EN)"
date: 2026-10-13
lang: en
---

> From 193 items, 10 important content pieces were selected

---

**Technology News**
1. [Hackers Trigger Defrost Cycles in European Supermarket Fridges](#item-tech-news-1) ⭐️ 8.0/10
2. [WiFi 7 Router Repurposed as 320 Msps SDR Receiver](#item-tech-news-2) ⭐️ 8.0/10
3. [Aged Blood Cells Reprogrammed to Stem Cells With Younger Molecular Age](#item-tech-news-3) ⭐️ 8.0/10
4. [Python 3.15 Released with Lazy Imports and Sampling Profiler](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Flask Session Pickle RCE Bug Nets $90,000](#item-tech-news-5) ⭐️ 8.0/10
6. [华为公布麒麟 9050 Pro 架构并确认量产](#item-tech-news-6) ⭐️ 8.0/10
7. [微软发布 Maia 300 自研 AI 芯片，明年拟部署超百万颗](#item-tech-news-7) ⭐️ 8.0/10
8. [NVIDIA Opens Vera Rubin Rack Design via OCP](#item-tech-news-8) ⭐️ 8.0/10
9. [SK Hynix Unveils H-TPU SSD Processor Architecture](#item-tech-news-9) ⭐️ 8.0/10
10. [NVIDIA and Cisco Unveil USFP 400G/lane Optical Module Spec](#item-tech-news-10) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Hackers Trigger Defrost Cycles in European Supermarket Fridges](https://www.tomshardware.com/tech-industry/cyber-security/unprecedented-cyberattack-cripples-supermarket-fridges-across-europe-as-hackers-activate-automatic-defrosting-delivery-and-store-prices-also-impacted-by-incident) ⭐️ 8.0/10

Hackers exploited internet-connected refrigeration controllers to remotely activate automatic defrosting, disrupting supermarket operations across Europe, with French chain Intermarché reporting that 150 stores were targeted. Reporting from Reuters, the BBC, and Le Monde ties the incident to insecure OT/IoT refrigeration equipment, and related research from Claroty&\#x27;s Team82 documents vulnerabilities in Danfoss refrigeration controllers. Community discussion points to legacy hardware such as the Danfoss SM800 \(end of support 2021\) and SC355 \(end of support 2016\) as likely suspects, alongside the broader problem of internet-exposed controllers. Delivery and in-store prices were also reportedly affected by the incident.

hackernews · Zeekaas · Oct 12, 12:16 · [Discussion](https://news.ycombinator.com/item?id=50055304)

**「Background」** Danfoss refrigeration controllers are widely used in commercial supermarket refrigeration systems, and some models such as the AK-SM 800A series have been the subject of security research. In August 2026, Claroty&\#x27;s Team82 published research identifying multiple vulnerabilities in the Danfoss AK-SM 800A refrigeration controller platform, and Danfoss issued a security advisory \(DSA-2025-08-01\) recommending patch 4.3.1 for affected AK-SM 8xxA series devices. The incident described here follows that disclosure and involves attackers exploiting internet-connected refrigeration controllers to trigger automatic defrosting.

**「Impact」** The incident affected supermarket refrigeration operations across Europe, with Intermarché reporting that 150 stores were targeted and that personal data of nearly 300,000 customers was compromised. The attack underscores that internet-connected legacy refrigeration controllers, such as end-of-support Danfoss models, remain exposed in production retail environments.

**「Community Discussion」** Commenters debated why refrigeration controllers are internet-connected at all, with one citing Danfoss marketing that remote diagnostics and estate-wide efficiency comparisons justify connectivity, and another noting that newer hospital lab machines require paid subscriptions and internet access to function. One commenter argued that shift-work labor and low-margin operations lack the budget for security reviews or hardware refresh cycles, while another asked whether the attack is linked to a similar August 2026 incident at US military bases or is an unrelated or copycat event.

<details><summary>References</summary>
<ul>
<li>Uncovering Vulnerabilities in Danfoss Refrigeration Controllers | Claroty</li>
<li>DSA-2025-08-01 - Danfoss</li>
<li><a href="https://www.connexionfrance.com/news/intermarche-cyberattack-affects-nearly-300000-customers/806317">Intermarché cyberattack 2026 : Nearly 300,000 customers&#x27; data stolen...</a></li>
<li><a href="https://torwire.com/news/cybersecurity/intermarche-drive-service-data-breach/">Cyberattack on Intermarché Drive Service Exposes Data of... - TorWire</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#IoT/OT security`, `#embedded systems`, `#critical infrastructure`, `#vulnerability disclosure`

---

<a id="item-tech-news-2"></a>
### [WiFi 7 Router Repurposed as 320 Msps SDR Receiver](https://github.com/h0m3us3r/w1700k-sdr) ⭐️ 8.0/10

A developer has published a project, w1700k-sdr, that turns a WiFi 7 router into a 320 Msps software-defined radio receiver. The work is notable for achieving a 320 Msps receive rate at 5 GHz using low-cost consumer hardware rather than dedicated SDR equipment. Community commenters note that the same developer previously built an SDR from an ESP32 Wi-Fi microcontroller \(eSpDR\), and that the same chipset is likely present in the Banana Pi R4, which includes built-in PCIe for NVMe. Commenters also observe that this may be among the cheapest ways to obtain a 320 Msps receiver at 5 GHz, though it is not a DC-to-daylight solution. The project is presented as an open-source hardware-hacking effort with potential for broader reuse on common Wi-Fi cards.

hackernews · djfergus · Oct 12, 12:41 · [Discussion](https://news.ycombinator.com/item?id=50055593)

**「Background」** Software-defined radio \(SDR\) replaces dedicated analog radio hardware with software processing of digitized signals, traditionally requiring specialized receivers such as the RTL-SDR \(RTL2832U\) dongle. Common low-cost SDRs sample at only a few megasamples per second, so a 320 Msps receiver at 5 GHz represents a much higher-performance, lower-cost alternative. The project builds on the same developer&\#x27;s earlier work turning an ESP32 Wi-Fi microcontroller into an SDR.

**「Impact」** Owners of the Banana Pi BPI-R4, which uses the same MediaTek MT7988A \(Filogic 880\) chipset, can likely run this 320 Msps SDR receiver, according to community reports.

**「Community Discussion」** Commenters reacted enthusiastically, highlighting the low cost of a 320 Msps receiver at 5 GHz and the possibility of running the same approach on the Banana Pi R4 due to its shared chipset and built-in PCIe for NVMe. One commenter pointed to the developer&\#x27;s earlier ESP32-based eSpDR project and hoped similar work would spread to common Wi-Fi cards so ordinary laptops could serve as budget SDRs. Another raised the question of whether software-defined radios explain why Samsung requires third parties to sign a contract before using phone FM radios, while a commenter with service-monitor repair experience described how cheap CNC, PCBs, and high-frequency components could enable building advanced test equipment around such an SDR.

<details><summary>References</summary>
<ul>
<li><a href="https://radiohooligan.ru/hdsdr-dlya-rtl-sdr/">HDSDR — установка и настройка программы для приемника...</a></li>
<li><a href="https://www.rtl-sdr.com/foxsdr-updates-node-canvas-single-map-display-linuxandroid-builds-locating-air-traffic-radar-positions/comment-page-100/">FoxSDR Updates: Node Canvas, Single Map Display, Linux+Android...</a></li>
<li><a href="https://wiki.banana-pi.org/Banana_Pi_BPI-R4">Banana Pi BPI- R 4 - Banana Pi Wiki</a></li>

</ul>
</details>

**Tags**: `#SDR`, `#WiFi 7`, `#hardware hacking`, `#open source`, `#wireless`

---

<a id="item-tech-news-3"></a>
### [Aged Blood Cells Reprogrammed to Stem Cells With Younger Molecular Age](https://doi.org/10.1111/acel.70751) ⭐️ 8.0/10

A study published in Aging Cell reports that blood cells from an 80-year-old donor were reprogrammed into stem cells whose molecular age measured under 20. The work sits at the intersection of cellular reprogramming and aging research, where induced pluripotent stem cells are used to reset epigenetic markers associated with age. The reported result is notable because the starting cells came from a very old donor, suggesting the reprogramming process can substantially reverse molecular aging signatures in human cells. The finding is early-stage and does not establish that whole-organism aging can be reversed or that such cells are safe for therapeutic use. The linked peer-reviewed article is available via PubMed Central.

hackernews · arunc · Oct 12, 23:34 · [Discussion](https://news.ycombinator.com/item?id=50064536)

**「Background」** Cellular reprogramming is the process of converting one cell type into another, often by resetting epigenetic marks that accumulate with age. Epigenetic clocks estimate biological age from DNA methylation patterns, and partial reprogramming aims to reverse those marks without losing cell identity. The study in question used blood cell progenitors from an 80-year-old donor and directly reprogrammed them into neural stem cells, tracking the reset over more than 100 days.

**「Impact」** The result is early-stage and in vitro, so it does not yet demonstrate rejuvenation at the organismal level; its practical significance for regenerative medicine remains unproven.

**「Community Discussion」** Commenters reacted with a mix of personal motivation and skepticism: one said news like this prompted healthier habits in hopes of living long enough to benefit from future aging treatments, while another compared the process to the immortal jellyfish resetting damage by returning to a single cell. Others raised concerns about the abstract&\#x27;s dense language and speculated darkly about potential misuses, such as dictators seeking rejuvenation or cell reprogramming being applied to AI workloads before aging remediation.

<details><summary>References</summary>
<ul>
<li><a href="https://medicalxpress.com/news/2026-10-blood-cells-year-donor-stem.html">Blood cells from 80-year-old donor become stem cells with ...</a></li>
<li><a href="https://nautil.us/blood-cells-from-an-80-year-old-transformed-into-young-brain-cells-1285722">Blood Cells From an 80-Year-Old Transformed into Young Brain ...</a></li>
<li><a href="https://bioengineer.org/blood-cells-from-80-year-olds-rejuvenated-into-brain-cells-with-molecular-age-under-20/">Blood Cells From 80-Year-Olds Rejuvenated Into Brain Cells ...</a></li>
<li><a href="https://www.cell.com/trends/molecular-medicine/fulltext/S1471-4914%2826%2900011-0">Cellular reprogramming beyond pluripotency: Trends in ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1568163725000832">Conserved biological processes in partial cellular ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1471491426000110">Cellular reprogramming beyond pluripotency - ScienceDirect</a></li>

</ul>
</details>

**Tags**: `#stem cells`, `#aging research`, `#cellular reprogramming`, `#biotechnology`, `#longevity`

---

<a id="item-tech-news-4"></a>
### [Python 3.15 Released with Lazy Imports and Sampling Profiler](https://simonwillison.net/2026/Oct/12/python-3-15/) ⭐️ 8.0/10

Python 3.15 has been released, with the official &quot;What&\#x27;s new in Python 3.15&quot; guide curated by 3.14 and 3.15 release manager Hugo van Kemenade. The headline feature is PEP 810 explicit lazy imports, which let developers write \`lazy import json\` or \`lazy from pathlib import Path\` so the module is imported only when its symbols are first used, directly addressing startup costs such as those caused by plugins with heavy dependencies like \`sentence\_transformers\`. PEP 798 adds unpacking in comprehensions, enabling syntax such as \`\[\*sublist for sublist in lists\]\`, \`\{\*s for s in sets\}\`, and \`\{\*\*d for d in dicts\}\` as an extension of PEP 448 unpacking from Python 3.5. The existing tracing profiler has been renamed from \`cProfile\` to \`profiling.tracing\` and is joined by a new sampling profiler, Tachyon, exposed as \`profiling.sampling\`, which can attach to a running process by PID, produce reports, flame graphs, heat maps, and Firefox-profiler-compatible output. Miguel Grinberg&\#x27;s testing against 3.15.0rc3 found performance mostly unchanged from 3.14, except the experimental JIT, which gave a 1.2x boost over the standard 3.15 interpreter on a Fibonacci test. As a maintainer supporting every supported Python version, Simon Willison notes he can now say goodbye to Python 3.10 and begin adopting features from Python 3.11.

rss · Simon Willison · Oct 12, 18:15

**「Background」** Python is a widely used open-source programming language, and each annual release adds syntax and standard-library features while dropping older versions from support. PEP 448, which landed in Python 3.5 in 2015, generalized unpacking syntax; PEP 798 extends that idea to comprehensions. Profiling in Python has traditionally relied on the tracing profiler \`cProfile\`, while sampling profilers such as py-spy have been external tools.

**「Impact」** Library and plugin maintainers can use PEP 810 lazy imports to avoid multi-second startup penalties from heavy optional dependencies, and developers gain a built-in sampling profiler for low-overhead production-style profiling. The modest 3.15 performance gains mean the experimental JIT remains the main source of meaningful speedups for now.

**Tags**: `#python`, `#programming-languages`, `#open-source`, `#language-releases`, `#pep-810`

---

<a id="item-tech-news-5"></a>
### [Google Flask Session Pickle RCE Bug Nets $90,000](https://simonkoeck.com/writeups/google-devsite-flask-session-pickle-rce) ⭐️ 8.0/10

A security researcher published a writeup describing the discovery of a remote code execution vulnerability in Google infrastructure, reportedly earning a $90,000 bug bounty. According to the analysis summary, the flaw involved Flask session pickle deserialization, a class of issue where untrusted serialized session data is deserialized in a way that can allow arbitrary code execution. The writeup is presented as a technical deep-dive into the vulnerability and its exploitation. The source content provided is only a link stub, so specific technical details, affected components, disclosure timeline, and Google&\#x27;s response are not available in the supplied material.

rss · Lobsters · Oct 12, 14:40

**「Background」** Flask is a Python web framework that can store session data in client-side cookies, and when those sessions are serialized with Python&\#x27;s pickle module, deserializing attacker-controlled data can lead to remote code execution. Pickle is designed for trusted data and is unsafe to unpickle from untrusted sources, a known class of vulnerability demonstrated in public proof-of-concept Flask applications. This writeup describes how that deserialization weakness was found in Google infrastructure and earned a $90,000 bug bounty.

**「Impact」** This finding reinforces that Flask applications using pickle-based session serialization remain exposed to remote code execution when attackers can supply or tamper with serialized session data, as demonstrated by prior issues such as CVE-2021-33026 in Flask-Caching and the Flask-KVSession pickle RCE. For Google, the $90,000 bounty signals that even hardened production infrastructure can contain deserialization flaws with severe consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/CalfCrusher/Python-Pickle-RCE-Exploit">GitHub - CalfCrusher/Python- Pickle - RCE -Exploit: Python Pickle RCE ...</a></li>
<li><a href="https://davidhamann.de/2020/04/05/exploiting-python-pickle/">Exploiting Python pickles | David Hamann</a></li>
<li><a href="https://www.sourcery.ai/vulnerabilities/python-flask-security-insecure-deserialization">Flask Insecure Deserialization Vulnerability | Security ... | Sourcery</a></li>
<li><a href="https://github.com/deepanshhooda/flask-kvsession-pickle-rce">GitHub - deepanshhooda/ flask -kvsession- pickle -rce: PoC...</a></li>
<li><a href="https://vulmon.com/vulnerabilitydetails?qid=CVE-2021-33026">CVE-2021-33026 - Remote Code Execution in Flask -Caching</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#remote-code-execution`, `#web-frameworks`, `#bug-bounty`

---

<a id="item-tech-news-6"></a>
### [华为公布麒麟 9050 Pro 架构并确认量产](https://www.ithome.com/1/012/196.htm) ⭐️ 8.0/10

华为于 10 月 13 日在上海练秋湖举行的 2026 麒麟媒体沟通会上，由半导体业务无线终端芯片产品管理部部长徐松余首次公布麒麟 9050 Pro 芯片的详细架构图（发布会现场为简要版本）。该芯片搭载新一代灵犀 CPU、新一代马良 GPU、新一代达芬奇架构 NPU、新一代麒麟 AI ISP，并包含灵犀微核、FFTS 函数流任务调度器与安全处理器等组件。徐松余同时确认，首款逻辑折叠芯片麒麟 9050 系列在中国半导体产业界的支持下已成功量产。他列举了该路径未来面临的挑战，包括工具链和方法论、工艺差异补偿、跨层互联开销优化、能耗控制以及基准测试方法。徐松余呼吁半导体产业界与学术界加强合作，称未来属于开放合作，没有一家企业可以独自解答所有答案。

rss · IT HOME · Oct 13, 02:34

**「背景」** 麒麟是华为自研的移动终端芯片系列，其架构通常涵盖 CPU、GPU、NPU 与 ISP 等模块。所谓“逻辑折叠”指通过跨层设计或堆叠方式提升集成度与性能的芯片实现路径，其量产往往依赖制造工艺、工具链与测试方法的配套成熟。

**「影响」** 对关注国产半导体的开发者和产业链厂商而言，麒麟 9050 系列量产意味着逻辑折叠路径已进入实际产品阶段，但工具链、工艺补偿与基准测试等未解问题仍可能影响后续迭代节奏。

**Tags**: `#semiconductors`, `#Huawei Kirin`, `#chip architecture`, `#AI hardware`, `#open source collaboration`

---

<a id="item-tech-news-7"></a>
### [微软发布 Maia 300 自研 AI 芯片，明年拟部署超百万颗](https://www.ithome.com/1/012/191.htm) ⭐️ 8.0/10

Microsoft unveiled Maia 300, its third-generation in-house AI chip, and plans to deploy more than one million units next year to support its internal AI workloads. Unlike Nvidia&\#x27;s single large accelerator die paired with high-bandwidth memory, Maia 300 uses a chiplet architecture: compute chiplets are made on TSMC&\#x27;s 2nm process, while chiplets handling data transfer and in-system scheduling use the cheaper 3nm process. A single Maia 300 server rack holds 96 chips and draws about 167 kW, compared with Nvidia&\#x27;s latest GB300 rack with 72 GPUs at 142 kW. Microsoft claims Maia 300 delivers roughly 40% more useful compute per megawatt than &quot;mainstream GPU systems,&quot; without naming the comparison products, and says it will begin multi-gigawatt-scale deployment next year as its capital spending this calendar year is expected to exceed $175 billion. The launch comes as cloud providers and AI companies including OpenAI push their own chips to challenge Nvidia&\#x27;s dominance.

rss · IT HOME · Oct 13, 02:25

**「Background」** Microsoft has been developing its own AI silicon to reduce reliance on Nvidia GPUs and lower the cost of running internal and Azure-hosted AI workloads. The Maia line is Microsoft&\#x27;s custom accelerator family; earlier generations have already been used for Microsoft&\#x27;s own models and for OpenAI models hosted on Azure. Maia 300 is the third generation, and Microsoft is positioning it as part of a broader industry push by cloud providers and AI companies to challenge Nvidia&\#x27;s dominance in AI compute.

**「Impact」** Microsoft&\#x27;s plan to deploy over a million Maia 300 chips next year could reduce its internal AI compute costs and lessen its reliance on Nvidia, while intensifying competition among cloud providers building custom AI silicon. However, the claimed 40% efficiency advantage over &quot;mainstream GPU systems&quot; is a vendor statement without a specified comparison product, and it remains uncertain whether Maia 300 will serve external customers such as Anthropic or remain limited to Microsoft&\#x27;s internal workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/1/012/115.htm">微软 Maia 300 AI 芯片发布：台积电 N2P 工艺，288GB HBM4 内存、带宽...</a></li>
<li><a href="https://technews.tw/2026/10/13/microsoft-maia-300-to-begin-production-deployments-in-2027/">微軟 Maia 300 新晶片明年量產，關鍵運算 Chiplet 採台積電 N2P 製程 ...</a></li>
<li><a href="https://www.spotech.online/zh/news-1f073325dc394b50df945714/">微软发布第三代自研AI芯片Maia 300，预计2027年量产部署</a></li>
<li><a href="https://xueqiu.com/4885703643/404468806">深度解读如下｜ 微 软 Maia 300 寻求 台积电 30 万 枚产能，云厂商自研AI...</a></li>
<li><a href="https://m.163.com/dy/article/L41OURVI0550WHYR.html">摆脱 英 伟 达 依赖！ 微 软 Maia 300 ...</a></li>

</ul>
</details>

**Tags**: `#AI 芯片`, `#微软`, `#数据中心硬件`, `#chiplet`, `#算力成本`

---

<a id="item-tech-news-8"></a>
### [NVIDIA Opens Vera Rubin Rack Design via OCP](https://www.ithome.com/1/012/120.htm) ⭐️ 8.0/10

At the OCP Global Summit, NVIDIA announced it is opening its Vera Rubin rack and compute tray designs through the NVIDIA MGX architecture, contributing them to the Open Compute Project alongside Cisco, Google, Meta, Microsoft, and Visionbay. The updated MGX 1.2 specification adds rack-level blind-mate liquid cooling, interoperable rack interconnects, a liquid-cooled 5000A busbar, and native 19-inch device support, enabling deployments up to 250kW per rack while simplifying assembly, testing, maintenance, and deployment. NVIDIA also released four open-source DSX AI Factory software components covering switch configuration, GPU cluster stress testing, rack firmware management, and bare-metal deployment, derived from DGX Cloud operational experience, which can help cloud providers turn hardware into production clusters within hours. In addition, NVIDIA, AMD, Google, and Meta published Open Data Center Specification v0.7 to unify power, cooling, and physical layout designs for AI factories, while Google, Meta, Microsoft, and NVIDIA issued a grid resilience specification requiring large-scale AI facilities to stay connected during grid disturbances and recover to near full load in under 2 seconds. Meta will adopt NVIDIA Spectrum-6 102.4Tb/s Ethernet switches for an open-network Vera Rubin AI factory, with Spectrum-6 doubling Spectrum-4&\#x27;s switching capacity and per-lane bandwidth and, with Spectrum-X Multiplane, supporting clusters of over 100,000 GPUs. NVIDIA and Cisco also introduced USFP, described as the industry&\#x27;s first pluggable optical module for 400Gb/s network architectures, offering 16 full-duplex lanes in a size close to OSFP, four times the bandwidth density of traditional 200Gb/s single-lane pluggable optics, and about 1.3 times better energy efficiency; NVIDIA and Google further announced that future ConnectX-10 SuperNICs and BlueField DPUs will support Falcon Transport to improve Ethernet AI network reliability and bandwidth utilization.

rss · IT HOME · Oct 13, 02:12

**「Background」** The Open Compute Project \(OCP\) is an industry effort to share datacenter hardware and infrastructure designs so vendors can build interoperable systems. NVIDIA&\#x27;s MGX architecture provides a modular reference design for AI servers and racks, and the Vera Rubin platform is positioned as the basis for next-generation AI factory infrastructure. The DSX AI Factory software components build on operational practices from NVIDIA DGX Cloud.

**「Impact」** System vendors and cloud providers gain standardized rack, cooling, power, and software building blocks intended to speed deployment of next-generation AI datacenters, while the involvement of Cisco, Google, Meta, Microsoft, AMD, and Visionbay signals broad industry alignment around these specifications.

**Tags**: `#AI infrastructure`, `#open standards`, `#datacenter hardware`, `#NVIDIA`, `#liquid cooling`

---

<a id="item-tech-news-9"></a>
### [SK Hynix Unveils H-TPU SSD Processor Architecture](https://www.ithome.com/1/012/160.htm) ⭐️ 8.0/10

SK Hynix announced H-TPU \(Hynix Transaction Processing Unit\) on October 12, a lightweight, programmable processor architecture dedicated to controlling SSD data planes and processing transactions rather than AI tensor computation. SoC design vice president 구인재 presented the architecture at the ISOCC 2026 conference in Songdo, Incheon, South Korea, arguing that general-purpose CPU cores inside SSD controllers have hit limits in frequency and control capability even as GPU performance and PCIe bandwidth double each generation. Instead of relying on a single monolithic CPU, H-TPU splits control functions into dozens of small TPU clusters and uses a simplified four-stage pipeline that excludes superscalar and out-of-order execution. SK Hynix claims H-TPU occupies about 1/25 the area of a general-purpose CPU core \(roughly 4% of total CPU area\) and consumes about 2.5% of its power, with unused function modules switching to a minimum-power mode. The company plans to apply H-TPU across its NAND product lines, starting with next-generation enterprise SSD \(eSSD\) controllers and later its next-generation AI storage architecture, Storage Next, and expects synergy with its next-generation high-bandwidth flash \(HBF\) due next year.

rss · IT HOME · Oct 13, 01:15

**「Background」** As AI workloads grow, data center bottlenecks are shifting from compute to memory and storage layers, putting pressure on SSD controllers. Traditional SSD controllers rely on general-purpose CPU cores to handle hundreds of detailed storage control functions, an approach SK Hynix says causes power waste and unpredictable pipeline latency. H-TPU is not a tensor accelerator for AI math but a transaction-oriented control processor, and no independent benchmarks or shipping products have been announced yet.

**「Impact」** If the claimed area and power figures hold in production, H-TPU could let SK Hynix build more power-efficient enterprise SSD controllers and lay groundwork for its Storage Next AI storage architecture, though the technology remains unproven outside the company&\#x27;s own projections.

**Tags**: `#storage`, `#hardware-architecture`, `#ssd`, `#ai-infrastructure`, `#sk-hynix`

---

<a id="item-tech-news-10"></a>
### [NVIDIA and Cisco Unveil USFP 400G/lane Optical Module Spec](https://www.ithome.com/1/012/155.htm) ⭐️ 8.0/10

NVIDIA and Cisco announced USFP, described as the industry&\#x27;s first pluggable optical module specification supporting 400Gbps per lane. USFP matches OSFP in size, with first-generation products integrating 16 full-duplex lanes that can later scale to 32 or more lanes, enabling up to 12.8 Tb/s throughput. The specification claims four times the bandwidth of existing 200G/lane pluggable optical modules and 1.3x better energy efficiency with 400G SerDes support. It uses a new two-dimensional array connector whose two-step insertion design engages high-speed contacts only after the module is inserted, reducing contact wear, improving signal integrity, and making insertion force more predictable. USFP also supports 100W power, which the companies say simplifies switch design.

rss · IT HOME · Oct 13, 00:55

**「Background」** Pluggable optical modules are the interchangeable transceivers that connect switches and servers in data centers, and their per-lane signaling rate sets how much bandwidth a single port can carry. OSFP is an established module form factor, so USFP&\#x27;s matching size is relevant for compatibility with existing physical layouts. The announcement is a specification release rather than a shipped product.

**「Impact」** If adopted, USFP would let switch and data center operators reach 12.8 Tb/s per module while keeping the OSFP footprint, potentially reducing the number of modules and ports needed for a given throughput. The 100W power support and claimed 1.3x energy efficiency could also ease switch thermal and power design, though no shipping products or independent performance data were announced.

**Tags**: `#optical networking`, `#hardware`, `#NVIDIA`, `#Cisco`, `#data center interconnect`

---