---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 201 items, 10 important content pieces were selected

---

**Technology News**
1. [Qwen3.8-2.4T-A95B: Massive MoE Model Released](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 Released](#item-tech-news-2) ⭐️ 8.0/10
3. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](#item-tech-news-3) ⭐️ 8.0/10
4. [Grok 4.6 Scores 61 on Artificial Analysis Intelligence Index](#item-tech-news-4) ⭐️ 8.0/10
5. [Signal Introduces Automatic Key Verification](#item-tech-news-5) ⭐️ 8.0/10
6. [Fudan Team First Creates Single-Layer CuO2 High-Temp Superconductor](#item-tech-news-6) ⭐️ 8.0/10
7. [China&\#x27;s Breakthrough in Lepidolite Lithium Extraction](#item-tech-news-7) ⭐️ 8.0/10
8. [Honor Robot Phone Pre-orders Exceed 400,000](#item-tech-news-8) ⭐️ 8.0/10
9. [LTX-2.5: Open-Source Video Model Runs on RTX 5090](#item-tech-news-9) ⭐️ 8.0/10

**Technology Blog**
1. [Why Tiny JPEGs Look Different in Chrome](#item-tech-blog-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen3.8-2.4T-A95B: Massive MoE Model Released](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen has released Qwen3.8-2.4T-A95B, a massive Mixture-of-Experts \(MoE\) language model with 2.4 trillion total parameters and 95 billion active parameters per token. The model supports a native context length of 262,144 tokens, extendable to 1,010,000 tokens, and is available in BF16 and FP8 formats, with a 1-bit quantized version at 397GB. Performance is claimed to be between Opus 4.8 and Fable 5, and the model is positioned as a rival to Kimi k3. The open-weight release lacks vision input and non-thinking support, which are exclusive to the official Qwen3.8-Max version.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**「Background」** Qwen is a family of large language models developed by Alibaba, with Qwen3.8 being the latest iteration. The open-weights release of Qwen3.8-2.4T-A95B on 12 August 2026 marks the first time a Qwen-Max-class model has been made openly available, following the release of Moonshot AI&\#x27;s competing Kimi K3 model. The model uses a mixture-of-experts \(MoE\) architecture with 2.4 trillion total parameters and 95 billion activated per token, and it omits certain cloud-model features such as image input and a non-thinking mode.

**「Impact」** The 1-bit quantized version at 397GB makes Opus 4.5-level performance accessible on high-end consumer hardware, potentially democratizing access to frontier AI capabilities. However, the lack of QAT on q4 means that serving the model at scale will require significant resources or external quantization efforts, limiting immediate deployment for smaller organizations.

**「Community Discussion」** Community members note the model&\#x27;s size and quantization challenges, with some pointing out that the BF16 version is 4.9TB and the 1-bit version is 397GB, making it a &\#x27;chonker&\#x27; that is harder to serve than Kimi k3 at launch. Others highlight the licensing caveats, including free use for internal purposes or revenue under $50M per year, and express disappointment that the open-weight model lacks vision support and the 1M context length of the official version.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B">Qwen/Qwen3.8-2.4T-A95B · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#Qwen`, `#large language models`, `#MoE`, `#AI release`, `#model quantization`

---

<a id="item-tech-news-2"></a>
### [DeepSeek V4 Pro 0813 Released](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 \(DeepSeek-V4-Pro-0813\) was officially released on August 13 and updated to the API, with the model name unchanged. The new version enhances agent capabilities, supports the Responses API and Codex integration, and shows significant improvements over the preview version, approaching Fable 5 performance in multiple benchmarks. Pricing is set at 0.025 yuan per million tokens for cached input, 3 yuan per million tokens for uncached input, and a specified output price \(not fully provided\). Community tests on OpenRouter show it completed a coding task in 12 minutes 2 seconds at a cost of $0.12 but with a bug, compared to Grok 4.6 which took 3 minutes 18 seconds at $1.41 without a bug, highlighting its low cost but potential reliability trade-offs.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**「Background」** DeepSeek V4 Pro 0813 is the general-availability release of DeepSeek&\#x27;s V4 Pro model, succeeding the earlier preview version. It is designed for coding, tool use, cybersecurity, automation, and long-horizon agent workflows, and it supports the Responses API and Codex integration. The model was released on August 12, 2026, and is accessible via DeepSeek&\#x27;s API. Vendor-reported benchmarks indicate it outperforms both the V4 Flash 0731 and the V4 Pro Preview on all listed agent benchmarks, approaching the performance of Fable 5.

**「Impact」** Developers using DeepSeek models for coding tasks can now access a significantly improved, low-cost model, potentially reducing expenses dramatically compared to alternatives like Grok 4.6, though they may need to account for occasional bugs in output.

**「Community Discussion」** Commenters expressed enthusiasm about DeepSeek&\#x27;s cost-effectiveness, with one noting the previous Flash update enabled heavy development for &\#x27;peanuts&\#x27; and another sharing a direct comparison showing DeepSeek V4 Pro 0813 was much cheaper but produced a bug, while Grok 4.6 was faster and bug-free. Some criticized the OpenRouter link for lacking useful information, suggesting official API docs or benchmark posts instead.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseekv4pro.com/news/deepseek-v4-pro-0813-official-release-opus-fable-benchmarks">DeepSeek V 4 Pro 0813 : Opus 4.8 and Fable 5 Agent Benchmarks</a></li>
<li><a href="https://lmmarketcap.com/model/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 - Pricing &amp; Benchmarks 2026 | LM Market Cap</a></li>
<li><a href="https://nano-gpt.com/models/text/deepseek/deepseek-v4-pro-0813">DeepSeek V 4 Pro 0813 model | NanoGPT</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#Open Source`, `#Cost Efficiency`

---

<a id="item-tech-news-3"></a>
### [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale&\#x27;s engineering blog details a rare SQLite WAL-reset race condition that corrupted databases, despite a single-writer design. The bug, a 16-year-old issue, was isolated using an open-source SQLite VFS shim funded by Tailscale, which will aid future debugging. The root cause involved a race between writer and checkpointing logic, and the fix has been released in a SQLite update. The post highlights Tailscale&\#x27;s investment in open-source tooling and a support contract with SQLite.

hackernews · Lobsters · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**「Background」** SQLite is an embedded database that uses a Write-Ahead Log \(WAL\) to improve concurrency and performance. In WAL mode, changes are appended to a separate log file before being checkpointed into the main database. The WAL-Reset bug is a data race in SQLite&\#x27;s checkpointing code that has existed since version 3.7.0 \(July 2010\) and affects all versions through 3.51.2. It was fixed in SQLite 3.51.3, released on March 13, 2026. Tailscale, which uses SQLite as the control plane database for its coordination service, encountered 19 database corruptions over six months before tracing the issue to this race condition.

**「Impact」** Tailscale users and developers relying on SQLite in single-writer configurations may have experienced database corruption due to this bug; the fix in the SQLite release resolves it, and the funded VFS shim provides a reusable tool for diagnosing similar concurrency issues.

**「Community Discussion」** Commenters praised the article&\#x27;s clarity and Tailscale&\#x27;s funding of open-source debugging tools, with some noting the surprise that a single-writer design could still hit a race. Others appreciated the detailed write-up and hoped Tailscale continues supporting SQLite.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://www.theregister.com/databases/2026/08/12/tailscale-says-deeply-buried-16-year-old-sqlite-bug-caused-last-years-outages/5287004">Tailscale says deeply buried 16-year-old SQLite bug caused ...</a></li>
<li><a href="https://byteiota.com/sqlite-wal-bug-tailscale-found-it-after-19-corruptions/">SQLite WAL Bug: Tailscale Found It After 19 Corruptions</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#database`, `#bug`, `#tailscale`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Grok 4.6 Scores 61 on Artificial Analysis Intelligence Index](https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis) ⭐️ 8.0/10

Grok 4.6 has been released, achieving a score of 61 on the Artificial Analysis Intelligence Index, which aggregates nine benchmarks. This places it on par with GPT-5.6 Sol, marking a frontier-level performance in agentic coding and knowledge work tasks. The model builds on Grok 4.5 with enhanced capabilities for long-horizon agentic tasks, complex interactions, and visual work, including handling large codebases and transforming product ideas into complete applications. However, community reports indicate that cache read pricing has nearly doubled from $0.30 in Grok 4.5 to $0.50 in Grok 4.6, which could significantly impact heavy coding session costs.

hackernews · wertyk · Aug 12, 16:54 · [Discussion](https://news.ycombinator.com/item?id=49275385)

**「Background」** The Artificial Analysis Intelligence Index is a composite score derived from nine separate benchmarks, designed to measure the overall intelligence of AI models. Grok 4.6, released by SpaceXAI \(formerly xAI\) on August 12, 2026, scored 61 on this index, tying with GPT-5.6 Sol and surpassing its predecessor Grok 4.5, which scored 56. The model is priced at $2 per million input tokens and $6 per million output tokens, and is positioned for long-running agentic tasks and knowledge work.

**「Impact」** For developers and organizations using Grok for coding and agentic workflows, the performance gains may be offset by increased cache read costs, potentially raising token bills substantially in heavy sessions. The pricing change could influence decisions between Grok and competing frontier models like GPT-5.6 Sol, especially for cost-sensitive users.

**「Community Discussion」** Community members praise Grok&\#x27;s communication style and speed, with some preferring it over Claude for personal coding due to its concise responses and interactive sessions. Others highlight that Cursor&\#x27;s subscription offers better value with Grok 4.5, and note that SpaceXAI&\#x27;s vertical integration may lead to cheaper tokens and better tools. However, concerns about the near-doubling of cache read pricing are raised, as cache reads and writes dominate token bills in heavy coding sessions.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis">Grok 4.6 returns SpaceXAI to the intelligence frontier and ...</a></li>
<li><a href="https://aireleasetracker.com/model/xai/grok-4.6">Grok 4.6 — Benchmarks, Specs &amp; Release Date</a></li>
<li><a href="https://officechai.com/ai/grok-4-6-benchmarks/">SpaceXAI Releases Grok 4.6, Benchmarks Show Performance ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#benchmarks`, `#Grok`, `#pricing`

---

<a id="item-tech-news-5"></a>
### [Signal Introduces Automatic Key Verification](https://signal.org/blog/automatic-key-verification/) ⭐️ 8.0/10

Signal has announced a new feature called Automatic Key Verification, designed to simplify and strengthen the security of end-to-end encrypted communications. The feature automates the process of verifying encryption keys, reducing the need for manual safety number checks while maintaining the integrity of the encryption. This change addresses a core usability issue in end-to-end encryption, making it easier for users to trust that their conversations are secure. The feature is part of Signal&\#x27;s ongoing efforts to enhance privacy and security for its users.

rss · Lobsters · Aug 12, 07:10

**「Background」** Signal&\#x27;s Automatic Key Verification is based on key transparency, a mechanism that helps ensure that Signal devices agree on which encryption keys belong to which phone numbers. This feature builds on Signal&\#x27;s existing safety number verification, which requires users to manually compare numbers to confirm the authenticity of their connections. The new automatic verification, combined with ongoing checks by the Signal connection and third-party auditors, aims to ensure the consistency of a connection&\#x27;s key across the Signal ecosystem.

**「Impact」** Signal users will benefit from a more streamlined and secure messaging experience, as automatic key verification reduces the risk of man-in-the-middle attacks without requiring manual verification steps. This could increase user trust in the platform and encourage broader adoption of secure communication practices.

<details><summary>References</summary>
<ul>
<li><a href="https://support.signal.org/hc/en-us/articles/10223569377562-Automatic-Key-Verification">Automatic Key Verification – Signal Support</a></li>
<li><a href="https://signal.org/blog/automatic-key-verification/">Signal &gt;&gt; Blog &gt;&gt; Introducing Automatic Key Verification</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#messaging`, `#encryption`, `#signal`

---

<a id="item-tech-news-6"></a>
### [Fudan Team First Creates Single-Layer CuO2 High-Temp Superconductor](https://www.ithome.com/0/989/009.htm) ⭐️ 8.0/10

A Fudan University team led by Professor Zhang Yuanbo has successfully fabricated a high-temperature superconductor with a single CuO2 plane, confirming the two-dimensional nature of high-temperature superconductivity. The work, published in Nature on August 12, 2026, also revealed an anomalous metallic state and quantum critical phenomena at the superconductor-insulator transition. By precisely controlling ozone concentration and temperature, the team achieved a doping resolution of δp≈0.0005, enabling observation of the full phase diagram from Mott insulator to the entire superconducting dome. This provides a highly tunable, high-quality 2D experimental platform for studying quantum critical phenomena and the mechanism of high-temperature superconductivity.

rss · IT HOME · Aug 12, 23:13

**「Background」** High-temperature superconductors, discovered in 1986, exhibit zero resistance and perfect diamagnetism below a critical temperature, with applications in power transmission, medical imaging, maglev trains, and quantum computing. However, their microscopic mechanism remains unresolved after nearly four decades. Copper oxide superconductors are known to have layered structures, and it has been hypothesized that their superconductivity is a strong two-dimensional phenomenon, but previous experiments were limited to double-layer or thicker samples.

**「Impact」** This breakthrough provides the first experimental evidence that high-temperature superconductivity in copper oxides is a strong two-dimensional phenomenon, offering a new platform for researchers to systematically study the evolution of superconductivity from onset to optimal doping. It may accelerate the understanding of high-temperature superconductivity mechanisms and guide the development of new high-temperature superconductors and 2D quantum materials.

**Tags**: `#high-temperature superconductivity`, `#2D materials`, `#quantum materials`, `#Nature publication`, `#condensed matter physics`

---

<a id="item-tech-news-7"></a>
### [China&\#x27;s Breakthrough in Lepidolite Lithium Extraction](https://www.ithome.com/0/988/980.htm) ⭐️ 8.0/10

China has achieved a major breakthrough in extracting lithium from lepidolite, overcoming long-standing technical challenges such as equipment corrosion, rotary kiln ring formation, and low recovery rates. The project, led by Changsha Nonferrous Metallurgy Design and Research Institute under Chinalco International, developed an innovative molten salt displacement roasting technology that has been successfully industrialized. This technology significantly improves lithium recovery and enables comprehensive recycling of potassium, rubidium, and other valuable metals, while also enhancing product purity and environmental sustainability. The technology is now in stable industrial operation at multiple projects in Jiangxi, including Yongxing Special Steel, Lingneng Lithium, Fengxin New Era, Yichun Longpan Times, and Jinfeng Lithium. The breakthrough addresses the complexity of lepidolite ore, which has low lithium grade and contains impurities like fluorine, making it a critical advancement for China&\#x27;s domestic lithium supply chain.

rss · IT HOME · Aug 12, 13:51

**「Background」** Lepidolite is a lithium-bearing mineral found mainly in granite pegmatites and is one of China&\#x27;s primary domestic sources of lithium. However, its complex composition, low lithium grade, and impurities such as fluorine make extraction difficult, historically causing equipment corrosion, kiln ring formation, and low recovery rates. The new molten salt displacement roasting technology, developed by Changsha Nonferrous Metallurgy Design and Research Institute under Chinalco International, addresses these challenges and has been industrialized in several projects in Jiangxi province.

**「Impact」** This breakthrough directly benefits Chinese lithium producers and the broader battery supply chain by enabling more efficient and cost-effective extraction from domestic lepidolite resources, reducing reliance on imported lithium. The technology&\#x27;s industrial application in Jiangxi projects demonstrates its practical viability, potentially lowering production costs and increasing output for battery-grade lithium compounds.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stdaily.com/web/gdxw/2026-08/12/content_562563.html">锂 云 母 提 锂 多项 技 术 难题攻克</a></li>
<li><a href="http://www.ce.cn/xwzx/gnsz/gdxw/202608/t20260812_3142630.shtml">锂 云 母 提 锂 多项 技 术 难题攻克_ 中 国 经济网—— 国 家经济门户</a></li>
<li><a href="https://www.donews.com/news/detail/8/6668879.html">锂 云 母 高 效 提 锂 技 术 实现工业化应用- DoNews快讯</a></li>

</ul>
</details>

**Tags**: `#lithium extraction`, `#industrial technology`, `#battery materials`, `#China`, `#metallurgy`

---

<a id="item-tech-news-8"></a>
### [Honor Robot Phone Pre-orders Exceed 400,000](https://www.ithome.com/0/988/965.htm) ⭐️ 8.0/10

At its global launch event on August 12, Honor unveiled the world&\#x27;s first robot phone, the Honor Robot Phone, with a starting price of 9,999 yuan. Honor&\#x27;s chief imaging engineer Luo Wei revealed that pre-orders have surpassed 400,000 units, warning that availability may be limited. The device is the first product from Honor&\#x27;s collaboration with ARRI, featuring a 200MP 4D gimbal main camera with F1.6 aperture, a 50MP ultrawide lens, and a 200MP periscope telephoto lens, powered by the in-house YOYO on-device AI model. It is equipped with the Snapdragon 8 Gen 5 chip and a 6.31-inch 1.5K display, with configurations of 12GB+512GB at 9,999 yuan and 16GB+1TB at 12,999 yuan.

rss · IT HOME · Aug 12, 13:04

**「Background」** Honor&\#x27;s Robot Phone is the world&\#x27;s first smartphone to integrate embodied intelligence, combining motion and spatial awareness with traditional mobile features. It was previewed at MWC 2026 as part of Honor&\#x27;s Augmented Human Intelligence \(AHI\) vision and ALPHA PLAN, and is the first product from a strategic technical collaboration with ARRI, the professional cinema camera manufacturer, to bring cinematic imaging principles to mobile devices.

**「Impact」** The Honor Robot Phone&\#x27;s strong pre-order numbers signal significant consumer interest in a new product category, potentially influencing competitors to explore similar AI-driven robotic features. However, the long-term impact depends on actual availability and user satisfaction, which remain unverified.

<details><summary>References</summary>
<ul>
<li><a href="https://www.honor.com/global/news/honor-mwc2026-launch/">HONOR Advances Its AI Vision at MWC 2026 with Robot Phone, Humanoid Robot and Magic V6 - HONOR Global</a></li>
<li><a href="https://www.arri.com/en/company/press/press-releases-2026/honor-and-arri-announce-strategic-technical-collaboration">HONOR and ARRI announce strategic technical collaboration to bring ARRI Image Science into next-generation consumer devices</a></li>

</ul>
</details>

**Tags**: `#Honor`, `#Robot Phone`, `#mobile`, `#hardware`, `#product launch`

---

<a id="item-tech-news-9"></a>
### [LTX-2.5: Open-Source Video Model Runs on RTX 5090](https://ltx.io/model/ltx-2-5) ⭐️ 8.0/10

LTX has released LTX-2.5, an open-source video generation foundation model, with weights, training code, and inference pipeline fully available. It can run locally on a single RTX 5090 and is free for commercial use if annual revenue is below $10 million. The model supports text-to-video and image-to-video generation, with improvements in multi-shot coherence and prompt adherence, and uses a new diffusion video decoder and a Gemma 4 12B text encoder. In an evaluation of 98 prompts for text-to-video artifacts, LTX 2.5 Pro ranked first among ten models.

telegram · zaihuapd · Aug 12, 02:15

**「Background」** LTX-2.5 is an open-source video generation foundation model built on a diffusion transformer architecture, released by LTX with open weights, training code, and inference pipeline. It supports text-to-video and image-to-video generation, and can run locally on a single RTX 5090 GPU. The model is free for commercial use for companies with annual revenue under $10 million, with API pricing starting at $0.09 per second for 720p video. This release follows LTX&\#x27;s pattern of offering open-source models for production, research, and experimentation, with the latest version introducing a new diffusion video decoder and Gemma 4 12B text encoder for improved multi-shot coherence and prompt adherence.

**「Impact」** This release enables researchers and developers to run a high-performing video generation model locally on consumer hardware, with commercial use allowed for smaller companies, potentially accelerating innovation in video AI applications.

<details><summary>References</summary>
<ul>
<li><a href="https://ltx.io/model/open-source">LTX-2.5 Model Open Source: AI Video Generator</a></li>
<li><a href="https://ltx.io/model/ltx-2-5">LTX-2.5: LTX&#x27;s Latest AI Open-Source Foundation Model | LTX</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#open-source`, `#AI model`, `#LTX-2.5`, `#local inference`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Why Tiny JPEGs Look Different in Chrome](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

hackernews · Lobsters · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**「Background」** When displaying small images, Chrome and Firefox often produce visibly different results, puzzling developers. The author explains that Chrome&\#x27;s JPEG downscaling optimization, which uses DCT-based scaling during decompression, is the culprit, causing tiny JPEGs to appear blurrier or otherwise altered compared to other browsers.

**「Solution」** The article details how Chrome&\#x27;s DCT-based scaling works: instead of fully decoding the JPEG and then scaling, it leverages the discrete cosine transform coefficients to approximate a smaller image, saving memory and CPU. This optimization, while efficient, introduces differences in appearance, especially for small images like icons. The author provides code and measurements to illustrate the effect and suggests practical mitigations: use appropriate image formats \(e.g., PNG for icons\) and ensure images are at the correct resolution for their display size. Community comments reinforce these points, noting similar issues with PNGs and the availability of the CSS \`image-rendering\` property to control scaling behavior.

**「Takeaway」** The author&\#x27;s core thesis is that browser-specific optimizations like DCT-based scaling can cause unexpected visual differences, so developers should choose image formats and resolutions suited to their use case rather than relying on browser defaults.

**Tags**: `#JPEG`, `#browser rendering`, `#image scaling`, `#Chrome`, `#web performance`

---