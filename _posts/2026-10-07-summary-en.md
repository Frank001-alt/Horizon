---
layout: default
title: "Horizon Summary: 2026-10-07 (EN)"
date: 2026-10-07
lang: en
---

> From 203 items, 10 important content pieces were selected

---

**Technology News**
1. [OpenAI Shares AI-Generated Solutions to Major Math Problems](#item-tech-news-1) ⭐️ 9.0/10
2. [Mistral Large 4 Trained on 3,800 GPUs in Europe](#item-tech-news-2) ⭐️ 8.0/10
3. [Google Releases EmbeddingGemma 2 Under Apache 2.0](#item-tech-news-3) ⭐️ 8.0/10
4. [AnyPS5 Ports PS5 Binaries to PC Without Emulation](#item-tech-news-4) ⭐️ 8.0/10
5. [Francis Halzen Wins 2026 Nobel Prize in Physics for IceCube](#item-tech-news-5) ⭐️ 8.0/10
6. [Polars 2.0 Major Release Announced](#item-tech-news-6) ⭐️ 8.0/10
7. [Synthetic Prior Enables In-Context Language Learning](#item-tech-news-7) ⭐️ 8.0/10

**Financial News**
1. [Paramount Skydance Completes $111B Warner Bros. Discovery Merger](#item-finance-news-1) ⭐️ 8.0/10
2. [SpaceX Reportedly Plans $40 Billion Raise to Buy Nvidia AI Chips](#item-finance-news-2) ⭐️ 8.0/10
3. [Google Signs 3.59GW Long-Term Power Deal With Constellation](#item-finance-news-3) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Shares AI-Generated Solutions to Major Math Problems](https://openai.com/index/sharing-ai-progress-in-mathematics/) ⭐️ 9.0/10

OpenAI published a GitHub repository \(github.com/openai/math\) containing preprints that claim AI-generated solutions to numerous major open mathematics problems. According to community analysis, the list claims to fully solve 90 of the top 500 open problems tracked by proofatlas.ai, with the highest-ranked including Hilbert&\#x27;s tenth problem over Q \(rank 22\), Unique Games \(rank 29\), the Anderson-model extended states problem \(rank 31\), the spacetime Penrose inequality \(rank 37\), nonexistence of Landau–Siegel zeros \(rank 48\), Baum–Connes \(rank 52\), Abundance \(rank 78\), Hadwiger \(rank 80\), Bose–Einstein condensation \(rank 87\), and a two-dimensional entanglement result \(rank 92\). The release also includes a proof of Barnette&\#x27;s Conjecture and a claimed polynomial-time algorithm for three-machine unit-job scheduling, an open problem since Garey and Johnson&\#x27;s 1979 book. The claims are extraordinary and verification remains uncertain, but the concrete artifacts \(preprints and repository\) and substantive expert discussion indicate potentially paradigm-shifting implications for AI-for-mathematics and automated theorem proving.

hackernews · OpenAI Blog · Oct 6, 22:17 · [Discussion](https://news.ycombinator.com/item?id=49984923)

**「Background」** OpenAI published new results on open problems in mathematics from an internal frontier model, sharing Lean proof formalizations and research details on GitHub. The release includes hundreds of findings spanning algebra, number theory, theoretical computer science, and mathematical logic, and mathematicians say it will take months to parse whether the proofs contain novel ideas or mostly combine existing techniques.

**「Impact」** If the claimed results hold up, the affected communities are mathematicians and theoretical computer scientists working on the listed problems, including Hilbert&\#x27;s tenth problem over Q, Unique Games, and Barnette&\#x27;s Conjecture, whose status would shift from open to resolved pending verification. The claims remain unverified, so the practical consequence depends on independent checking of the preprints and repository.

**「Community Discussion」** Commenters highlighted the scale of the claims, noting that the repository asserts full solutions to 90 of the top 500 open problems, and quoted Kevin Buzzard&\#x27;s 2020 Notices of the AMS question about how much further one human with total knowledge of modern pure mathematics could see, suggesting the answer is now emerging. A TCS/scheduling commenter said the three-machine unit-job scheduling result is less important than Unique Games but has been open since 1979, while another commenter described Barnette&\#x27;s Conjecture as an approachable graph theory problem they had failed to solve with state-of-the-art models and said the posted proof looks approachable at first glance. Others emphasized that the Unique Games Conjecture is a seminal complexity-theory assumption underlying many inapproximability results, underscoring the significance if the proof holds.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/sharing-ai-progress-in-mathematics/">Sharing AI progress in mathematics - OpenAI</a></li>
<li><a href="https://www.scientificamerican.com/article/openai-unleashes-hundreds-more-math-results-upon-a-field-already-in-shock/">OpenAI unleashes hundreds more math results... | Scientific American</a></li>
<li><a href="https://www.nytimes.com/2026/10/06/science/openai-math-problems.html">OpenAI Releases Findings on 377 Math Problems, Further ...</a></li>
<li><a href="https://techjournal.org/openai-astra-solves-open-math-problems">OpenAI Astra Solves 10 Open Math Problems for $2,000</a></li>
<li><a href="https://openai.com/index/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer science</a></li>
<li><a href="https://officechai.com/ai/big-deal-how-the-math-community-has-reacted-to-openais-astra-model-solving-10-open-math-problems/">&quot;Big Deal&quot;: How The Math Community Has Reacted To OpenAI&#x27;s ...</a></li>

</ul>
</details>

**Tags**: `#AI for mathematics`, `#automated theorem proving`, `#open problems`, `#research`, `#OpenAI`

---

<a id="item-tech-news-2"></a>
### [Mistral Large 4 Trained on 3,800 GPUs in Europe](https://mistral.ai/news/mistral-large-4//) ⭐️ 8.0/10

Mistral announced Mistral Large 4, a new flagship model that the company says was trained from scratch on roughly 3,800 NVIDIA Grace Blackwell GPUs in its own datacenters in Europe. The release drew heavy Hacker News discussion \(1,596 points, 968 comments\) focused on its benchmarks, reasoning controls, and European training and inference. Commenters noted that the model&\#x27;s reasoning setting supports only &quot;none&quot; or &quot;high,&quot; and one tester reported the difference was minimal, with &quot;high&quot; producing fewer output tokens than &quot;none.&quot; Community members highlighted strong vision and cyber-security benchmark results, and one commenter working at Plotly said the model was 10x cheaper than Mistral Medium 3.5 from April while improving their data analytics benchmark from 58% to 74% correct. The item itself is a link post with limited primary detail, and some claims remain unverified.

hackernews · Philpax · Oct 6, 13:15 · [Discussion](https://news.ycombinator.com/item?id=49977979)

**「Background」** Mistral AI is a French AI company that has positioned itself as Europe&\#x27;s leading developer of frontier large language models. Mistral Large 4 is its new flagship model, released in Research Public Preview with plans to release the weights of the 1T parameter \(49B active\) model at the end of October. It was trained from scratch on roughly 3,800 NVIDIA Grace Blackwell GPUs in Mistral&\#x27;s own European datacenters, a detail that matters for discussions of EU technological sovereignty.

**「Impact」** For European enterprises and public-sector buyers, Mistral Large 4&\#x27;s training and inference within EU datacenters under European law offers a sovereignty-aligned alternative to US and Chinese models, though its reliance on NVIDIA Grace Blackwell GPUs leaves that independence partial. Community reports also suggest strong price-performance gains, with one commenter citing a jump from 58% to 74% accuracy on a data analytics benchmark at roughly one-tenth the cost of Mistral Medium 3.5.

**「Community Discussion」** Commenters were broadly positive about the benchmark numbers, with one calling the vision results potentially best in the world and the cyber results a strong defender model, while another framed the EU-based training and inference as an important step for European sovereignty. Skepticism centered on the reasoning controls: simonw found the &quot;none&quot; versus &quot;high&quot; setting made little real difference and that &quot;high&quot; produced fewer output tokens, though he still rated the output the best he had seen from a Mistral model. A separate thread questioned how a ~1T-parameter model trained on about 4,000 GB GPUs could approach Kimi&\#x27;s K3 and beat other leading Chinese lab models.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/articles/mistral-large-4-france-ai">Mistral has released Mistral Large 4, making France home to ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/mistral-large-4-doesn-t-155055704.html?fr=sycsrp_catchall">Mistral Large 4 Doesn’t Just Compete With Chinese Open ...</a></li>
<li><a href="https://byteiota.com/mistral-large-4-drops-today-open-weights-on-october-27/">Mistral Large 4 Drops Today: Open Weights on October 27</a></li>
<li><a href="https://www.constellationr.com/insights/news/mistral-makes-its-open-model-case-mistral-large-4">Mistral makes its open model case with Mistral Large 4</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Mistral`, `#AI models`, `#model training`, `#benchmarks`

---

<a id="item-tech-news-3"></a>
### [Google Releases EmbeddingGemma 2 Under Apache 2.0](https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2/) ⭐️ 8.0/10

Google released EmbeddingGemma 2, an open lightweight multimodal embedding model available under the Apache 2.0 license. The model comes in a 270M text-only configuration and a 440M text-plus-vision configuration, making it suitable for on-device search and privacy-focused retrieval-augmented generation pipelines. The release follows the original EmbeddingGemma, which Google says has surpassed 20 million downloads. Practitioners on Hacker News highlighted the permissive licensing, the moderate model sizes, and the multimodal capability as notable improvements over older embedding models.

hackernews · ilreb · Oct 6, 16:03 · [Discussion](https://news.ycombinator.com/item?id=49980487)

**「Background」** Embedding models convert text, images, and other inputs into numeric vectors so that similar items can be compared and retrieved, which makes them central to search and retrieval-augmented generation \(RAG\) pipelines. Google previously released EmbeddingGemma, a lightweight text embedding model that the source says has been downloaded more than 20 million times for on-device search and privacy-focused RAG. EmbeddingGemma 2 extends that line to multimodal inputs under an Apache 2.0 license, with Google describing it as a compact open model for on-device multimodal embeddings.

**「Impact」** Practitioners building retrieval and embedding pipelines gain an Apache 2.0-licensed multimodal model they can self-host and quantize, avoiding the risk of a proprietary vendor discontinuing a hosted embedding model. The 270M text-only and 440M text+vision sizes make local and on-device deployment feasible, though no published benchmark scores were available at release.

**「Community Discussion」** Commenters broadly welcomed the Apache 2.0 license, with simonw arguing that proprietary hosted-only embedding models are risky because stored vectors become unusable if a vendor retires the model. minimaxir praised the 270M text-only and 440M text-plus-vision sizes as filling a gap for moderate-size embeddings, and kaycebasques asked whether binary quantization would work with EmbeddingGemma 2 as an alternative to MRL. flockonus noted the model is likely close to what Google would ship on Android phones.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.googleblog.com/embeddinggemma-2-the-developer-guide/?ref=communeify.com">EmbeddingGemma 2 : The Developer Guide - Google Developers Blog</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/embeddinggemma-2/">EmbeddingGemma 2 is a best-in-class open model for natively...</a></li>
<li><a href="https://benchlm.ai/models/embeddinggemma-2">EmbeddingGemma 2 Context, Specs &amp; Sources (October 2026 )</a></li>
<li><a href="https://cellcog.ai/blog/embeddinggemma-2/">EmbeddingGemma 2 : Benchmarks , Specs and How to Run It | CellCog</a></li>

</ul>
</details>

**Tags**: `#embeddings`, `#multimodal`, `#open-source`, `#machine-learning`, `#google`

---

<a id="item-tech-news-4"></a>
### [AnyPS5 Ports PS5 Binaries to PC Without Emulation](https://github.com/boykopovar/AnyPS5) ⭐️ 8.0/10

AnyPS5 is a reverse-engineering project that ports PS5 binaries to PC by mapping 87% of system libraries without emulation. The project, hosted on GitHub by boykopovar, aims to run PS5 binaries natively on PC hardware rather than through an emulator. It is not a finished product, and the remaining 13% of system libraries are unmapped. The approach has drawn substantial community discussion about its technical novelty and legal and industry implications.

hackernews · Fe2O3 · Oct 6, 23:28 · [Discussion](https://news.ycombinator.com/item?id=49985664)

**「Background」** Emulation traditionally recreates a console&\#x27;s hardware and system software so that unmodified games can run on another platform. AnyPS5 takes a different route: it rewrites the game&\#x27;s own program, replaces Sony&\#x27;s system software with community-made stand-ins, and outputs a native .exe, with many pull requests marked as AI-assisted. The project is still early — it can execute up to a game&\#x27;s main function but has not yet fully run a complete game, and no public release is available.

**「Impact」** If AnyPS5&\#x27;s approach matures, it could let PC users run PS5 binaries without emulation, reducing vendor lock-in and potentially enabling day-one PC ports. However, legal precedent \(Sony v. Connectix, Sony v. Bleem\) protects reverse engineering for interoperability, but bypassing DRM or shipping copyrighted firmware remains a DMCA risk, and community members note that such projects often face takedowns \(e.g., Yuzu, Ryujinx\).

**「Community Discussion」** Commenters debated the project&\#x27;s implications, with one arguing it could push Sony, Nintendo, and Microsoft further toward cloud gaming to prevent such reverse engineering, while another noted the importance of local git clone backups because similar projects like Yuzu and Ryujinx were taken down through legal threats. A third commenter joked about whether this means a day-one PC port of GTA 6.

<details><summary>References</summary>
<ul>
<li><a href="https://latestintech.com/anyps5-project-ps5-games-pc-port/">AnyPS 5 Project : Impressive PS 5 -to- PC Port , No Emulator</a></li>
<li><a href="https://www.youtube.com/watch?v=Go_h0Y7BUm0">Modders Used AI to Port the PS 5 to PC … It&#x27;s 80% Done - YouTube</a></li>
<li><a href="https://en.3dmgame.com/news/4897">Open-source project AnyPS 5 attempts to run PS 5 games on Windows...</a></li>
<li><a href="https://aliteq.com/is-game-emulation-legal">Is emulation legal? What US emulation laws and court cases ...</a></li>
<li><a href="https://www.twoaveragegamers.com/are-emulators-legal-2026/">Are Emulators Legal? Everything You Need to Know in 2026</a></li>
<li><a href="https://expertbeacon.com/is-ps5-emulator-illegal/">Is Ps5 Emulator Illegal? - ExpertBeacon</a></li>

</ul>
</details>

**Tags**: `#reverse-engineering`, `#game-console`, `#binary-compatibility`, `#systems-programming`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [Francis Halzen Wins 2026 Nobel Prize in Physics for IceCube](https://www.nobelprize.org/prizes/physics/2026/) ⭐️ 8.0/10

The Royal Swedish Academy of Sciences announced on October 6 that the 2026 Nobel Prize in Physics goes to Francis Halzen of the University of Wisconsin–Madison for his decisive contributions to the IceCube Neutrino Observatory and the discovery of high-energy neutrinos of astrophysical origin. Halzen proposed the idea of detecting neutrinos in Antarctic ice in 1988 and led the effort that became IceCube, a cubic-kilometer detector buried at the South Pole. Neutrinos are electrically neutral, nearly massless elementary particles that interact only via the weak nuclear force and gravity, making them extremely difficult to detect; IceCube observes them indirectly when neutrino interactions produce charged particles that emit Cherenkov radiation in the ice. The award recognizes both the conception of the large-scale instrument and the astrophysical results it enabled.

hackernews · solarist · Oct 6, 09:48 · [Discussion](https://news.ycombinator.com/item?id=49976265)

**「Background」** Neutrinos are elementary particles produced in nuclear reactions such as those inside stars, supernovae, and radioactive decay; they have no electric charge and near-zero mass, interacting only via the weak nuclear force and gravity, which makes them extremely difficult to detect. Francis Halzen proposed in 1988 that the deep ice at the South Pole could be used to track these particles, leading to the IceCube Neutrino Observatory, a cubic-kilometer volume of ice instrumented with light sensors. The detector works by converting neutrinos into charged particles that are then observed through Cherenkov radiation, emitted when a charged particle travels faster than light in the ice medium.

**「Impact」** The award recognizes IceCube&\#x27;s transformation of a cubic kilometer of Antarctic ice into a Cherenkov detector that has recorded roughly 700,000 neutrinos between 100 GeV and 1 PeV and 200,000 between 10 GeV and 100 GeV, with purity above 99% against downgoing cosmic-ray muons, establishing a new observational window on the high-energy universe.

**「Community Discussion」** Commenters highlighted the scale and boldness of the project, with one describing the appeal of building a South Pole base to bury sensors in ice and another sharing firsthand experience helping with construction at the South Pole in 2009. Others explained the detection mechanism—neutrino conversion into charged particles observed via Cherenkov radiation—and noted the practical engineering work behind the science, including a trip to the station solely to install Debian for the data-processing systems.

<details><summary>References</summary>
<ul>
<li><a href="https://icecube.wisc.edu/news/awards/2026/10/francis-halzen-icecube-principal-investigator-wins-2026-physics-nobel-prize/">Francis Halzen , IceCube principal investigator, wins 2026 Physics...</a></li>
<li><a href="https://www.nobelprize.org/prizes/physics/">NobelPrize .org</a></li>
<li><a href="https://www.theguardian.com/science/2026/oct/06/nobel-prize-in-physics-francis-halzen-south-pole-neutrinos-icecube-detector">Nobel prize in physics goes to Francis Halzen for... | The Guardian</a></li>
<li><a href="https://icecube.wisc.edu/science/research/">Research Highlights – IceCube Nobel Prize in Physics 2026 Scientific Background Latest results from the IceCube Neutrino Observatory Nobel prize in physics goes to Francis Halzen for south pole ... 2026 Nobel Prize in Physics awarded to Francis Halzen ...</a></li>

</ul>
</details>

**Tags**: `#physics`, `#scientific-computing`, `#instrumentation`, `#neutrino-detection`, `#research`

---

<a id="item-tech-news-6"></a>
### [Polars 2.0 Major Release Announced](https://pola.rs/posts/release-polars-2/) ⭐️ 8.0/10

Polars 2.0, a major release of the Rust/Python DataFrame library, has been announced by the project at pola.rs. The announcement is significant for software engineers and data practitioners working in the Python and Rust data ecosystems, where Polars is widely used. However, the supplied item contains only a link to a comments page and no technical details, changelog, benchmarks, or compatibility notes, so the specific changes, performance claims, and migration requirements in this release cannot be verified from the available content.

rss · Lobsters · Oct 6, 14:30

**「Background」** Polars is an open-source DataFrame library implemented in Rust with Python bindings, widely used in data engineering and analytics workflows. The project announced a pre-release of Polars 2.0 on September 2, 2026, describing it as a version bump rather than a large feature release, with the stable 2.0 release expected in the following weeks. The project maintains separate Python and Rust release channels via GitHub, where changelogs for each release are published.

**「Impact」** Polars 2.0&\#x27;s redesigned API, GPU acceleration via cuDF integration, and streaming improvements directly affect Python and Rust data practitioners who rely on the library for DataFrame workloads. The release also includes SQL benchmarks against DuckDB 1.5.6, DuckDB 2.0 alpha, and DataFusion 54.0.0, indicating performance comparisons are part of the update&\#x27;s positioning.

<details><summary>References</summary>
<ul>
<li><a href="https://pola.rs/posts/release-polars-2/">Polars — Release of Polars 2.0</a></li>
<li><a href="https://pola.rs/posts/announcing-polars-2/">Polars — Pre-release of Polars 2.0</a></li>
<li><a href="https://docs.pola.rs/releases/changelog/">Changelog - Polars user guide</a></li>
<li><a href="https://pyrastra.com/posts/polars-2-dataframe-api-2026/">Polars 2.0: What the New DataFrame API Means for Python Data ...</a></li>
<li><a href="https://pola.rs/posts/release-polars-2/">Polars — Release of Polars 2.0</a></li>

</ul>
</details>

**Tags**: `#polars`, `#dataframes`, `#rust`, `#python`, `#open-source`

---

<a id="item-tech-news-7"></a>
### [Synthetic Prior Enables In-Context Language Learning](https://www.reddit.com/r/MachineLearning/comments/1wyzhdw/learning_to_learn_a_language_incontext_learning/) ⭐️ 8.0/10

A new paper, &quot;Learning to Learn a Language,&quot; extends prior-fitted networks \(the approach behind TabPFN\) from tabular data to structured sequences such as natural language. The authors define a prior over languages in which every training sequence is generated by a randomly sampled recurrent causal model, so each sequence constitutes a new synthetic &quot;language.&quot; A 300M-parameter byte-level transformer trained only on these synthetic sequences can then predict real languages in context with frozen weights: on Wikipedia text, its next-byte predictions improve the more it reads, in all six tested languages \(English, Chinese, Hindi, Arabic, Japanese, Korean\), going from 8 bits per byte down to 0.9–2.4 after a million bytes. The same model also learns in context to count, compare numbers, add approximately, and predict deterministic sequences such as the primes or the Kolakoski sequence. The authors note it remains far worse on text than classical language models trained on trillions of tokens, since their model sees at most a million bytes of a language at test time, but they highlight that the ability to learn a language in context can emerge from a synthetic non-linguistic prior. The paper, code, and weights are available at arxiv.org/abs/2610.05879, github.com/cbl/prior-fitted-language-model, and huggingface.co/lennartcb/pflm1.

reddit · r/MachineLearning · /u/cbl007 · Oct 6, 10:50

**「Background」** Prior-fitted networks \(PFNs\) are a class of transformer models trained on synthetic datasets sampled from a prior distribution so that they approximate the posterior predictive distribution through in-context learning, rather than updating weights at test time. The approach was popularized by TabPFN, a 2022 transformer for tabular classification and regression on small- to medium-sized datasets. The paper discussed here extends the PFN idea from tabular data to structured sequences such as natural language.

**「Impact」** The Prior-Fitted Language Model \(PFLM\) demonstrates that a 300M-parameter byte-level transformer pretrained only on synthetic non-linguistic data can adapt to real natural languages in context with frozen weights, potentially offering a lightweight alternative for low-resource or on-the-fly language adaptation. However, the authors note it remains far worse on text than classical language models trained on trillions of tokens, as it sees at most a million bytes of a language at test time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TabPFN">TabPFN - Wikipedia</a></li>
<li><a href="https://github.com/Cloudy1225/Awesome-Prior-Data-Fitted-Networks">GitHub - Cloudy1225/Awesome- Prior -Data- Fitted - Networks ...</a></li>
<li><a href="https://www.emergentmind.com/topics/prior-data-fitted-transformer-network-pfn">Prior -Data Fitted Transformer Network</a></li>
<li><a href="https://arxiv.org/abs/2610.05879">[2610.05879] Learning to Learn a Language - arXiv.org</a></li>
<li><a href="https://huggingface.co/papers/2610.05879">Paper page - Learning to Learn a Language</a></li>
<li><a href="https://arxiv.org/abs/2610.05879">[2610.05879] Learning to Learn a Language</a></li>

</ul>
</details>

**Tags**: `#in-context learning`, `#prior-fitted networks`, `#language modeling`, `#meta-learning`, `#synthetic data`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Paramount Skydance Completes $111B Warner Bros. Discovery Merger](https://arstechnica.com/tech-policy/2026/10/paramount-completes-111b-warner-merger-creating-skydance-behemoth/) ⭐️ 8.0/10

Paramount Skydance announced on October 6 that it completed its roughly $111 billion acquisition of Warner Bros. Discovery, creating a combined media company spanning film, television, streaming, and news. The merged company, to be known simply as Skydance, will include the Paramount and Warner Bros. studios, the Paramount+ and HBO Max streaming services, and the CNN and CBS News divisions.

hackernews · Mgtyalx · Oct 6, 20:33 · [Discussion](https://news.ycombinator.com/item?id=49983703)

**「Background」** The deal combines two media and entertainment companies with more than a century of history each, and the merged company will be known simply as Skydance, according to the report. Community commenters noted that Time Warner has been acquired before — by AOL in 2001 and by AT&amp;T in 2018 — and that the new company carries significant debt, though those points are opinions rather than verified facts.

**「Impact」** The combined company would control major film and TV studios, the Paramount+ and HBO Max streaming services, and two newsrooms, CNN and CBS News, concentrating a large share of US media under one owner. Community commenters also note the merged firm carries heavy debt, though that claim is not verified by the source.

**Tags**: `#media`, `#mergers-and-acquisitions`, `#antitrust`, `#corporate-consolidation`, `#entertainment`

---

<a id="item-finance-news-2"></a>
### [SpaceX Reportedly Plans $40 Billion Raise to Buy Nvidia AI Chips](https://www.ithome.com/1/010/134.htm) ⭐️ 8.0/10

SpaceX is reportedly planning to raise $40 billion, led by Apollo Global Management, to buy Nvidia AI chips, according to the Financial Times. People familiar with the plan say it involves about $10 billion in bank loans and $30 billion in investment-grade bonds, with the deal expected to close in 2027.

rss · IT HOME · Oct 6, 23:24

**「Background」** SpaceX obtained an investment-grade credit rating \(BBB, the second-lowest investment grade\) after a reported $86 billion IPO in June, and then issued $25 billion in high-grade bonds, which later sold off as investors worried about rising debt and heavy capital spending.

**「Impact」** If completed, the financing would deepen SpaceX&\#x27;s reliance on Nvidia chips and give Nvidia a large new order, while expanding Apollo&\#x27;s role in funding AI infrastructure after it led a $35 billion chip-financing deal in June.

**Tags**: `#SpaceX`, `#Nvidia`, `#AI infrastructure`, `#corporate financing`, `#private credit`

---

<a id="item-finance-news-3"></a>
### [Google Signs 3.59GW Long-Term Power Deal With Constellation](https://www.ithome.com/1/010/063.htm) ⭐️ 8.0/10

Google announced a long-term strategic energy agreement with U.S. power company Constellation totaling 3.59GW. The deal includes 890MW of new nuclear capacity expected online between 2028 and 2032 for a 20-year term, plus 2.7GW of unspecified capacity for 15 years.

rss · IT HOME · Oct 6, 11:37

**「Background」** With Google&\#x27;s funding, Constellation will upgrade 11 nuclear units across multiple states, creating about 7,200 construction jobs, and the two companies will form a five-year technology alliance with Google Cloud and Gemini Enterprise to build an &quot;energy AI&quot; blueprint.

**「Impact」** The agreement signals growing electricity demand from data centers and adds new nuclear capacity to the grid, though it is a single corporate deal rather than a market-wide policy change.

**Tags**: `#energy`, `#nuclear power`, `#big tech`, `#corporate deal`, `#data centers`

---