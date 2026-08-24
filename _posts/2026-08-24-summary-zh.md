---
layout: default
title: "Horizon Summary: 2026-08-24 (ZH)"
date: 2026-08-24
lang: zh
---

> 从 187 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [MS Paint 和照片应用为本地 AI 编辑图片添加隐形 GUID 水印](#item-tech-news-1) ⭐️ 8.0/10
2. [seL4 在 AArch64 上的形式化安全证明完成](#item-tech-news-2) ⭐️ 8.0/10
3. [Mozilla 宣布计划在 Firefox 中支持 JPEG XL](#item-tech-news-3) ⭐️ 8.0/10
4. [Emacs 31.1 正式发布](#item-tech-news-4) ⭐️ 8.0/10
5. [IBM 发布首款双架构大型机处理器：2nm 工艺，11 核心 5.7GHz](#item-tech-news-5) ⭐️ 8.0/10

**财经新闻**
1. [全球海洋温度创历史新高](#item-finance-news-1) ⭐️ 8.0/10
2. [全球粮食供应面临新威胁](#item-finance-news-2) ⭐️ 8.0/10
3. [希音上市估值大幅缩水](#item-finance-news-3) ⭐️ 8.0/10

**科技博客**
1. [Jabber/XMPP：25 年的数字独立](#item-tech-blog-1) ⭐️ 8.0/10
2. [将可执行文件视为 SQLite 数据库](#item-tech-blog-2) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [MS Paint 和照片应用为本地 AI 编辑图片添加隐形 GUID 水印](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

微软的 MS Paint 和 Photos 应用在本地 AI 编辑生成的图片中嵌入不可见的 GUID 水印，即使使用本地模型处理也无法禁用。该水印在后台静默添加，用户无感知，可能用于追踪图片来源。这一发现引发了对用户隐私和内容透明度的担忧，因为水印可能关联到用户的 Microsoft 账户。目前尚不清楚是否所有 AI 操作（如背景删除）都会触发水印，但已确认部分 AI 编辑功能会添加。

hackernews · ComputerGuru · 8月24日 15:28 · [社区讨论](https://news.ycombinator.com/item?id=49421158)

**「背景」** 微软的画图（MS Paint）和照片（Photos）应用现在内置了本地 AI 图像编辑功能，例如 AI 增强的背景删除或图像生成。这些功能在本地运行 AI 模型，但根据逆向工程分析，当用户使用这些 AI 功能时，应用会向微软服务器发送提示词，服务器审核后返回一个唯一的 GUID，该 GUID 作为不可见水印嵌入到本地生成的图像中。这意味着即使图像完全在本地生成，也会包含一个可追踪的标识符。

**「影响」** 对于使用 MS Paint 或 Photos 进行 AI 编辑的 Windows 用户，其生成的图片可能携带可追踪的隐形标识，若图片被公开，第三方可能通过法律途径向微软索取用户个人信息，从而威胁匿名性。

**「社区讨论」** 社区评论指出，AI 方面是转移注意力的焦点，真正的问题在于微软在用户创建的每张图片中秘密添加唯一标识符，可能被用于追踪用户身份。也有用户提到，微软此前曾错误地为 Azure DevOps 提交添加 Copilot 水印，引发争议后撤回，暗示此类行为可能并非首次。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zeli.app/story/49421158">Microsoft Paint and Photos Embed Server-Issued GUIDs as... | Zeli</a></li>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs as...</a></li>

</ul>
</details>

**标签**: `#privacy`, `#watermarking`, `#AI`, `#Microsoft`, `#content authenticity`

---

<a id="item-tech-news-2"></a>
### [seL4 在 AArch64 上的形式化安全证明完成](https://proofcraft.systems/news-2026/#2026-08-21) ⭐️ 8.0/10

seL4 微内核在 AArch64 架构上的形式化安全证明现已完成，这是验证微内核部署中的一个重要里程碑。该证明复盖了非 MCS（混合关键性系统）和单核配置，为广泛使用的架构提供了罕见的高级别安全保证。这一成就对操作系统和安全社区具有重要价值，尽管社区评论指出其局限性，如不支持多核和 MCS 特性。

hackernews · snvzz · 8月24日 11:32 · [社区讨论](https://news.ycombinator.com/item?id=49418255)

**「背景」** seL4 是一个经过形式化验证的微内核，其正确性、完整性和机密性证明此前主要针对特定架构完成。AArch64 是 64 位 ARM 架构，广泛用于移动设备和嵌入式系统。此前，seL4 在 AArch64 上的机密性证明尚未完成，而 Proofcraft 在 NCSC 的支持下，于 2026 年 1 月宣布完成了该证明，确保内核能防止其上运行的应用程序未经授权获取信息。

**「影响」** 这一完成将增强 seL4 在安全关键系统（如军事和嵌入式市场）中的可信度，但当前证明的局限性（非 MCS、单核）可能限制其在更广泛多核系统中的应用。

**「社区讨论」** 社区评论指出该证明的局限性，如仅覆盖非 MCS 和单核配置，并质疑侧信道攻击可能影响结果。此外，讨论涉及 seL4 的实际使用案例，包括 GenodeOS、LionsOS 以及中国汽车制造商将其用作虚拟机监控程序，但有人认为需要原生 seL4/Linux 才能更广泛地改善系统安全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://proofcraft.systems/news-2026/">Proofcraft News - 2026</a></li>

</ul>
</details>

**标签**: `#seL4`, `#formal verification`, `#AArch64`, `#microkernel`, `#security`

---

<a id="item-tech-news-3"></a>
### [Mozilla 宣布计划在 Firefox 中支持 JPEG XL](https://hacks.mozilla.org/2026/08/intent-to-ship-jpeg-xl/) ⭐️ 8.0/10

Mozilla 宣布有意在 Firefox 浏览器中支持 JPEG XL，这是一种下一代图像格式，旨在提供比现有格式更好的压缩效率和更丰富的功能。JPEG XL 支持有损和无损压缩，具有更高的压缩率、更快的解码速度，并支持宽色域、高动态范围（HDR）和动画等高级特性。该格式由 JPEG 委员会开发，并已得到多家公司的支持。Mozilla 的这一决定意味着 Firefox 用户将能够使用这种格式，从而可能推动 Web 上图像标准的演进。目前，Chrome 和 Safari 已部分或完全支持 JPEG XL，而 Firefox 的加入将进一步扩大其生态。

rss · Lobsters · 8月24日 16:25

**「背景」** JPEG XL 是一种下一代图像格式，旨在提供比现有格式（如 JPEG、PNG 和 WebP）更好的压缩效率和更丰富的功能。Safari 已于 2023 年支持 JPEG XL，但其实现缺少一些关键特性，例如渐进式渲染，而 Mozilla 在 Rust 实现中推动了这一特性。Chrome 也已支持 JPEG XL，并且 Google Research 开发了基于 Rust 的 jxl-rs 解码器，同时 Google 正式宣布计划在 Blink 引擎中默认启用 JPEG XL 解码。

**「影响」** 对于 Web 开发者和图像处理相关用户，Firefox 支持 JPEG XL 将提供更高效的图像压缩选项，减少带宽消耗并提升加载性能，同时支持 HDR 和动画等新特性，有助于提升用户体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hacks.mozilla.org/2026/08/intent-to-ship-jpeg-xl/">Intent to Ship : JPEG XL - Mozilla Hacks - the Web developer blog</a></li>
<li><a href="https://www.phoronix.com/news/Firefox-JPEG-XL-2026-Plans">Mozilla Presents Their Plan For Shipping JPEG - XL In... - Phoronix</a></li>

</ul>
</details>

**标签**: `#JPEG XL`, `#web standards`, `#image compression`, `#Mozilla`, `#browser`

---

<a id="item-tech-news-4"></a>
### [Emacs 31.1 正式发布](https://lists.gnu.org/archive/html/info-gnu-emacs/2026-08/msg00004.html) ⭐️ 8.0/10

Emacs 31.1 已由 GNU 官方邮件列表正式发布，这是这款广受欢迎的文本编辑器的一次重大版本更新。该版本标志着 Emacs 在功能、性能和稳定性方面的重要进展，但官方公告未提供详细的变更日志。作为开源软件，Emacs 31.1 的发布对全球开发者社区具有重要意义，用户可通过官方渠道获取更新。

rss · Lobsters · 8月24日 10:52

**「背景」** Emacs 是一款历史悠久的开源文本编辑器，以其高度可扩展性和强大的编辑功能著称，深受软件工程师和高级用户的喜爱。GNU 项目定期发布新版本，每个主版本号（如 31.1）通常包含新特性、改进和错误修复。此次发布延续了 Emacs 长期以来的版本迭代传统。

**「影响」** 对于依赖 Emacs 进行日常开发工作的用户和开发者，31.1 版本可能带来性能提升和新功能，但具体影响需待详细变更日志公布后才能明确。建议用户关注官方发布说明以了解更新内容。

**标签**: `#Emacs`, `#release`, `#open source`, `#text editor`, `#GNU`

---

<a id="item-tech-news-5"></a>
### [IBM 发布首款双架构大型机处理器：2nm 工艺，11 核心 5.7GHz](https://www.ithome.com/0/993/720.htm) ⭐️ 8.0/10

IBM 在 Hot Chips 2026 大会上发布了首款双架构大型机处理器，标志着 IBM 与 Arm 合作在处理器领域的首个里程碑。该处理器基于 2nm 先进逻辑制程工艺，整合了 11 个运行频率超过 5.7GHz 的高性能核心、AI 推理加速器、片上 DPU 和大容量缓存。基于该处理器的 Z 和 LinuxONE 系统允许企业客户同时在 IBM 和 Arm 计算平台上运行操作系统和应用程序，其核心均可原生执行 IBM Z / LinuxONE 和 Arm 指令。此举实现了 Arm 软件生态系统与 IBM 企业级能力的互通，双方可吸收对方的优势。基于该处理器的系统可扩展至数百个核心和数十 TB 的内存。

rss · IT HOME · 8月24日 12:21

**「背景」** 大型机（Mainframe）是面向企业关键任务的高端服务器，传统上使用 IBM 专有的 z/Architecture 指令集，运行 z/OS 或 LinuxONE 等操作系统。Arm 架构则广泛应用于移动设备和云服务器，拥有庞大的软件生态。IBM 与 Arm 此前已有合作关系，但本次在 Hot Chips 2026 大会上发布的处理器是双方合作在处理器领域的首个里程碑，每个核心都能原生执行 IBM Z/LinuxONE 和 Arm 指令，从而在保持大型机核心能力的同时，扩展其应用生态。

**「影响」** 该处理器将直接影响使用 IBM Z 和 LinuxONE 系统的企业客户，使他们能够在同一硬件上运行 IBM 和 Arm 工作负载，从而简化基础设施并降低多样性成本。此外，这也可能促进 Arm 生态在企业级应用中的采用，并推动 IBM 在 AI 和高性能计算领域的竞争力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.techzine.eu/news/infrastructure/143778/ibm-develops-mainframe-chip-that-also-runs-arm-code/">IBM develops mainframe chip that also runs Arm ... - Techzine Global</a></li>
<li><a href="https://blockonomi.com/ibm-ibm-unveils-groundbreaking-dual-architecture-mainframe-chip-with-arm-integration/">IBM ( IBM ) Unveils Groundbreaking Dual-Architecture Mainframe Chip...</a></li>
<li><a href="https://thecuberesearch.com/ibm-opens-the-mainframe-to-arm-and-widens-zs-moat/">IBM Opens the Mainframe to Arm — and... - theCUBE Research</a></li>

</ul>
</details>

**标签**: `#IBM`, `#mainframe`, `#processor`, `#2nm`, `#Arm`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [全球海洋温度创历史新高](https://www.bbc.com/news/articles/c62m4gpnp78o) ⭐️ 8.0/10

据 BBC 报道，全球海洋温度已达到有记录以来的最高水平，这是气候变化加速的一个关键指标。这一数据点表明海洋吸收了更多热量，可能加剧极端天气事件。

hackernews · tcp\_handshaker · 8月24日 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49424606)

**「背景」** 海洋温度创下历史新高，部分原因是厄尔尼诺现象，这是一种自然气候模式，其特征是太平洋水域异常温暖，通常会推高全球气温。

**「影响」** 海洋温度创纪录升高，将加剧极端天气，因为较暖的海洋向大气传递更多能量和水汽，使降雨和风暴更强。同时，海洋热浪会给珊瑚礁、渔业和沿海栖息地带来压力，威胁依赖这些生态系统的社区生计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.livescience.com/planet-earth/climate-change/ocean-under-unprecedented-strain-as-el-nino-helps-supercharge-warming-to-record-levels">Ocean &#x27;under unprecedented strain&#x27; as El Niño helps... | Live Science</a></li>
<li><a href="https://www.theguardian.com/environment/2026/aug/24/worlds-oceans-hit-hottest-temperature-on-record-in-august">World’s oceans hit hottest temperature on record in August | Oceans | The Guardian</a></li>
<li><a href="https://www.syracuse.com/us-news/2026/08/something-unusual-is-happening-beneath-the-oceans-surface-and-scientists-are-alarmed.html">Global ocean temperatures break ancient record as marine heat waves spread worldwide - syracuse.com</a></li>

</ul>
</details>

**标签**: `#climate change`, `#ocean temperature`, `#environment`, `#global warming`, `#El Niño`

---

<a id="item-finance-news-2"></a>
### [全球粮食供应面临新威胁](https://www.economist.com/europe/2026/08/24/the-renewed-threat-to-global-grain-supplies) ⭐️ 8.0/10

据《经济学人》报道，乌克兰和俄罗斯的谷物出口均受到攻击，这对全球粮食供应构成重大威胁。与 2022 年不同，此次两国的出口都面临风险。

rss · The Economist · 8月24日 16:35

**「背景」** 2022 年，俄罗斯入侵乌克兰后，全球粮食供应曾受到威胁。如今，乌克兰和俄罗斯的谷物出口均遭到攻击，这可能导致全球粮食供应再次紧张。

**「影响」** 依赖谷物进口的国家可能面临供应短缺和价格上涨，全球粮食安全形势趋于严峻。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.economist.com/europe/2026/08/24/the-renewed-threat-to-global-grain-supplies">The renewed threat to global grain supplies - The Economist</a></li>
<li><a href="https://www.themoscowtimes.com/2026/08/24/kremlin-says-its-working-to-minimize-impact-of-ukrainian-attacks-on-russian-grain-exports-a93566">Kremlin Says It&#x27;s Working to Minimize Impact of Ukrainian Attacks on ...</a></li>

</ul>
</details>

**标签**: `#grain exports`, `#global food security`, `#Ukraine`, `#Russia`, `#agriculture`

---

<a id="item-finance-news-3"></a>
### [希音上市估值大幅缩水](https://www.economist.com/business/2026/08/24/how-shein-came-crashing-down) ⭐️ 8.0/10

中国电商零售商希音（Shein）上市，估值仅为 250 亿美元，是其此前 1000 亿美元估值的四分之一。

rss · The Economist · 8月24日 15:14

**「背景」** Shein 曾于 2022 年达到约 982 亿美元的估值峰值，但此后因面临监管审查、竞争加剧以及美国取消其关税豁免等挑战，估值大幅缩水。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.forbes.com/sites/markfaithfull/2026/08/24/the-shein-ipo-is-finally-on-but-it-has-lost-70-in-value-along-the-way/">The Shein IPO Is Finally On But It Has Lost 70% In Value Along The...</a></li>
<li><a href="https://www.roic.ai/news/sheins-ipo-ambitions-tumble-to-25b-as-fast-fashion-model-faces-headwinds-08-17-2026">Shein ’s IPO Ambitions Tumble to $25B as Fast-Fashion... | Roic News</a></li>

</ul>
</details>

**标签**: `#Shein`, `#IPO`, `#valuation`, `#e-commerce`, `#retail`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [Jabber/XMPP：25 年的数字独立](https://gultsch.de/posts/25-years-of-digital-independence/) ⭐️ 8.0/10

hackernews · inputmice · 8月24日 15:51 · [社区讨论](https://news.ycombinator.com/item?id=49421536)

**「背景」** 在即时通讯领域，XMPP（可扩展消息处理现场协议）已走过 25 年历程。作者回顾了这一开放标准的兴衰，指出其面临的主要挑战：尽管早期被 Google、Facebook 等巨头采用，但后来这些公司纷纷退出，导致生态系统碎片化。然而，XMPP 的核心价值——去中心化、联邦制和开放标准——依然吸引着忠实用户。

**「方案」** 作者深入探讨了 XMPP 的技术演进和生态系统的韧性。他强调了协议设计的灵活性，如通过 XEP 扩展实现新功能，以及联邦制带来的互操作性。尽管面临 Matrix 等新协议的竞争，XMPP 仍通过社区驱动的开发保持活力。作者还分享了实际应用案例，如将 XMPP 用于代理通信，以及通过桥接服务（如 jmp.chat）实现电话和短信功能。这些实践展示了 XMPP 在特定场景下的实用性和可扩展性。

**「启示」** 作者的核心论点是，XMPP 的持久价值在于其对数字独立的承诺——通过开放标准和联邦制，用户能够掌控自己的通信基础设施，而不受单一供应商的束缚。这种独立性在当今互联网环境中尤为珍贵。

**标签**: `#XMPP`, `#protocol design`, `#federation`, `#open standards`, `#ecosystem`

---

<a id="item-tech-blog-2"></a>
### [将可执行文件视为 SQLite 数据库](https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database) ⭐️ 8.0/10

rss · Lobsters · 8月24日 07:32

**「背景」** 传统上，可执行文件是二进制格式，难以直接进行结构化查询或修改。Farid Zakaria 提出了一种巧妙的方法，将 SQLite 数据库文件本身设计为可执行文件，从而允许通过 SQL 查询来检查和操作二进制内容。

**「方案」** 作者利用 SQLite 文件格式中的 4 字节应用 ID（位于文件偏移 68 字节处）设置为“SELF”，代表“结构化可执行与链接格式”。然后，他将 ELF 可执行格式的各个组件组织成多个 SQLite 表，并提供了一个名为 \`self-exec\` 的解释器（C 代码），用于提取并执行必要的部分。此外，通过 Linux 的 \`binfmt\_misc\` 机制，可以注册该二进制模式，使内核在遇到匹配的可执行文件时自动调用 \`self-exec\`。作者在 NixOS 上实现了这一模式，并提供了非 NixOS 下的注册示例。

**「启示」** 作者的核心观点是，通过将可执行文件与 SQLite 数据库结合，可以开启一种新的二进制分析和数据嵌入方式，使开发者能够利用 SQL 的灵活性来理解和操作程序结构。

**标签**: `#SQLite`, `#executable`, `#binary analysis`, `#data embedding`, `#systems programming`

---