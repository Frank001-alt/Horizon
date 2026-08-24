---
layout: default
title: "Horizon Summary: 2026-08-24 (EN)"
date: 2026-08-24
lang: en
---

> From 187 items, 10 important content pieces were selected

---

**Technology News**
1. [MS Paint and Photos Add Invisible GUID Watermarks to AI-Edited Images](#item-tech-news-1) ⭐️ 8.0/10
2. [seL4 Security Proofs Complete on AArch64](#item-tech-news-2) ⭐️ 8.0/10
3. [Mozilla to Ship JPEG XL in Firefox](#item-tech-news-3) ⭐️ 8.0/10
4. [Emacs 31.1 Released](#item-tech-news-4) ⭐️ 8.0/10
5. [IBM Unveils First Dual-Architecture Mainframe Processor](#item-tech-news-5) ⭐️ 8.0/10

**Financial News**
1. [Oceans Hit Highest Temperature on Record](#item-finance-news-1) ⭐️ 8.0/10
2. [Renewed Attacks Threaten Global Grain Supplies](#item-finance-news-2) ⭐️ 8.0/10
3. [Shein&\#x27;s Valuation Plummets Ahead of IPO](#item-finance-news-3) ⭐️ 8.0/10

**Technology Blog**
1. [Jabber/XMPP: 25 Years of Digital Independence](#item-tech-blog-1) ⭐️ 8.0/10
2. [Your Executable as a SQLite Database](#item-tech-blog-2) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [MS Paint and Photos Add Invisible GUID Watermarks to AI-Edited Images](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

A recent analysis reveals that Microsoft Paint and Microsoft Photos embed invisible GUID watermarks into images that have been AI-manipulated, even when the AI processing is performed locally on the user&\#x27;s device. The watermark is added silently in the background and cannot be disabled, although a visible watermark can be turned off. This raises significant privacy and transparency concerns, as the unique identifier could potentially be used to trace images back to the user&\#x27;s Microsoft account. The exact scope, including whether features like AI-enhanced background removal are affected, remains unclear. The discovery has sparked debate about the implications for user privacy and content authenticity.

hackernews · ComputerGuru · Aug 24, 15:28 · [Discussion](https://news.ycombinator.com/item?id=49421158)

**「Background」** Microsoft Paint and Photos have recently integrated AI-powered editing features, including local AI models for tasks like background removal and image generation. To address concerns about AI-generated content, Microsoft has implemented a watermarking system that embeds a unique GUID into images edited with these AI tools. This GUID is issued by Microsoft&\#x27;s servers after the prompt is moderated, even when the image generation itself occurs locally on the user&\#x27;s device. The watermark is invisible and cannot be disabled, raising questions about user privacy and the transparency of local AI processing.

**「Impact」** Users who create or edit images with AI features in MS Paint or Photos may have their images invisibly linked to their Microsoft account, potentially enabling identification if the images are shared or published. This could undermine anonymity and raise legal exposure, as authorities or copyright holders could subpoena Microsoft for user data.

**「Community Discussion」** Commenters expressed shock that MS Paint has evolved beyond a simple pixel editor and criticized the addition of AI features. One user argued that the AI aspect is a red herring, emphasizing that the real issue is the secret embedding of unique identifiers in every image, which could be used to trace users via copyright subpoenas. Another noted that the invisible watermark is added even when using local models, and questioned whether this violates privacy regulations, while also pointing out that the practice defeats the purpose of local generation.

<details><summary>References</summary>
<ul>
<li><a href="https://zeli.app/story/49421158">Microsoft Paint and Photos Embed Server-Issued GUIDs as... | Zeli</a></li>
<li><a href="https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/">Microsoft Paint and Photos Embed Server-Issued GUIDs as...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#watermarking`, `#AI`, `#Microsoft`, `#content authenticity`

---

<a id="item-tech-news-2"></a>
### [seL4 Security Proofs Complete on AArch64](https://proofcraft.systems/news-2026/#2026-08-21) ⭐️ 8.0/10

The seL4 microkernel&\#x27;s formal security proofs have been completed for the AArch64 architecture, a significant milestone in verified systems security. This achievement extends the high-assurance guarantees of seL4, previously proven on other architectures, to a widely used 64-bit ARM platform. The proofs cover the non-MCS \(mixed criticality systems\) variant and are limited to unicore configurations, as noted in the fine print. This development is expected to bolster confidence in deploying seL4 in security-critical embedded and military systems, though it does not yet address multicore or MCS configurations.

hackernews · snvzz · Aug 24, 11:32 · [Discussion](https://news.ycombinator.com/item?id=49418255)

**「Background」** seL4 is a formally verified microkernel, meaning its source code has been mathematically proven to implement its specification. The verification effort, led by Proofcraft with support from the UK&\#x27;s National Cyber Security Centre \(NCSC\), has previously established functional correctness and integrity proofs. The newly completed confidentiality proof on AArch64 demonstrates that the kernel enforces security isolation between applications, preventing unauthorized information flow. However, the proof currently applies only to non-MCS \(mixed-criticality system\) configurations and single-core setups, with proofs for MCS and RISC-V variants still in progress.

**「Impact」** The completion of seL4&\#x27;s formal verification on AArch64 provides a rare level of assurance for systems relying on this microkernel, potentially accelerating adoption in security-sensitive domains such as automotive, avionics, and defense. However, the limitations to non-MCS and unicore configurations mean that systems requiring multicore support or mixed criticality will not yet benefit from these proofs.

**「Community Discussion」** Commenters expressed skepticism about the practical impact, with one noting that side-channel timing attacks could undermine the security guarantees, and another highlighting the restrictions to non-MCS and unicore configurations. Others discussed the current users of seL4, including GenodeOS, LionsOS, and a Chinese car manufacturer, while questioning whether the capability model truly improves security without a native seL4/Linux integration.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.sel4.systems/projects/sel4/verified-configurations.html">Verified Configurations | seL4 docs</a></li>
<li><a href="https://proofcraft.systems/news-2026/">Proofcraft News - 2026</a></li>

</ul>
</details>

**Tags**: `#seL4`, `#formal verification`, `#AArch64`, `#microkernel`, `#security`

---

<a id="item-tech-news-3"></a>
### [Mozilla to Ship JPEG XL in Firefox](https://hacks.mozilla.org/2026/08/intent-to-ship-jpeg-xl/) ⭐️ 8.0/10

Mozilla has announced its intent to ship JPEG XL, a next-generation image format designed to offer better compression and enhanced features compared to existing formats like JPEG and PNG. This move is significant for web standards, as it could lead to faster loading times and richer image capabilities for web developers and users. JPEG XL supports lossless and lossy compression, high dynamic range, and progressive decoding, among other features. The announcement indicates that Firefox will likely include support for JPEG XL in an upcoming release, though no specific version or date has been provided.

rss · Lobsters · Aug 24, 16:25

**「Background」** JPEG XL is a next-generation image format designed to offer better compression efficiency and advanced features compared to older formats like JPEG and PNG. It was standardized by the JPEG committee and has been under consideration for web adoption. Safari shipped a version of JPEG XL in 2023, but its implementation lacked some features, such as progressive rendering, which allows images to display while downloading. Chrome has also shipped JPEG XL, and Google has developed a Rust-based decoder called jxl-rs. Mozilla&\#x27;s intent to ship JPEG XL in Firefox marks a significant step toward broader browser support for the format.

**「Impact」** Web developers and users of Firefox will benefit from improved image compression and new features, potentially reducing bandwidth usage and enabling more advanced image display on the web. However, the impact depends on broader adoption across other browsers and platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://hacks.mozilla.org/2026/08/intent-to-ship-jpeg-xl/">Intent to Ship : JPEG XL - Mozilla Hacks - the Web developer blog</a></li>
<li><a href="https://www.phoronix.com/news/Firefox-JPEG-XL-2026-Plans">Mozilla Presents Their Plan For Shipping JPEG - XL In... - Phoronix</a></li>

</ul>
</details>

**Tags**: `#JPEG XL`, `#web standards`, `#image compression`, `#Mozilla`, `#browser`

---

<a id="item-tech-news-4"></a>
### [Emacs 31.1 Released](https://lists.gnu.org/archive/html/info-gnu-emacs/2026-08/msg00004.html) ⭐️ 8.0/10

Emacs 31.1 has been officially released, marking a major update to the popular open-source text editor. The announcement was made on the official GNU mailing list, confirming the release&\#x27;s authority. This version is significant for the Emacs community, as major releases typically introduce new features, improvements, and bug fixes. The release is particularly relevant for software engineers and developers who rely on Emacs for their daily work. While the announcement does not include a detailed changelog, the release itself is a notable event for the open-source ecosystem.

rss · Lobsters · Aug 24, 10:52

**「Background」** Emacs is a highly extensible and customizable text editor that has been a cornerstone of the free software movement since its creation in the 1970s. It is known for its powerful editing capabilities, extensive package ecosystem, and Lisp-based extension language. Major version releases, such as 31.1, are infrequent and typically bring substantial changes, making them eagerly anticipated by the community.

**「Impact」** The release of Emacs 31.1 provides users with a new stable version that likely includes improvements in performance, usability, and compatibility, potentially affecting how developers and enthusiasts use the editor. However, without a detailed changelog, the specific impact remains uncertain until further details are published.

**Tags**: `#Emacs`, `#release`, `#open source`, `#text editor`, `#GNU`

---

<a id="item-tech-news-5"></a>
### [IBM Unveils First Dual-Architecture Mainframe Processor](https://www.ithome.com/0/993/720.htm) ⭐️ 8.0/10

IBM announced its first dual-architecture mainframe processor at the Hot Chips 2026 conference on August 24. Built on a 2nm process, the chip integrates 11 high-performance cores running at over 5.7GHz, along with AI inference accelerators, an on-chip DPU, and large caches. The processor enables IBM Z and LinuxONE systems to natively execute both IBM Z/LinuxONE and Arm instructions, allowing enterprises to run operating systems and applications from both ecosystems simultaneously. This milestone stems from the IBM-Arm partnership and aims to bridge Arm&\#x27;s software ecosystem with IBM&\#x27;s enterprise capabilities. The resulting systems can scale to hundreds of cores and tens of terabytes of memory.

rss · IT HOME · Aug 24, 12:21

**「Background」** IBM mainframes traditionally run on IBM&\#x27;s proprietary z/Architecture, which supports IBM Z and LinuxONE systems. The company has been exploring ways to expand the mainframe&\#x27;s application ecosystem, and in 2021 announced a partnership with Arm to bring Arm technology to its enterprise offerings. This new processor is the first concrete result of that collaboration, allowing each core to natively execute both IBM Z and Arm instructions.

**「Impact」** Enterprises using IBM Z and LinuxONE systems will be able to run Arm-based workloads natively on the same hardware, potentially reducing the need for separate Arm infrastructure and enabling tighter integration between IBM&\#x27;s enterprise stack and the broader Arm software ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techzine.eu/news/infrastructure/143778/ibm-develops-mainframe-chip-that-also-runs-arm-code/">IBM develops mainframe chip that also runs Arm ... - Techzine Global</a></li>
<li><a href="https://thecuberesearch.com/ibm-opens-the-mainframe-to-arm-and-widens-zs-moat/">IBM Opens the Mainframe to Arm — and... - theCUBE Research</a></li>

</ul>
</details>

**Tags**: `#IBM`, `#mainframe`, `#processor`, `#2nm`, `#Arm`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Oceans Hit Highest Temperature on Record](https://www.bbc.com/news/articles/c62m4gpnp78o) ⭐️ 8.0/10

Oceans have reached their highest temperature on record, according to a BBC report, signaling accelerating climate change with wide-ranging implications. The record is based on recent measurements, though specific figures and baseline comparisons are not provided in the source.

hackernews · tcp\_handshaker · Aug 24, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49424606)

**「Background」** El Niño is a natural climate pattern that periodically warms the Pacific Ocean, often boosting global temperatures. Combined with long-term human-caused climate change, it has helped push ocean temperatures to record highs.

**「Impact」** Warmer oceans can intensify rainfall and storms, and prolonged marine heat waves stress coral reefs, fisheries, and coastal habitats, threatening the livelihoods of communities that depend on them.

<details><summary>References</summary>
<ul>
<li><a href="https://www.abc.net.au/news/2026-08-25/ocean-temperatures-hit-record-spurred-by-el-ni%C3%B1o/107073982">Ocean temperatures hit &#x27;very troubling&#x27; record high - ABC News</a></li>
<li><a href="https://www.livescience.com/planet-earth/climate-change/ocean-under-unprecedented-strain-as-el-nino-helps-supercharge-warming-to-record-levels">Ocean &#x27;under unprecedented strain&#x27; as El Niño helps... | Live Science</a></li>
<li><a href="https://www.theguardian.com/environment/2026/aug/24/worlds-oceans-hit-hottest-temperature-on-record-in-august">World’s oceans hit hottest temperature on record in August | Oceans | The Guardian</a></li>
<li><a href="https://www.syracuse.com/us-news/2026/08/something-unusual-is-happening-beneath-the-oceans-surface-and-scientists-are-alarmed.html">Global ocean temperatures break ancient record as marine heat waves spread worldwide - syracuse.com</a></li>

</ul>
</details>

**Tags**: `#climate change`, `#ocean temperature`, `#environment`, `#global warming`, `#El Niño`

---

<a id="item-finance-news-2"></a>
### [Renewed Attacks Threaten Global Grain Supplies](https://www.economist.com/europe/2026/08/24/the-renewed-threat-to-global-grain-supplies) ⭐️ 8.0/10

Renewed attacks on both Ukrainian and Russian grain exports are threatening global food supplies, according to The Economist. Unlike in 2022, when only Ukraine&\#x27;s exports were affected, now both countries&\#x27; exports are under attack, which could disrupt a significant portion of global grain trade.

rss · The Economist · Aug 24, 16:35

**「Background」** In 2022, Russia&\#x27;s invasion of Ukraine disrupted grain exports, but now both countries&\#x27; exports are under attack, threatening global food supplies. Ukraine has proposed a deal to halt attacks on civilian targets in the Black Sea to allow grain shipments to resume from both countries.

**「Impact」** This development could lead to higher food prices and increased food insecurity, particularly in import-dependent regions such as the Middle East and Africa, which rely heavily on grain from these exporters.

<details><summary>References</summary>
<ul>
<li><a href="https://www.economist.com/europe/2026/08/24/the-renewed-threat-to-global-grain-supplies">The renewed threat to global grain supplies - The Economist</a></li>
<li><a href="https://theconversation.com/russia-is-cutting-off-ukraines-grain-exports-again-threatening-a-critical-harvest-and-global-food-security-289718">Russia is cutting off Ukraine&#x27;s grain exports again, threatening a ...</a></li>

</ul>
</details>

**Tags**: `#grain exports`, `#global food security`, `#Ukraine`, `#Russia`, `#agriculture`

---

<a id="item-finance-news-3"></a>
### [Shein&\#x27;s Valuation Plummets Ahead of IPO](https://www.economist.com/business/2026/08/24/how-shein-came-crashing-down) ⭐️ 8.0/10

Shein is listing at a valuation of $25bn, a quarter of its previous $100bn valuation, according to The Economist.

rss · The Economist · Aug 24, 15:14

**「Background」** Shein, a Chinese-founded fast-fashion e-retailer, was once valued at $100 billion in 2022. Its valuation has since fallen sharply due to regulatory scrutiny, intense competition from rivals like Temu and Amazon, and the loss of duty-free access to the U.S. market, which has pressured its margins.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/markfaithfull/2026/08/24/the-shein-ipo-is-finally-on-but-it-has-lost-70-in-value-along-the-way/">The Shein IPO Is Finally On But It Has Lost 70% In Value Along The...</a></li>
<li><a href="https://www.roic.ai/news/sheins-ipo-ambitions-tumble-to-25b-as-fast-fashion-model-faces-headwinds-08-17-2026">Shein ’s IPO Ambitions Tumble to $25B as Fast-Fashion... | Roic News</a></li>
<li><a href="https://ionanalytics.com/insights/dealogic/shein-valuation-reset-reflects-tariff-reality-as-focus-shifts-to-execution/">Shein valuation reset reflects tariff reality as focus... - ION Analytics</a></li>

</ul>
</details>

**Tags**: `#Shein`, `#IPO`, `#valuation`, `#e-commerce`, `#retail`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Jabber/XMPP: 25 Years of Digital Independence](https://gultsch.de/posts/25-years-of-digital-independence/) ⭐️ 8.0/10

hackernews · inputmice · Aug 24, 15:51 · [Discussion](https://news.ycombinator.com/item?id=49421536)

**「Background」** The author reflects on the 25th anniversary of Jabber/XMPP, a protocol that has enabled federated, open instant messaging since its inception. Despite being overshadowed by proprietary platforms and newer protocols like Matrix, XMPP remains a cornerstone of digital independence, offering a decentralized alternative to centralized communication services.

**「Solution」** The author, a long-time XMPP contributor, traces the protocol&\#x27;s evolution from its early days to its current state, highlighting key technical milestones such as the development of extensions \(XEPs\) that have kept it adaptable. He discusses the ecosystem&\#x27;s challenges, including the rise and fall of major adopters like Google and Facebook, and the fragmentation of clients and servers. He argues that XMPP&\#x27;s strength lies in its simplicity and extensibility, which have allowed it to persist despite competition. He also addresses the comparison with Matrix, noting that while Matrix offers modern features, XMPP&\#x27;s federated model and mature standards provide a more stable foundation for long-term digital independence. The author shares practical lessons from his experience, such as the importance of backward compatibility and community governance, and acknowledges tradeoffs like the complexity of implementing certain features.

**「Takeaway」** The author concludes that XMPP&\#x27;s enduring relevance stems from its commitment to open standards and federation, which empower users to control their communication infrastructure. Its 25-year history demonstrates that digital independence is achievable through persistent, community-driven protocol development.

**Tags**: `#XMPP`, `#protocol design`, `#federation`, `#open standards`, `#ecosystem`

---

<a id="item-tech-blog-2"></a>
### [Your Executable as a SQLite Database](https://fzakaria.com/2026/08/23/your-executable-is-a-sqlite-database) ⭐️ 8.0/10

rss · Lobsters · Aug 24, 07:32

**「Background」** Farid Zakaria explores a novel Linux pattern where a SQLite database file is crafted to also serve as an executable binary. Traditionally, executables and data files are distinct, but this approach blurs the line by embedding an ELF executable within a SQLite database, enabling SQL-based introspection and manipulation of the binary itself.

**「Solution」** The trick leverages SQLite&\#x27;s 4-byte application ID field, located 68 bytes into the file, by setting it to &\#x27;SELF&\#x27; \(Structured Executable &amp; Linkable Format\). The ELF components are then organized into SQLite tables according to a specific schema. A custom interpreter, self-exec, extracts and executes the necessary parts. Additionally, Linux&\#x27;s binfmt\_misc mechanism can be configured to recognize executables with this pattern and invoke the interpreter automatically, as demonstrated with a registration command. This allows the executable to be queried and modified using SQL, offering a unique approach to binary analysis and data embedding.

**「Takeaway」** The author demonstrates that by creatively using file format features, an executable can be treated as a database, enabling powerful introspection and manipulation capabilities that could change how binaries are analyzed and managed.

**Tags**: `#SQLite`, `#executable`, `#binary analysis`, `#data embedding`, `#systems programming`

---