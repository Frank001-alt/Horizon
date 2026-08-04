---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 39 items, 18 important content pieces were selected

---

**Technology News**
1. [Qwen 3.8-Max Released: 2.4T Parameters, First Open-Sourced Max-Level Model](#item-tech-news-1) ⭐️ 9.0/10
2. [OpenAI highlights ten AI-driven advances in mathematics and theoretical computer science](#item-tech-news-2) ⭐️ 8.0/10
3. [ComfyUI Adds Day-0 Support for Open-Weight MiniMax H3, 2K Video and Audio](#item-tech-news-3) ⭐️ 8.0/10
4. [DNA device flaw could let hackers alter 30 years of U.S. forensic evidence](#item-tech-news-4) ⭐️ 8.0/10
5. [Nvidia CMP 170HX Mining Card Hack Unlocks 80GB VRAM, Prices Soar](#item-tech-news-5) ⭐️ 8.0/10
6. [Apple Sues UK Over iCloud Backdoor Order](#item-tech-news-6) ⭐️ 8.0/10
7. [LLMs reward expertise, not just democratize skill](#item-tech-news-7) ⭐️ 7.0/10
8. [Andy Pavlo joins ClickHouse to launch ClickHouse Labs](#item-tech-news-8) ⭐️ 7.0/10
9. [Bonsai: OCaml UI library from Jane Street sparks ecosystem debate](#item-tech-news-9) ⭐️ 7.0/10
10. [Kimi K3 Architecture Deep Dive](#item-tech-news-10) ⭐️ 7.0/10
11. [Desk reject papers without reproducible code, says ML reviewer](#item-tech-news-11) ⭐️ 7.0/10
12. [ARPL Auto-Configures llama.cpp for ARM Chips at Runtime](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [California diesel prices jump since Iran war began, raising risk of higher U.S. goods costs](#item-finance-news-1) ⭐️ 8.0/10
2. [Visa to Buy BioCatch for $2.4 Billion to Strengthen Fraud Detection](#item-finance-news-2) ⭐️ 8.0/10
3. [Japan and US reportedly intervene jointly to stem yen&\#x27;s slide to 40-year low](#item-finance-news-3) ⭐️ 8.0/10
4. [China’s domestic tourism downturn deepens while inbound luxury travel grows](#item-finance-news-4) ⭐️ 7.0/10
5. [CXMT Seeks Funding for Second Beijing Chip Fab, Reuters Says](#item-finance-news-5) ⭐️ 7.0/10
6. [Samsung shrinks China phone stores with monthly sales threshold](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen 3.8-Max Released: 2.4T Parameters, First Open-Sourced Max-Level Model](https://qwen.ai/blog?id=qwen3.8) ⭐️ 9.0/10

The Qwen team today officially released Qwen 3.8-Max, a 2.4-trillion-parameter model with 95 billion active parameters, making it the strongest model in the Qwen family. The model weights are scheduled to be open-sourced next week, marking the first time Qwen has opened weights for a Max-level model. Built on the Qwen 3.5 architecture, it delivers broad improvements in coding, work, research, and long-horizon tasks. In coding tests, the model can autonomously run for over 10 days to complete project construction and self-evolution, and within 24 hours it entered the WWW2025 multimodal dialogue intent recognition competition, outperforming 458 of 526 teams. Qwen 3.8-Max is now available via the QwenCloud API.

telegram · zaihuapd · Aug 3, 02:31

**「Background」** Qwen is Alibaba&\#x27;s family of large language models, usually divided into tiers that range from smaller open models to a Max tier reserved for the largest capabilities. Previously, Max-level Qwen models were only accessible through the QwenCloud API, so this release is notable because it is the first time Qwen will open-source the weights of a Max-level model.

**「Impact」** Developers and researchers will soon be able to download and self-host a 2.4-trillion-parameter open-weight model instead of relying solely on Qwen&\#x27;s API, though running a model of this scale will require enormous computational resources.

**Tags**: `#Qwen`, `#AI model`, `#open source`, `#large language model`, `#tech news`

---

<a id="item-tech-news-2"></a>
### [OpenAI highlights ten AI-driven advances in mathematics and theoretical computer science](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI has published an item titled &\#x27;Ten advances in mathematics and theoretical computer science,&\#x27; describing recent AI-assisted results in formal reasoning and proof. The company presents the advances as evidence of accelerating progress in automated reasoning, including the ability to generate candidate proofs and check them computationally. The announcement is aimed at AI/ML researchers and the theoretical computer science community, where it has generated substantive discussion. Specific proof details, problem statements, and dates are not available in the provided source material, so their exact scope cannot be confirmed here.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**「Background」** OpenAI published a 249-page manuscript on August 1, 2026, describing ten new results in pure mathematics and theoretical computer science, each accompanied by a machine-checkable certificate in the Lean 4 proof assistant. This follows a broader trend of using AI models, including large language models, to help generate and verify formal proofs for open problems in areas such as geometry, cryptography, and complexity theory.

**「Community Discussion」** Commenters largely agree that AI&\#x27;s progress in mathematics is following an exponential curve rather than a linear timeline, and that the technology can now generate and check candidate proofs at scale. Some note that intuition and conjecture formation remain human domains, while others point to specific examples like high-dimensional sphere packing and multicolor Ramsey numbers as illustrations, and one commenter quotes Douglas Adams&\#x27;s philosophers to suggest mathematicians should worry about being replaced.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer science</a></li>
<li><a href="https://beyondtmrw.org/article/ten-advances-in-mathematics-and-theoretical-computer-science">Ten advances in mathematics and theoretical computer science</a></li>

</ul>
</details>

**Tags**: `#AI research`, `#mathematics`, `#theoretical computer science`, `#automated reasoning`, `#OpenAI`

---

<a id="item-tech-news-3"></a>
### [ComfyUI Adds Day-0 Support for Open-Weight MiniMax H3, 2K Video and Audio](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

ComfyUI has announced day-0 support for MiniMax H3, an open-weights model capable of native audio and 2K video generation. The integration lets users run the model locally, and the project claims pruning roughly 40% of parameters into a lookup table cuts total memory from 123.6 GB in full precision to 42.5 GB with the smallest variants, a 66% reduction; combined with dynamic VRAM offloading, this can run on a GPU such as an RTX 3060. Early community tests show strong output quality, though one user reported about 10 minutes to generate a 10-second 480p clip on a 4070 Ti Super with 16 GB VRAM. The announcement generated substantial practitioner interest because it advances accessible local text/video generation.

hackernews · vblanco · Aug 3, 13:34 · [Discussion](https://news.ycombinator.com/item?id=49155629)

**「Background」** ComfyUI is a popular node-based interface for running AI image and video generation models locally. MiniMax H3, released by MiniMaxAI with open weights under the MiniMax H3 Community License, is a next-generation multimodal video model that accepts text, images, video, or audio and generates video with native stereo sound at resolutions up to 2K and clips up to 15 seconds. Day-0 support in ComfyUI means the model is available immediately in the ComfyUI ecosystem via the Comfy-Org Hugging Face repository, allowing users to run it locally from the day of release.

**「Impact」** Affected users can now run at least the lower-memory MiniMax H3 variants locally through ComfyUI on a GPU such as an RTX 3060, but typical user hardware still yields lengthy generation times \(about 10 minutes for a 10-second 480p clip on a 4070 Ti Super\).

**「Community Discussion」** Commenters were broadly impressed by the results and speed, but they cautioned that non-standard prompts still produce janky outputs and questioned whether the claimed &\#x27;no loss&\#x27; pruning approach would transfer to LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui">MiniMax H 3 Day - 0 Support in ComfyUI : Open Weights , Native Audio...</a></li>
<li><a href="https://huggingface.co/Comfy-Org/MiniMax-H3">Comfy -Org/ MiniMax - H 3 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#video generation`, `#ComfyUI`, `#MiniMax H3`, `#open weights`, `#AI models`

---

<a id="item-tech-news-4"></a>
### [DNA device flaw could let hackers alter 30 years of U.S. forensic evidence](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

Researchers found a security flaw in DNA analysis devices used by most U.S. crime laboratories, potentially allowing undetected tampering with roughly 30 years of forensic DNA files dating back to 1995. Using AI-generated code from Anthropic&\#x27;s Claude, they modified DNA scan data without leaving traces; the first tampering took about 45 minutes and altered files did not trigger alerts from common analysis software. Manufacturer Thermo Fisher Scientific privately acknowledged the vulnerability in July and published a high-severity advisory last Friday, warning that files could face &quot;almost undetectable modification&quot; if lab controls are bypassed, and released a software update adding digital signatures. The company says it is working with the U.S. Cybersecurity and Infrastructure Security Agency and no exploit has been observed. Researchers said more than 200 U.S. labs lack unified oversight and security varies, and it remains unclear whether pending or closed cases are affected.

telegram · zaihuapd · Aug 3, 05:15

**「Background」** DNA analysis instruments in forensic labs convert biological samples into digital profiles and data files that prosecutors rely on in criminal cases. Because these systems usually trust the integrity of files they process, a vulnerability that allows altered data to go unnoticed undermines the evidentiary chain of custody. The patch introduces digital signatures so labs can verify that files have not been changed.

**「Impact」** The advisory and update shift responsibility to the more than 200 U.S. crime labs using these instruments to apply the patch and assess exposure, though no exploitation has been reported and whether pending or closed cases are affected remains unclear.

**Tags**: `#cybersecurity`, `#forensics`, `#DNA analysis`, `#AI`, `#Thermo Fisher`

---

<a id="item-tech-news-5"></a>
### [Nvidia CMP 170HX Mining Card Hack Unlocks 80GB VRAM, Prices Soar](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

Researchers at Arizona State University disclosed a bypass for Nvidia&\#x27;s CMP 170HX mining card that uses a stack overflow in the GPU security coprocessor to defeat the official OTP fuse locks, unlocking up to 80 GB of VRAM and boosting FP32 compute from 0.39 TFLOPS to 94 TFLOPS. The card, released in 2021 with the same GA100 core as the A100, was originally crippled by hardware limits on compute, memory, and PCIe. After the exploit became public, secondary market prices in China jumped from 300–500 yuan to 3,000–4,000 yuan, with overseas listings reaching $1,500. Community members have verified the unlocked cards can run AI image generation and large language model inference on both Windows and Linux, though long-term stability and the maximum unlock per card batch remain uncertain.

telegram · zaihuapd · Aug 3, 11:29

**「Background」** The CMP 170HX was Nvidia&\#x27;s dedicated cryptocurrency mining card built on the GA100 die used in the A100, but it was intentionally restricted through one-time programmable fuses that limited memory capacity, compute performance, and PCIe bandwidth. These restrictions were managed by the Falcon security coprocessor, making the card effectively a crippled version of a high-end data center GPU. The disclosed vulnerability exploits an unbounded DMA overflow in that coprocessor to hijack control and modify the previously irreversible hardware locks.

**「Impact」** The exploit has created a supply of cheap, high-VRAM GPUs for AI inference workloads, but it has also driven used-card prices up roughly tenfold in China and to $1,500 overseas, shrinking the affordability window and introducing resale and long-term reliability risks for buyers.

**Tags**: `#hardware`, `#security`, `#Nvidia`, `#GPU`, `#AI`

---

<a id="item-tech-news-6"></a>
### [Apple Sues UK Over iCloud Backdoor Order](https://www.ft.com/content/2cc9c96a-0e5b-4c33-a95a-3d11072a145c?syn-25a6b1a6=1) ⭐️ 8.0/10

Apple has filed a legal challenge with the UK Investigatory Powers Tribunal against a Technical Capability Notice requiring a backdoor into encrypted iCloud backups for UK users, contesting the government&\#x27;s authority to issue the order. Apple has long argued that any backdoor reduces security for all users; due to legal restrictions, both Apple and the UK Home Office declined to comment. The move continues a protracted encryption dispute: the UK withdrew an earlier notice covering US users after a clash with Washington, then issued a new UK-only notice, prompting Apple to remove iCloud Advanced Data Protection in the UK in February 2025. Privacy groups Privacy International and Liberty have also challenged the notice, and the tribunal has scheduled a case-management hearing for next month.

telegram · zaihuapd · Aug 3, 15:40

**「Background」** The Technical Capability Notice is a UK legal instrument under the Investigatory Powers Act that can compel technology companies to weaken or bypass encryption. Apple&\#x27;s iCloud Advanced Data Protection offers end-to-end encryption for backups and other data, meaning Apple retains no decryption keys; a backdoor would force Apple to provide access to encrypted user content to UK authorities.

**「Impact」** UK iCloud users have lost access to end-to-end encrypted Advanced Data Protection since February 2025, and the legal outcome will help determine whether UK authorities can compel backdoors into encrypted cloud services.

**Tags**: `#Apple`, `#encryption`, `#government surveillance`, `#iCloud`, `#security`

---

<a id="item-tech-news-7"></a>
### [LLMs reward expertise, not just democratize skill](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 7.0/10

In the essay &\#x27;LLMs reward expertise&\#x27; at seangoedecke.com, Sean Goedecke argues that large language models amplify existing knowledge and skill rather than leveling the playing field for novices. The piece contends that deep domain knowledge, codebase familiarity, and the ability to craft precise prompts let experts extract far more value from LLMs, while novices often lack the context to evaluate or direct the output. The essay has drawn substantive Hacker News discussion, with commenters broadly agreeing that LLMs act as an &\#x27;amplifying mirror&\#x27; of the user&\#x27;s capabilities and that explicitly signaling expertise in prompts improves results. Others caution that the effect needs formal study and may reflect confirmation bias.

hackernews · MaxMussio · Aug 3, 21:13 · [Discussion](https://news.ycombinator.com/item?id=49161518)

**「Background」** In his July 24, 2026 essay, software engineer Sean Goedecke argues that LLMs reward expertise: while they let almost anyone produce passable generalist output, such as “sort-of-okay CSS,” getting high-quality results still depends on deep familiarity with the codebase or domain in question. The essay, which sparked a Hacker News discussion with 266 points and 113 comments, contends that LLMs amplify existing expertise rather than making specialized knowledge unnecessary, because effective prompting and evaluation require knowing what to ask and how to judge the answer.

**「Community Discussion」** Commenters largely endorse the essay&\#x27;s thesis, describing LLMs as a reflection of the user&\#x27;s prompt quality and world knowledge, with one noting that explicit expertise signaling \(&\#x27;I have significant background in biblical scholarship...&\#x27;\) changes outputs significantly. A counterpoint asks for formal study to avoid confirmation bias, observing that some coworkers get good results with very brief prompts, while another stresses that codebase familiarity remains a hands-on, hard-to-replace skill.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seangoedecke.com/llms-reward-expertise/">LLMs reward expertise - seangoedecke.com</a></li>
<li><a href="https://www.aib.vote/en/news/llms-reward-domain-expertise">LLMs Reward Domain Expertise | AIB</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#software engineering`, `#expertise`, `#AI`, `#productivity`

---

<a id="item-tech-news-8"></a>
### [Andy Pavlo joins ClickHouse to launch ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 7.0/10

Andy Pavlo has joined ClickHouse to establish ClickHouse Labs, a new research lab representing closer ties between academic database research and the commercial OLAP community. ClickHouse, known for real-time analytics database software, is the organizing company behind the lab. The move is notable because Pavlo is a prominent database researcher and educator, widely followed through his CMU database lecture series. The announcement was met with community interest in potential research directions and continued academic engagement.

hackernews · nikolay\_sivko · Aug 3, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49156011)

**「Background」** ClickHouse is an open-source columnar OLAP database widely used for high-performance analytics. Andy Pavlo is one of the database industry&\#x27;s most prominent researchers, known for his academic work and widely followed teaching. By joining ClickHouse to lead a new research group, ClickHouse Labs, Pavlo will bridge academic database research with the commercial OLAP community.

**「Community Discussion」** Commenters generally welcomed the news, with one noting they had watched Pavlo&\#x27;s CMU lecture series while studying and another hoping the lectures continue in a ClickHouse-sponsored format. Several comments also raised broader questions about the future of OLAP systems, including whether fast engines like ClickHouse and StarRocks will converge with Trino on decoupled compute/storage using S3-like storage, and what that means for ingestion and indexing.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/blog/andy-pavlo-joins-clickhouse">Andy Pavlo joins ClickHouse to establish ClickHouse Labs</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/clickhouse-launches-clickhouse-labs-andy-133000640.html?fr=sycsrp_catchall">ClickHouse Launches ClickHouse Labs With Andy Pavlo as VP of ...</a></li>
<li><a href="https://www.linkedin.com/posts/clickhouseinc_andy-pavlo-joins-clickhouse-to-establish-activity-7490039183105937409-PIGE">Andy Pavlo joins ClickHouse to establish ClickHouse Labs ...</a></li>

</ul>
</details>

**Tags**: `#ClickHouse`, `#database research`, `#OLAP`, `#Andy Pavlo`, `#systems engineering`

---

<a id="item-tech-news-9"></a>
### [Bonsai: OCaml UI library from Jane Street sparks ecosystem debate](https://github.com/janestreet/bonsai) ⭐️ 7.0/10

Jane Street has released Bonsai, an OCaml UI library on GitHub that allows developers to build web interfaces in OCaml and share types between frontend and backend. The project has attracted substantial Hacker News discussion, focusing on production readiness, how it compares with the OCaml-to-JavaScript compiler Melange, and whether it sacrifices access to the broader JavaScript ecosystem. Jane Street&\#x27;s Signals and Threads podcast has also covered the framework in an episode titled &\#x27;Building a UI Framework.&\#x27; While no external production adopters are cited in the discussion, the library highlights Jane Street&\#x27;s push to use a single functional language across the entire web stack.

hackernews · KolmogorovComp · Aug 3, 08:29 · [Discussion](https://news.ycombinator.com/item?id=49152842)

**「Background」** Bonsai is Jane Street&\#x27;s OCaml library for building reactive, performant web applications, partly inspired by Elm, and it powers nearly all of Jane Street&\#x27;s internal web tools. It uses an Incremental-style engine to re-render only when the UI model changes, and it compiles OCaml to JavaScript via Js\_of\_ocaml, which is what enables sharing types and code between frontend and backend. This background context helps explain the excitement about using one language across the stack, as well as the comparisons to alternatives like Melange that also target OCaml-to-JavaScript compilation.

**「Community discussion」** In Hacker News comments, users express enthusiasm for shared types between backend and frontend, but also raise practical concerns about production readiness in internal apps, comparisons with Melange, and whether adopting Bonsai means giving up the React, GraphQL, and broader JavaScript ecosystem. A separate commenter criticizes the visual design as &\#x27;extremely ugly&\#x27; while acknowledging likely performance, and others point to a Signals and Threads podcast episode for more depth.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/janestreet/bonsai">GitHub - janestreet/bonsai: A library for building dynamic ...</a></li>
<li><a href="https://ocaml.janestreet.com/ocaml-core/v0.13/doc/bonsai/Bonsai/index.html">Bonsai (bonsai.Bonsai) - ocaml.janestreet.com</a></li>
<li><a href="https://github.com/janestreet/bonsai_examples">GitHub - janestreet/bonsai_examples: Examples for bonsai_web ...</a></li>

</ul>
</details>

**Tags**: `#OCaml`, `#UI framework`, `#web development`, `#functional programming`, `#Jane Street`

---

<a id="item-tech-news-10"></a>
### [Kimi K3 Architecture Deep Dive](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 7.0/10

A SemiAnalysis newsletter article by Kimbo Chen analyzes Kimi K3, a novel AI model architecture, highlighting innovations in compressed memory, attention across depth, latent expert routing, and inference performance. The piece positions K3&\#x27;s design as a significant technical development in model architecture, though the available excerpt offers only an outline rather than full benchmarks or conclusions. The specific mechanisms described suggest potential improvements in memory efficiency and inference speed, but no independent performance data or deployment details are provided.

rss · Semianalysis · Aug 3, 19:42

**「Background」** Kimi K3 is Moonshot AI&\#x27;s most capable flagship model, a 2.8-trillion-parameter open model that is the first in the 3T-parameter class, with native vision capabilities and a 1-million-token context window. It is built on new architectural components called Kimi Delta Attention and Attention Residuals, which underpin the compressed memory, attention across depth, and latent expert routing discussed in the analysis. Released as an open model, it targets frontier performance in coding, knowledge work, and reasoning, and is positioned for long-horizon agentic use cases.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K 3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://lmstudio.ai/models/kimi-k3">Kimi K 3</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K 3 | OpenLM. ai</a></li>

</ul>
</details>

**Tags**: `#AI`, `#model architecture`, `#inference`, `#machine learning`, `#Kimi K3`

---

<a id="item-tech-news-11"></a>
### [Desk reject papers without reproducible code, says ML reviewer](https://www.reddit.com/r/MachineLearning/comments/1vei12v/its_time_to_desk_reject_papers_that_dont_include/) ⭐️ 7.0/10

A reviewer reports that across 12 papers reviewed for three major ML conferences during NeurIPS review season, only one included full code capable of running the entire pipeline from input dataset to output AUROC; four provided only partial code, and seven provided no code. Of the five papers with at least some code, three contained obvious bugs that, in the reviewer&\#x27;s assessment, completely invalidated their results. The author argues that current incentives discourage code release during review because sharing code only increases the chance of rejection when reviewers find bugs, and proposes imposing real penalties by desk-rejecting papers that do not include code to reproduce results. The post highlights a systemic reproducibility concern in ML research practice rather than a technical breakthrough.

reddit · r/MachineLearning · /u/Flaky-Ambition5900 · Aug 3, 16:17

**「Background」** Machine learning conferences such as NeurIPS currently treat code submission as strongly encouraged rather than mandatory. The NeurIPS submission checklist and Code of Ethics address reproducibility and research integrity, but authors face little enforcement for withholding code during peer review. This leaves reviewers unable to verify results, which underlies the proposal to desk-reject papers without complete code.

<details><summary>References</summary>
<ul>
<li><a href="https://neurips.cc/public/EthicsGuidelines">NeurIPS Code of Ethics</a></li>
<li><a href="https://github.com/dgonier/hexis-public/blob/main/paper/neurips_2026_guidelines.md">hexis-public/paper/neurips_2026_guidelines.md at main ...</a></li>

</ul>
</details>

**Tags**: `#reproducibility`, `#machine learning`, `#research practice`, `#conferences`, `#code`

---

<a id="item-tech-news-12"></a>
### [ARPL Auto-Configures llama.cpp for ARM Chips at Runtime](https://www.reddit.com/r/MachineLearning/comments/1ven68z/arpl_runtime_isatopology_detection_for_llamacpp/) ⭐️ 7.0/10

The ARPL library performs runtime ISA and topology detection for llama.cpp on ARM, auto-configuring inference settings based on the actual hardware instead of requiring per-device builds or manual tuning. It reads HWCAPs to see which ISA extensions \(SDOT, I8MM, SME2\) are available and how CPU cores are clustered, then recommends thread counts and patches context parameters such as flash attention and KV cache quantization. The initial public release includes an Android reference app written in Kotlin/Compose with a JNI bridge into llama.cpp, and the author says it was built and tested on a Samsung S25 Ultra \(SM-S938B\). Heterogeneous CPU/GPU/NPU partitioning is not included yet, and the project is published under the PolyForm Noncommercial license. The author reports that the ISA/thread/context handling already made a real difference in testing.

reddit · r/MachineLearning · /u/OpeningTough145 · Aug 3, 19:22

**「Background」** llama.cpp is an open-source C/C++ inference engine that runs large language models on CPUs, GPUs, and mobile devices, but it normally needs thread counts, context settings, and feature flags to be chosen generically or tuned per chip. ARM Application Processors expose differing optional ISA extensions and heterogeneous core clusters, so runtime detection can select optimal settings such as SDOT/I8MM/SME2 support and appropriate thread counts without rebuilding for each device.

**「Impact」** ARM device owners using llama.cpp can skip per-device builds and manual tuning, with ARPL automatically enabling supported ISA extensions and topology-aware thread counts, which the author says made a real difference on a Samsung S25 Ultra.

**Tags**: `#llama.cpp`, `#ARM`, `#runtime detection`, `#Android`, `#Snapdragon`

---

## Financial News

<a id="item-finance-news-1"></a>
### [California diesel prices jump since Iran war began, raising risk of higher U.S. goods costs](https://www.cnbc.com/2026/08/03/californias-diesel-prices-have-jumped-since-the-iran-war-started-with-ripple-effects-across-the-country.html) ⭐️ 8.0/10

California’s average diesel price has risen to $6.92 a gallon from $5.10 before the Iran war, according to AAA, while the U.S. average is $5.36; because trucks and trains moving goods through the San Pedro Bay port complex pay those California fuel prices, analysts warn higher transport costs could push up delivered costs of goods nationwide.

rss · CNBC Finance · Aug 3, 19:20

**「Background」** The war with Iran, now in its sixth month, has closed the Strait of Hormuz—a passage for over a fifth of global oil trade—and tightened refinery product markets, helping push California diesel prices up. California also has few major pipelines connecting it to other U.S. markets, so it relies on fuel shipped in from elsewhere, and its strict environmental rules add to costs.

**「Impact on U.S. households」** Because most goods shipped through California&\#x27;s ports are moved by trucks and trains, the higher diesel costs are likely to be passed on to households as more expensive everyday products nationwide.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_Iran_war_fuel_crisis">2026 Iran war fuel crisis - Wikipedia</a></li>
<li><a href="https://www.energy.ca.gov/sites/default/files/2026-06/DPMO_California_Gasoline_Diesel_Market_Update_June_2026_ada.pdf">California Gasoline and Diesel Market Update</a></li>
<li><a href="https://www.tiktok.com/discover/why-are-diesel-prices-higher-than-gas">Why Are Diesel Prices Higher Than Gas | TikTok</a></li>

</ul>
</details>

**Tags**: `#diesel prices`, `#Iran war`, `#supply chain`, `#California`, `#energy markets`

---

<a id="item-finance-news-2"></a>
### [Visa to Buy BioCatch for $2.4 Billion to Strengthen Fraud Detection](https://www.cnbc.com/2026/08/03/visa-buys-biocatch-fraud-detection.html) ⭐️ 8.0/10

Visa agreed to acquire fraud-detection startup BioCatch for $2.4 billion in cash, a deal expected to close by the end of Visa’s fiscal second quarter in 2027, subject to regulatory approvals.

rss · CNBC Finance · Aug 3, 16:44

**「Background」** BioCatch uses behavioral biometrics—analyzing signals like keystroke timing and touch-screen pressure—to distinguish real users from scammers and bots, and says it currently protects 760 million users across roughly 350 banks. Visa says scams and account takeovers cost the global economy more than $1 trillion annually.

**Tags**: `#M&amp;A`, `#cybersecurity`, `#payments`, `#fraud detection`, `#Visa`

---

<a id="item-finance-news-3"></a>
### [Japan and US reportedly intervene jointly to stem yen&\#x27;s slide to 40-year low](https://www.zaobao.com.sg/news/world/story20260802-9457369) ⭐️ 8.0/10

Japanese Finance Minister Katayama Satsuki is expected to announce on Aug 3 that Japan and the US intervened jointly in forex markets to stop the yen from falling to a near 40-year low; market sources say authorities bought yen repeatedly and US Treasury Secretary Bessent&\#x27;s meeting notes cited buying $5–10 billion worth of yen.

telegram · zaihuapd · Aug 3, 01:29

**「Background」** The yen had earlier approached 164 per dollar, its weakest since 1986.

**Tags**: `#forex intervention`, `#Japanese yen`, `#US Treasury`, `#monetary policy`, `#currency markets`

---

<a id="item-finance-news-4"></a>
### [China’s domestic tourism downturn deepens while inbound luxury travel grows](https://www.cnbc.com/2026/08/03/china-price-demand-tourism-hotel.html) ⭐️ 7.0/10

China’s domestic tourism is weakening faster than expected: hotel revenue per available room \(RevPAR\) fell 6% year on year through late July across the country, and Hilton now expects its China RevPAR to decline by low single digits this year after earlier forecasting flat performance. A partial bright spot is inbound luxury travel, with Hyatt’s Greater China RevPAR up 7.2% year on year in the second quarter.

rss · CNBC Finance · Aug 3, 10:32

**「Background」** China’s post-Covid tourism rebound is fading as consumer spending and retail sales stay sluggish, with Natixis pointing to a sharp decline in per-capita tourism spending since the third quarter of 2025. A visa-free entry policy for more countries is helping draw higher-income inbound visitors.

**「Impact」** The slump pressures mass-market hotels and businesses dependent on Chinese domestic travelers, while luxury hotels could benefit from visa-free inbound travel.

**Tags**: `#China tourism`, `#hotel industry`, `#consumer spending`, `#RevPAR`, `#economic slowdown`

---

<a id="item-finance-news-5"></a>
### [CXMT Seeks Funding for Second Beijing Chip Fab, Reuters Says](https://www.reuters.com/world/asia-pacific/cxmt-plans-second-chip-plant-beijing-is-talks-its-funding-sources-say-2026-08-03/) ⭐️ 7.0/10

CXMT, the world&\#x27;s fourth-largest DRAM maker, is in early-stage talks to build a second 12-inch chip fab in Beijing&\#x27;s Yizhuang area and is seeking at least 60 million yuan in support from the local development zone, according to Reuters. The potential expansion comes as AI infrastructure drives a global chip shortage.

telegram · zaihuapd · Aug 3, 09:38

**「Background」** CXMT currently operates three 12-inch DRAM fabs in Hefei and Beijing, each with monthly capacity of about 100,000 wafers; previously planned new fabs in Shanghai and Hefei could double that to more than 600,000 wafers a month, still far below the roughly 90% combined market share of Samsung, SK Hynix and Micron.

**Tags**: `#DRAM`, `#semiconductor`, `#chip manufacturing`, `#China`, `#capacity expansion`

---

<a id="item-finance-news-6"></a>
### [Samsung shrinks China phone stores with monthly sales threshold](https://finance.sina.com.cn/jjxw/2026-08-03/doc-inikzqsf4656080.shtml) ⭐️ 7.0/10

Samsung is shrinking its mobile phone store network in China after people familiar with the matter said it set an internal monthly sales threshold of 300,000 yuan and will gradually phase out stores and staff who repeatedly miss it. According to market-research firm IDC, Samsung&\#x27;s China smartphone market share was 0.1% in the second quarter of 2026, with shipments down 60.8% year on year, and its mobile experience \(MX\) business posted an operating loss of 0.7 trillion won—its first loss for the phone business.

telegram · zaihuapd · Aug 3, 10:52

**「Background」** The reported store-closure push has already touched Shenzhen, Fuzhou, Zhengzhou, Xi&\#x27;an, Kunming and Hefei, and comes after Samsung exited China&\#x27;s home appliance market in May. Samsung has not publicly responded to the store-shrinkage reports.

**Tags**: `#Samsung`, `#China smartphone market`, `#retail contraction`, `#IDC data`, `#operating loss`

---