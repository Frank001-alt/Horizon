---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 184 items, 10 important content pieces were selected

---

**Technology News**
1. [GLM-5.3: Frontier Coding with Emergent Cyber Capabilities](#item-tech-news-1) ⭐️ 9.0/10
2. [Chinese Doctor Uses GPT-5.6 to Prove 22-Year-Old Crouzeix Conjecture](#item-tech-news-2) ⭐️ 9.0/10
3. [Qwen 3.8 27B: Open-Source Model Impresses with Reasoning](#item-tech-news-3) ⭐️ 8.0/10
4. [Going Dark: The Shift to Law Enforcement Hacking](#item-tech-news-4) ⭐️ 8.0/10
5. [IPv8 Internet-Draft Implemented in Linux Kernel, Musl, and BGP](#item-tech-news-5) ⭐️ 8.0/10
6. [NVIDIA Begins Mass Production of Spectrum-X, World&\#x27;s First 200G/lane CPO Ethernet Switch](#item-tech-news-6) ⭐️ 8.0/10
7. [Doom Renderer Compiled into 21B-Parameter Transformer Without Training](#item-tech-news-7) ⭐️ 8.0/10
8. [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Parameters](#item-tech-news-8) ⭐️ 8.0/10
9. [Apple Trains China-Specific AI Model with Alibaba, Could Be First Foreign Firm Approved](#item-tech-news-9) ⭐️ 8.0/10

**Financial News**
1. [SpaceX Completes $60 Billion Acquisition of AI Coding Company Cursor](#item-finance-news-1) ⭐️ 9.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GLM-5.3: Frontier Coding with Emergent Cyber Capabilities](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.AI has announced GLM-5.3, a new AI model that introduces frontier coding with emergent cyber capabilities, enabling autonomous security research and vulnerability discovery, including zero-day exploitation. The model demonstrates advanced performance in red-team scenarios, such as exploiting vulnerabilities in WordPress plugins, achieving remote code execution, and adapting kernel exploits, while also playing defensive roles against other AI agents. Z.AI has also launched a coordinated vulnerability disclosure platform at cvd.z.ai, where they are scanning open-source and popular software at scale and disclosing found vulnerabilities, many under embargo and rated critical or high. Community reports indicate that GLM-5.3 is a significant improvement over its predecessor, GLM 5.2, with some users upgrading their subscriptions immediately, though it still trails leading models like Mythos 5 on certain benchmarks. The model&\#x27;s weights are expected to be released in about two weeks, and it is seen as a potential competitor to offerings from OpenAI and Anthropic.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**「Background」** GLM-5.3 is the latest iteration of Z.ai&\#x27;s open-weights large language model series, built on a 743B parameter base model with post-training focused on coding and agentic capabilities. It follows GLM-5.2 and is positioned as a frontier model for long-horizon coding tasks, achieving the highest score of any open-source model on Terminal Bench 3.0 and a 50% improvement over GLM-5.2 on Z.ai&\#x27;s internal coding agent benchmark. The model also exhibits emergent cybersecurity capabilities, including autonomous vulnerability discovery and exploitation, which Z.ai reports grew faster than anticipated during training scaling.

**「Impact」** GLM-5.3&\#x27;s emergent cyber capabilities could significantly lower the barrier to automated vulnerability discovery and exploitation, impacting cybersecurity professionals and software vendors who may face an increase in AI-driven attacks and a greater need for defensive AI. The coordinated disclosure platform may also accelerate the patching cycle for open-source projects, but the scale of scanning raises concerns about the potential for misuse before embargoes lift.

**「Community Discussion」** Community members report that GLM-5.3 performs exceptionally well in real-world security research, with one user noting it seamlessly executed a red-team scenario including zero-day exploits and kernel adaptation, while another highlighted the model&\#x27;s vulnerability scanning and disclosure efforts. Some users express cautious optimism, noting that while GLM-5.3 is impressive, it still trails leading models like Mythos 5 on certain benchmarks, and there are concerns about the economic viability of switching from OpenAI due to subscription costs and the model&\#x27;s reliance on post-training improvements.

<details><summary>References</summary>
<ul>
<li><a href="https://explainx.ai/blog/glm-5-3-launch-cyber-defense-benchmarks-august-2026">GLM-5.3 Launch: Benchmarks, Pricing &amp; Access (Aug 2026) | explainx.ai Blog | explainx.ai</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>
<li><a href="https://siliconangle.com/2026/08/14/z-ai-debuts-glm-5-3-long-horizon-coding-cybersecurity-upgrades/">Z.ai debuts GLM-5.3 with long-horizon coding, cybersecurity upgrades - SiliconANGLE</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#coding`, `#GLM`, `#vulnerability discovery`

---

<a id="item-tech-news-2"></a>
### [Chinese Doctor Uses GPT-5.6 to Prove 22-Year-Old Crouzeix Conjecture](https://www.ithome.com/0/989/952.htm) ⭐️ 9.0/10

A Chinese doctor, Jinshan Mu, a postdoctoral researcher at Peking Union Medical College Hospital, used OpenAI&\#x27;s GPT-5.6-Sol model to prove the Crouzeix conjecture, a mathematical problem posed in 2004 that had remained unsolved for 22 years. The proof was completed in about 16 hours of autonomous AI operation, and the manuscript has been reviewed and confirmed correct by the conjecture&\#x27;s author Michel Crouzeix, as well as mathematicians Alex Townsend and Anne Greenbaum. Mu, whose formal education is in geology and clinical medicine, employed a non-traditional approach using the AI model on the ChatGPT Work platform, with strategies inspired by OpenAI&\#x27;s earlier work on the Cycle Double Cover conjecture. The proof has been open-sourced on GitHub, including the paper, prompts, iteration drafts, Lean 4 formalization code, and audit reports. This breakthrough highlights the growing role of AI in mathematical research, following other recent AI-assisted advances in mathematics.

rss · IT HOME · Aug 14, 15:08

**「Background」** The Crouzeix conjecture, proposed by French mathematician Michel Crouzeix in 2004, states that for any matrix and any polynomial function, the norm of the matrix under the function is at most twice the maximum of the function on the matrix&\#x27;s numerical range. Despite its simple formulation, the conjecture resisted proof for over two decades; by 2007, Crouzeix himself had only proven the bound with a constant of 11.08, and in 2017, a week-long workshop of top experts reduced it to 2.414, with no further progress until now. The recent breakthrough involved a Chinese neurosurgeon, Jinshanmu, who used OpenAI&\#x27;s GPT-5.6-Sol model in a 16-hour autonomous session to produce a proof, which was subsequently verified by mathematicians Alex Townsend, Anne Greenbaum, and Crouzeix himself.

**「Impact」** This proof demonstrates that AI models can autonomously solve long-standing mathematical conjectures, potentially accelerating research in mathematics and related fields, and may encourage more researchers to adopt AI-assisted methods.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nationpress.com/sciencetech/surgeon-cracks-20-year-maths-problem-with-gpt">Beijing surgeon solves 20-year-old Crouzeix conjecture using ...</a></li>
<li><a href="https://github.com/jinshanmu/CrouzeixConjecture">GitHub - jinshanmu/CrouzeixConjecture: Research draft of a ...</a></li>
<li><a href="https://alextownsend.net/essays/SIAMNews_CrouzeixConjecture.pdf">The Neurosurgery Resident Who Proved Crouzeix’s Conjecture</a></li>

</ul>
</details>

**Tags**: `#AI-assisted proof`, `#Crouzeix conjecture`, `#GPT-5.6`, `#mathematics`, `#OpenAI`

---

<a id="item-tech-news-3"></a>
### [Qwen 3.8 27B: Open-Source Model Impresses with Reasoning](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B is a newly released open-source AI model that has garnered attention for its strong reasoning capabilities and high-quality output. Community members report that it successfully passed private benchmarks, with one user noting it took 5x more tokens and 12m30s with MTP enabled, but performed well. The model is praised for its explicit reasoning style, though it appears less VRAM-efficient than competitors like Gemma 4. The release contributes to the growing commoditization of frontier AI, with users noting the rise of capable models from non-US companies.

hackernews · erdaltoprak · Aug 14, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49299605)

**「Background」** Qwen is Alibaba&\#x27;s open-source large language model family. The Qwen3.8-27B is a 27-billion-parameter model released on August 14, 2026, with a 262k context window, following Alibaba&\#x27;s commitment to open-weight releases. It is part of the Qwen 3.8 generation, which also includes the larger Qwen3.8-Max, and is designed to run locally on consumer hardware, making frontier-level AI capabilities accessible to individual developers and researchers.

**「Impact」** For developers and researchers running local models, Qwen 3.8 27B offers a viable option for tasks requiring explicit reasoning, though its higher VRAM usage may be a constraint. The model&\#x27;s success signals increasing competition in the open-source AI space, potentially pressuring proprietary models from major US companies.

**「Community Discussion」** Community members are impressed by the model&\#x27;s reasoning, with one noting it is the second local model to pass a private benchmark, while others highlight its unique thinking trace pattern and potential MTP prediction issues. There is also discussion about the broader trend of commoditized AI intelligence from non-US companies.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@rosgluk/qwen-3-8-27b-is-coming-and-it-could-be-the-most-important-local-ai-release-of-2026-c1cf381d5292">Qwen 3.8 27B Is Coming - and It Could Be the Most Important Local AI Release of 2026 | by Rost Glukhov | Aug, 2026 | Medium</a></li>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://aireleasetracker.com/model/qwen/qwen3.8-27b">Qwen3.8-27B — Benchmarks, Specs &amp; Release Date</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Open Source`, `#Model Release`, `#LLM`, `#Benchmark`

---

<a id="item-tech-news-4"></a>
### [Going Dark: The Shift to Law Enforcement Hacking](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

The article &\#x27;Going Dark, and the era of law enforcement hacking&\#x27; analyzes the transition from traditional wiretapping to law enforcement hacking as encryption becomes more prevalent. It discusses the potential ceiling on the number of useful software bugs, which could limit hacking capabilities, and the impact of AI on software security. The piece is authored by a well-known cryptography blog and has sparked substantive debate in the technology community. The analysis highlights implications for software security, privacy, and the future of law enforcement surveillance.

hackernews · vslira · Aug 14, 20:52 · [Discussion](https://news.ycombinator.com/item?id=49304447)

**「Background」** The term &quot;Going Dark&quot; refers to the growing challenge law enforcement faces in accessing communications and data protected by strong encryption. In 2014, FBI Director James Comey launched a &quot;Going Dark&quot; initiative to spark a national conversation about how technology providers could help law enforcement access encrypted data while balancing public safety and privacy. This debate has intensified as end-to-end encryption becomes more widespread, leading to a shift toward law enforcement hacking as an alternative to legal interception.

**「Impact」** The shift to law enforcement hacking could significantly affect software security practices and privacy expectations, as vulnerabilities become valuable for surveillance and may be stockpiled rather than disclosed. This trend may also influence how developers approach security, potentially leading to more robust systems but also raising concerns about government access to private communications.

**「Community Discussion」** Commenters debate the article&\#x27;s claim about a ceiling on useful bugs, with some arguing that AI-generated code introduces more bugs, while others note the contrast between sophisticated hacking operations and basic security failures. Historical context is also provided, noting that wiretapping has existed since the telephone&\#x27;s invention, challenging the notion that this is a new era.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/">Everything is about to “go dark” – A Few Thoughts on ...</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#law-enforcement`, `#security`, `#privacy`, `#encryption`

---

<a id="item-tech-news-5"></a>
### [IPv8 Internet-Draft Implemented in Linux Kernel, Musl, and BGP](https://goonhost.rocks/blog/implementing-ipv8-internet-draft) ⭐️ 8.0/10

A team has implemented the IPv8 Internet-Draft in the Linux kernel, musl libc, and BGP, marking a substantial systems engineering effort. IPv8 is an experimental protocol proposal that aims to address limitations of IPv4 and IPv6, and this implementation demonstrates its feasibility in core networking components. The work involves deep integration with the kernel&\#x27;s networking stack, the musl C library for system calls, and BGP for routing, indicating a comprehensive approach. While IPv8 is still an Internet-Draft and not widely deployed, this implementation could influence future protocol adoption and testing. The project showcases significant technical skill and may serve as a reference for further development.

rss · Lobsters · Aug 14, 19:05

**「Background」** IPv8 is an Internet-Draft \(draft-thain-ipv8\) that proposes a managed network protocol suite intended to replace or augment the current Internet Protocol stack. It introduces 64-bit ASN-prefixed addresses, treats IPv4 as a proper subset, and includes a Zone Server that consolidates functions like DHCP, DNS, authentication, and egress control. Every manageable element in an IPv8 network is authorized via OAuth2 JWT tokens served from a local cache. The draft is still in early stages, with version -02 published in April 2026 and an expiration date of October 2026.

**「Impact」** This implementation provides a concrete, testable reference for IPv8, potentially accelerating its evaluation and adoption by researchers and network engineers. However, since IPv8 is not yet a standard, its practical impact remains limited until broader community and standards body engagement occurs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ietf.org/archive/id/draft-thain-ipv8-00.html">Internet Protocol Version 8 (IPv8) - ietf.org</a></li>
<li><a href="https://datatracker.ietf.org/doc/draft-thain-ipv8/">draft-thain-ipv8-02 - Internet Protocol Version 8 (IPv8)</a></li>
<li><a href="https://transitai.app/blog/ipv8-draft-zone-server-math/">IPv8: The Draft of a New Internet — Transit AI</a></li>

</ul>
</details>

**Tags**: `#IPv8`, `#Linux kernel`, `#networking`, `#BGP`, `#systems programming`

---

<a id="item-tech-news-6"></a>
### [NVIDIA Begins Mass Production of Spectrum-X, World&\#x27;s First 200G/lane CPO Ethernet Switch](https://www.ithome.com/0/989/970.htm) ⭐️ 8.0/10

NVIDIA announced on August 14 that it has begun full production of the Spectrum-X Ethernet photonic switch, claiming it is the world&\#x27;s first mass-produced 200G/lane co-packaged optics \(CPO\) Ethernet switch system. The switch integrates optical engines and switching ASICs in the same module, reducing power consumption to one-fifth of traditional pluggable optics, extending AI application uptime by 5x, and improving mean time between events by 10x. The SN6810 offers 128 800Gb/s ports in a 2U liquid-cooled chassis with 102.4Tb/s total switching capacity, while the larger SN6800 stacks four ASICs in a 5U system to deliver 409.6Tb/s with 512 800Gb/s ports or over 2,000 200Gb/s ports. Manufacturing partners include TSMC for silicon photonics, SPIL for packaging and testing, Lumentum and TFC for laser components, and Foxconn for system development, with NVIDIA performing final testing before shipment.

rss · IT HOME · Aug 14, 22:53

**「Background」** Co-packaged optics \(CPO\) is an emerging technology that integrates optical engines directly with switching ASICs on the same package, reducing the power and latency overhead of traditional pluggable optical modules. NVIDIA&\#x27;s Spectrum-X Ethernet Photonics switch is the first mass-produced 200G/lane CPO Ethernet switch, marking a significant step in bringing CPO to mainstream AI networking. According to industry analyst LightCounting, NVIDIA&\#x27;s CPO rollout was expected to begin with InfiniBand in the second half of 2025, with Ethernet CPO following in 2026, and that CPO would be optional alongside pluggable module offerings.

**「Impact」** This milestone could accelerate adoption of CPO technology in AI data centers, offering significant power and reliability improvements for large-scale AI training and inference clusters, potentially influencing future network infrastructure designs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lightcounting.com/research-note/march-2025-nvidias-cpo-is-the-first-step-in-a-long-journey-395">LightCounting :: March 2025 Nvidia &#x27;s CPO is the First Step in a Long...</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#CPO`, `#Ethernet switch`, `#AI infrastructure`, `#silicon photonics`

---

<a id="item-tech-news-7"></a>
### [Doom Renderer Compiled into 21B-Parameter Transformer Without Training](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

A developer has compiled Doom&\#x27;s rendering algorithm into a 21-billion-parameter transformer checkpoint using a custom compiler that converts computation graphs into transformer weights, requiring no training. The model, when prompted with scene data, generates a token sequence of pixel-drawing commands that can be mechanically applied to render a frame from the game&\#x27;s E1M1 level. The checkpoint is a standard Hugging Face transformers model loadable without trust\_remote\_code, and the host program to load it, generate, and parse the output is just 43 lines of Python. Generating one frame takes a 3,614-token prompt plus 53,747 generated tokens, running in just over 40 minutes on an NVIDIA B200 GPU, achieving roughly 35 frames per day compared to the original Doom&\#x27;s 35 FPS on a 486 processor. The project includes a write-up, weights, and source code on GitHub.

reddit · r/MachineLearning · /u/notforrob · Aug 14, 15:50

**「Background」** Transformers are typically trained on vast datasets to learn patterns, but this project instead compiles an algorithm directly into the model&\#x27;s weights, bypassing training entirely. Doom&\#x27;s renderer is a classic real-time 3D graphics algorithm that draws the game world by processing scene geometry and emitting pixel-level commands, making it a suitable candidate for such a compilation approach.

**「Impact」** This demonstration shows that complex algorithms can be embedded into transformer weights without training, potentially opening new avenues for model interpretability and program synthesis, though the practical performance is far too slow for real-time use.

**Tags**: `#transformer`, `#compilation`, `#Doom`, `#neural networks`, `#program synthesis`

---

<a id="item-tech-news-8"></a>
### [Xiaohongshu Open-Sources dots3-note: 280B MoE with 16B Active Parameters](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

Xiaohongshu&\#x27;s dots lab has open-sourced dots3-note preview, the first open-weight model in the dots3 series. The model has 280B total parameters with only 16B active per inference, supports a 512K context window, and handles text, images, video, and audio. It introduces TEMPO, a new reinforcement learning method that uses self-critique and test-time value estimation to train long-horizon agents. The weights are available on Hugging Face, and the release also includes two new real-world agent benchmarks: VibeSearchBench and VibeLifeBench.

telegram · zaihuapd · Aug 14, 08:27

**「Background」** Mixture-of-Experts \(MoE\) models activate only a subset of their total parameters per token, enabling large model capacity with lower inference cost. Xiaohongshu&\#x27;s Dots Lab has released dots3-note preview, the first open-weight model in the dots3 series, with 280B total parameters and 16B activated parameters, supporting up to 512K tokens of context and multimodal input \(text, images, video, audio\) with text output. The model introduces TEMPO, a reinforcement learning method that trains long-horizon agents via self-critique and test-time value estimation, and is accompanied by two new benchmarks: VibeSearchBench and VibeLifeBench.

**「Impact」** AI/ML practitioners and researchers can now access a large-scale MoE model with efficient activation \(280B total, 16B active\) and long context \(512K\) for multimodal tasks, along with new benchmarks for evaluating real-world agent performance, potentially accelerating research in efficient large models and reinforcement learning.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/dots3-note-prev: dots3 note preview</a></li>
<li><a href="https://eu.36kr.com/en/p/3938759517896072">Xiaohongshu Open-Sourced Dots3-Note: The Same-Series Model ...</a></li>
<li><a href="https://huggingface.co/dots-studio/dots3-note-prev">dots-studio/dots3-note-prev · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#MoE`, `#multimodal`, `#reinforcement-learning`, `#benchmarks`

---

<a id="item-tech-news-9"></a>
### [Apple Trains China-Specific AI Model with Alibaba, Could Be First Foreign Firm Approved](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

Apple has trained a large language model specifically for the Chinese market, with support from Alibaba, according to sources familiar with the matter. This marks a shift from its previous reliance on third-party models. The China-specific AI model is expected to power Apple Intelligence, which will launch in China in the coming months via an iOS update. The Cyberspace Administration of China has already filed the generative AI service for registration last month. If approved, Apple would become the first foreign company authorized by Beijing to offer its own AI model in China.

telegram · zaihuapd · Aug 14, 14:47

**「Background」** Apple has historically relied on local partners to provide AI features in China due to strict regulatory requirements for generative AI services. The Cyberspace Administration of China \(CAC\) requires companies to obtain approval before offering such services, and foreign firms have faced additional hurdles. By training a proprietary large language model with Alibaba&\#x27;s technical support, Apple aims to gain more control over its AI experience in China while navigating these regulations, potentially becoming the first foreign company approved to offer its own AI model in the country.

**「Impact」** This development could give Apple greater control over the AI experience for Chinese users and set a precedent for other foreign tech firms seeking to offer AI services in China, while also intensifying competition in the Chinese AI market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.remio.ai/post/alibaba-apple-ai-partnership-gives-apple-more-control-in-china">Alibaba Apple AI Partnership Gives Apple More Control in China</a></li>
<li><a href="https://clashreport.com/world/articles/apple-develops-china-specific-ai-model-in-partnership-with-alibaba-qfsiu4onya">Apple Develops China -Specific AI Model in Partnership With Alibaba</a></li>
<li><a href="https://aichief.com/news/apple-taps-alibaba-for-china-ai-model-training/">Apple Taps Alibaba for China AI Model Training</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Regulation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [SpaceX Completes $60 Billion Acquisition of AI Coding Company Cursor](https://www.ithome.com/0/989/944.htm) ⭐️ 9.0/10

SpaceX has completed its $60 billion acquisition of AI coding startup Cursor, one of the largest tech deals ever, effective August 14. The deal aims to boost SpaceX&\#x27;s AI capabilities, with Cursor gaining access to SpaceX&\#x27;s large GPU cluster.

rss · IT HOME · Aug 14, 14:34

**「Background」** SpaceX, the aerospace company led by Elon Musk, had announced an agreement to acquire Cursor two months before the deal closed. The acquisition is part of SpaceX&\#x27;s broader push into AI, which includes its AI division SpaceXAI and the development of models like Grok.

**「Impact」** The acquisition positions SpaceX to compete more directly with AI leaders like Anthropic and OpenAI in the profitable AI coding market, potentially affecting developers and the broader AI industry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/sandycarter/2026/06/16/spacex-buys-cursor-in-largest-startup-acquisition-ever-at-60-billion/">SpaceX Buys Cursor In Largest Startup Acquisition Ever At $60 ...</a></li>
<li><a href="https://www.cnbc.com/2026/06/16/spacex-spcx-cursor-acquisition-ipo.html">SpaceX to acquire the AI coding startup Cursor for $60 billion</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Cursor`, `#acquisition`, `#AI`, `#tech industry`

---