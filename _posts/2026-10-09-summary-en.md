---
layout: default
title: "Horizon Summary: 2026-10-09 (EN)"
date: 2026-10-09
lang: en
---

> From 236 items, 10 important content pieces were selected

---

**Technology News**
1. [Lean verification of AI autoformalisation may not validate NL proofs](#item-tech-news-1) ⭐️ 8.0/10
2. [Let&\#x27;s Encrypt Plans 64-Day Certificate Lifetimes for Feb 2027](#item-tech-news-2) ⭐️ 8.0/10
3. [FAST Finds First Evolving Native Triple Pulsar System](#item-tech-news-3) ⭐️ 8.0/10
4. [陶哲轩质疑 OpenAI 的 719 份 AI 数学证明](#item-tech-news-4) ⭐️ 8.0/10
5. [ByteDance Seed links DeepSeek long-context drift to phase sensitivity](#item-tech-news-5) ⭐️ 8.0/10

**Financial News**
1. [China&\#x27;s Human Resources Ministry Seeks Public Comment on Draft Rules for Gig Worker Rights](#item-finance-news-1) ⭐️ 8.0/10
2. [OpenAI Annualized Revenue Reported About $20 Billion Below Earlier Figures](#item-finance-news-2) ⭐️ 8.0/10
3. [Brazil&\#x27;s General Election Swept by Bolsonaro Allies](#item-finance-news-3) ⭐️ 7.0/10
4. [The Economist: Europe Needs More Than Trade Weapons for New China Shock](#item-finance-news-4) ⭐️ 7.0/10
5. [JD.com&\#x27;s $2.5 Billion Ceconomy Deal Awaits Final EU Decision by November 4](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Lean verification of AI autoformalisation may not validate NL proofs](https://arxiv.org/abs/2610.08144) ⭐️ 8.0/10

An arXiv article argues that Lean verification of AI autoformalised mathematics does not guarantee the correctness of the original natural-language proof, because semantically faithful translation requires resolving ambiguities in mathematical NL text. The paper claims this ambiguity-resolution problem is arbitrarily high in the Solvability Complexity Index \(SCI\) hierarchy, with SCI = ∞, making it harder than any computational problem including the Halting problem \(SCI = 1\). To illustrate the effect, the article provides examples of AI mistranslations of NL statements and proofs into Lean that produce mismatches between NL proofs and their Lean &quot;verifications.&quot; These examples include OpenAI&\#x27;s announced proof of blow-up of solutions to the Navier-Stokes equations, where the author shows the formalised Lean proof does not correspond to the NL proof of blow-up.

rss · Lobsters · Oct 8, 17:16

**「Background」** Autoformalisation is the process of translating mathematical text from natural language into a formal language such as Lean, after which the formal argument can be mechanically verified. The approach has gained prominence as a way to check mathematical texts, including those produced by AI, and it featured in OpenAI&\#x27;s announced proof of blow-up of solutions to the Navier-Stokes equations, whose manuscript and Lean formalisation were made public and which targeted Clay options C and D for the full Navier-Stokes equations. The paper discussed here is by Alexander Bastounis and two other authors.

**「Impact」** The paper&\#x27;s argument implies that Lean verification of AI autoformalised mathematics cannot by itself certify the original natural-language proof, so claims such as OpenAI&\#x27;s announced Navier-Stokes blow-up proof should not be treated as verified on the strength of the Lean formalisation alone. Because ambiguity resolution in mathematical natural language is arbitrarily high in the Solvability Complexity Index hierarchy \(SCI = ∞\), the authors contend that semantically faithful autoformalisation is harder than any computational problem, including the Halting problem \(SCI = 1\).

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.08144">[2610.08144] Navier - Stokes lost in translation: Why Lean verification...</a></li>
<li><a href="https://dev.to/axrisi/navier-stokes-solved-what-openais-proof-shows-and-why-its-disputed-4a31">Navier - Stokes solved? What OpenAI &#x27;s proof ... - DEV Community</a></li>
<li><a href="https://www.datacamp.com/blog/openai-navier-stokes-math-problem">Did AI Solve Navier - Stokes ? OpenAI &#x27;s Claim, Explained | DataCamp</a></li>
<li><a href="https://arxiv.org/pdf/2610.08144">Navier-Stokes lost in translation: Why Lean verification of AI...</a></li>
<li><a href="https://jbenartzi.github.io/papers/SCI_STOC_Final.pdf">The Solvability Complexity Index - Computer Science and Logic</a></li>
<li><a href="https://www.youtube.com/watch?v=HxidCCh6eIM">Anders Hansen: What is the Solvability Complexity Index ... - YouTube</a></li>

</ul>
</details>

**Tags**: `#autoformalisation`, `#Lean`, `#AI for mathematics`, `#formal verification`, `#Navier-Stokes`

---

<a id="item-tech-news-2"></a>
### [Let&\#x27;s Encrypt Plans 64-Day Certificate Lifetimes for Feb 2027](https://letsencrypt.org/2026/10/07/64-day-certs.html) ⭐️ 8.0/10

Let&\#x27;s Encrypt has announced that it will move to 64-day TLS certificate lifetimes in February 2027, according to a post on letsencrypt.org. The change affects anyone managing TLS certificates through the widely used free certificate authority, which issues certificates for a vast number of sites. Shorter lifetimes increase the importance of reliable automated renewal, since certificates will expire roughly twice as fast as under the current 90-day default. The supplied item is only a link with a comments pointer and provides no further technical detail, so specifics such as the exact rollout date, transition schedule, and any compatibility constraints are not available in the source content.

rss · Lobsters · Oct 8, 19:06

**「Background」** TLS certificates are used to authenticate websites and encrypt connections, and their validity periods have historically been measured in months or years. Let&\#x27;s Encrypt, a widely used free certificate authority, has been progressively shortening lifetimes as automated issuance and renewal via the ACME protocol have become standard. The planned move to 64-day certificates in February 2027 continues that trend and is accompanied by compressed validation timelines, including authorization reuse periods shrinking from 30 days to 10 days and eventually to seven hours by 2028.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/gadgets/2026/10/lets-encrypt-cuts-certificate-lifetimes-to-64-days-starting-february-2027/">Let &#x27; s Encrypt cuts certificate lifetimes to 64 days starting February ...</a></li>
<li><a href="https://www.geekslop.com/technology-articles/computers-programming/hacking-and-security-technology-articles/2026/lets-encrypt-64-day-ssl-certs">Let &#x27; s Encrypt Cuts SSL Cert Lifetimes To 64 Days ... - Geek Slop</a></li>

</ul>
</details>

**Tags**: `#TLS certificates`, `#Let&\#x27;s Encrypt`, `#web PKI`, `#infrastructure`, `#security`

---

<a id="item-tech-news-3"></a>
### [FAST Finds First Evolving Native Triple Pulsar System](https://www.ithome.com/1/010/830.htm) ⭐️ 8.0/10

China&\#x27;s FAST telescope discovered pulsar J0435+3233, the first pulsar in a still-evolving native triple system and the second confirmed pulsar triple system, with results published in ApJL on October 9, 2026. The 3.2 ms pulsar, first detected on June 8, 2020, orbits a white dwarf every 8 days in a circular orbit, and its spin period increases by 1 ns per year—two orders of magnitude higher than similar pulsars, a result previously published in Nature Astronomy in April 2026. A second companion, a Sun-like star of about one solar mass, orbits the pulsar-white dwarf pair every 73.5 years on an eccentric orbit \(e=0.6\) and causes the observed period increase. The team combined FAST radio data with Gaia, 2MASS, PanSTARRS optical/infrared archives and 18 years of Fermi gamma-ray data \(160 valid photons\) to confirm the triple nature and measure component masses; a European team independently reached the same conclusion, but the Chinese team&\#x27;s orbital geometry and parameters are an order of magnitude more precise.

rss · IT HOME · Oct 9, 02:30

**「Background」** Pulsar triple systems are extremely rare; before this work, the only known pulsar triple system outside planetary systems was found by a US team using the GBT and consists of a pulsar and two white dwarfs, all fully evolved. Native triple systems form from the same cloud and can preserve clues about stellar evolution and gravitational interactions. FAST, the Five-hundred-meter Aperture Spherical radio Telescope in China, is the world&\#x27;s largest single-dish radio telescope and has been used for pulsar discovery and timing.

**「Impact」** This system provides a rare natural laboratory for testing strong equivalence principle and other gravitational theories, and for studying triple-star evolution, because its clear gravitational interactions and multi-band observability allow precise dynamical modeling.

**Tags**: `#astronomy`, `#FAST telescope`, `#pulsars`, `#scientific research`, `#multi-band observation`

---

<a id="item-tech-news-4"></a>
### [陶哲轩质疑 OpenAI 的 719 份 AI 数学证明](https://www.ithome.com/1/010/795.htm) ⭐️ 8.0/10

OpenAI published 719 AI-generated mathematical manuscripts covering 372 result families and hundreds of open research problems, after initially posting 722 on October 6 and retracting 3 on October 7 due to a notation error and its knock-on effects. OpenAI said it consulted the Institute for Advanced Study-hosted Mathematics and AI Advisory Group \(AGMAI\) and its public recommendations, but the release did not fully meet AGMAI&\#x27;s standards: OpenAI still used proprietary models, only 10 manuscripts included model reasoning chains, and about 42% of proofs were not formalized, with no machine-readable metadata linking natural-language proofs to formal artifacts. AGMAI said its advisory role does not constitute endorsement of OpenAI&\#x27;s obtaining or publishing the results, and that the mathematics community must ultimately assess whether its recommendations were adequately implemented. Terence Tao, a Fields Medalist and UCLA mathematics professor, said on mathstodon on October 7 that he does not oppose AI doing mathematics and actively uses AI-assisted research, but strongly opposes making &quot;quickly cracking famous problems with AI&quot; a primary goal or product demonstration, warning of a &quot;proof indigestion&quot; in which AI generates propositions, proofs, and counterexamples faster than humans can verify, understand, write, teach, and absorb them. He also criticized treating Millennium Prize problems such as the Navier-Stokes equations as model capability benchmarks, arguing that speed and quantity are not mathematical understanding and that once a problem is publicly &quot;solved,&quot; it can hardly be restored to &quot;unsolved,&quot; potentially polluting later exploration of alternative paths.

rss · IT HOME · Oct 9, 01:40

**「Background」** The Advisory Group on Mathematics and Artificial Intelligence \(AGMAI\) was announced in September 2026, and mathematician Martin Hairer explained his reasons for joining in a blog post cross-posted by Terence Tao. AGMAI has stated that its advisory role should not be interpreted as a judgment of the impact of these results or an endorsement of the process by which OpenAI obtained them, and that only the mathematical community can undertake the needed assessment. Terence Tao is a Fields Medalist and UCLA mathematics professor who has been an active user of AI-assisted research, including work extending the Green-Tao theorem to higher-degree polynomials.

**「Impact」** Mathematicians reviewing OpenAI&\#x27;s 719 manuscripts face a corpus in which only about 42% of main results have been translated into Lean, and only 10 manuscripts include model reasoning chains, leaving most proofs hard to read and verify. The dispute may push frontier AI labs toward releasing model names, prompts, and formalization metadata, as AGMAI and Terence Tao have demanded, though AGMAI has stated its advisory role does not constitute endorsement of OpenAI&\#x27;s results.

<details><summary>References</summary>
<ul>
<li><a href="https://agmai.org/">agmai .org</a></li>
<li><a href="https://proofsandprompts.com/2026/09/22/why-i-agreed-to-join-agmai/">Why I agreed to join AGMAI – Proofs and Prompts</a></li>
<li><a href="https://terrytao.wordpress.com/2026/09/22/why-i-agreed-to-join-agmai/">Why I agreed to join AGMAI | What&#x27;s new</a></li>
<li><a href="https://mathstodon.xyz/@tao">Terence Tao (@ tao @ mathstodon .xyz) - Mathstodon</a></li>
<li><a href="https://www.webpronews.com/terence-tao-extends-green-tao-theorem-to-polynomials-with-ai/">Terence Tao Extends Green- Tao Theorem to Polynomials with AI</a></li>
<li><a href="https://www.implicator.ai/openai-372-math-results-mathematicians-race-to-read/">OpenAI &#x27;s 372 AI Math Results Leave Mathematicians Racing</a></li>
<li><a href="https://www.zerohedge.com/political/bunker-mode-openais-jaw-dropping-math-blitz-draws-boycott-warning-over-crypto-wallets">&#x27;Bunker Mode&#x27;: OpenAI &#x27;s Jaw-Dropping Math Blitz Draws... | ZeroHe...</a></li>

</ul>
</details>

**Tags**: `#AI for mathematics`, `#OpenAI`, `#formal verification`, `#research transparency`, `#peer review`

---

<a id="item-tech-news-5"></a>
### [ByteDance Seed links DeepSeek long-context drift to phase sensitivity](https://www.ithome.com/1/010/780.htm) ⭐️ 8.0/10

ByteDance&\#x27;s Seed team submitted an arXiv preprint in late September reporting that chunked KV-cache compression introduces a systematic failure mode it calls &quot;phase sensitivity,&quot; which it identifies as the cause of DeepSeek&\#x27;s inconsistent long-context behavior. The compression reduces memory and attention costs by collapsing windows of consecutive tokens into fewer cache entries at a fixed stride, but this creates a new positional coordinate: a token&\#x27;s phase, or its position relative to compression window boundaries. The researchers evaluated base and post-trained DeepSeek-V4-Flash and DeepSeek-V4-Pro, plus post-trained DeepSeek-V4.1-Flash, and found an asymmetric pattern in which the same information is easy to retrieve in one phase but hard in another. In large open-weight models using this compression, long-context retrieval accuracy can vary by up to 40 percentage points across phases, a periodic weakness that average benchmark scores may hide.

rss · IT HOME · Oct 9, 00:49

**「Background」** ByteDance is a Chinese internet technology company founded in 2012 and known for platforms such as TikTok/Douyin and Toutiao. Its Seed team conducts AI research, and the referenced work is an arXiv preprint submitted in late September. KV-cache compression reduces the memory and attention cost of long-context inference by compressing windows of consecutive tokens into fewer cache entries.

**「Impact」** For developers and organizations serving long-context models with chunked KV-cache compression, average retrieval benchmarks may hide position-dependent accuracy swings of up to 40 points, so evaluation should include phase-aware tests rather than relying on aggregate scores alone.

<details><summary>References</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/ByteDance">ByteDance - Wikipedia</a></li>
<li><a href="https://www.bytedance.com/en/">ByteDance - Inspire Creativity, Enrich Life</a></li>

</ul>
</details>

**Tags**: `#long-context`, `#KV-cache`, `#DeepSeek`, `#LLM inference`, `#research paper`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s Human Resources Ministry Seeks Public Comment on Draft Rules for Gig Worker Rights](https://mp.weixin.qq.com/s/saqkOXlhe0wX7qD83vdkRw) ⭐️ 8.0/10

China&\#x27;s Ministry of Human Resources and Social Security released a draft regulation on protecting new-form employment workers&\#x27; rights on October 8, covering ride-hailing drivers, delivery riders, and livestreamers, with public comment open until November 8. The draft states that normal labor pay must not fall below the local minimum wage, that workers should get proper rest after 4 consecutive hours of work, and that major decisions such as stopping dispatch orders or banning accounts must be reviewed by humans rather than made automatically by algorithms.

telegram · zaihuapd · Oct 8, 09:23

**「Background」** China&\#x27;s Ministry of Human Resources and Social Security issued the draft on October 8, opening a public comment period through November 8; the rules target gig-economy workers such as ride-hailing drivers, delivery riders, and livestreamers, whose work is typically arranged through platform algorithms rather than traditional employment contracts.

**「Impact」** If finalized, the rules would directly affect platform companies operating ride-hailing, delivery, and livestreaming services, which would need to adjust pay floors, rest scheduling, and algorithmic penalty and account-ban processes; gig drivers, riders, and livestreamers covered by the draft would gain minimum-pay and rest protections and a right to human review of major account decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://news.17173.com/content/10082026/180506121.shtml">news.17173.com/content/10082026/180506121.shtml</a></li>
<li><a href="https://www.workercn.cn/papers/grrb/2026/04/29/5/grrb202604295.pdf">grrb0520260429C</a></li>

</ul>
</details>

**Tags**: `#labor policy`, `#gig economy`, `#regulation`, `#China`, `#platform workers`

---

<a id="item-finance-news-2"></a>
### [OpenAI Annualized Revenue Reported About $20 Billion Below Earlier Figures](https://www.ft.com/content/b66a9858-f8fb-46cb-b506-44bfe26fca2a?syn-25a6b1a6=1) ⭐️ 8.0/10

Financial documents shown to investors indicate OpenAI&\#x27;s annualized revenue was close to $50 billion at the end of September, roughly $20 billion below the widely reported $70 billion, according to the Financial Times. The gap partly reflects different accounting: Anthropic counts revenue sold through cloud partners such as AWS and Google Cloud, while OpenAI does not; OpenAI declined to comment.

telegram · zaihuapd · Oct 8, 17:22

**「Background」** The $70 billion figure came from reports citing people familiar with OpenAI&\#x27;s finances, including an Axios report that its annual recurring revenue was nearing that level as enterprise sales more than doubled since July. Annualized revenue is a run-rate estimate, not audited full-year results, and the two figures differ partly because Anthropic counts sales made through cloud partners such as AWS and Google Cloud while OpenAI does not.

**「Impact」** The disclosure weighed on AI-linked shares, with Nvidia, Oracle and CoreWeave among the stocks that fell after the revenue figure circulated, according to CNBC. The gap also matters to investors comparing OpenAI with Anthropic, because the two companies count cloud-partner revenue differently, the Financial Times reported.

<details><summary>References</summary>
<ul>
<li><a href="https://www.axios.com/2026/09/29/scoop-openais-annual-recurring-revenue-nears-70b">Scoop: OpenAI &#x27;s annual recurring revenue nears $ 70 B</a></li>
<li><a href="https://www.pymnts.com/news/artificial-intelligence/2026/openai-annualized-revenue-nears-70-billion-amid-enterprise-growth/">PYMNTS | OpenAI Annualized Revenue Nears $ 70 B Amid Enterprise...</a></li>
<li><a href="https://www.rkjdev.com/blog/openai-revenue-run-rate-nears-70-billion/">OpenAI Revenue Run Rate Nears $ 70 B as Sales Surge | rkj dev</a></li>
<li><a href="https://www.cnbc.com/2026/10/08/open-ai-revenue-nvidia-oracle-coreweave.html">Nvidia, Oracle, other AI stocks sink on OpenAI revenue report</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/msft-orcl-nvda-qqq-focus-190141481.html">MSFT, ORCL, NVDA, QQQ In Focus: OpenAI ’s Annualized Revenue ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI industry`, `#revenue reporting`, `#private company financials`, `#investor sentiment`

---

<a id="item-finance-news-3"></a>
### [Brazil&\#x27;s General Election Swept by Bolsonaro Allies](https://www.economist.com/the-americas/2026/10/08/brazil-falls-into-magas-orbit) ⭐️ 7.0/10

Brazil&\#x27;s general election has been swept by the Bolsonaro clan and its allies, according to The Economist. The report gives no vote counts, seat totals, or policy specifics, so the scale of the win and its economic consequences remain unclear.

rss · The Economist · Oct 8, 13:01

**「Background」** Brazil&\#x27;s October 2026 general election followed a first-round presidential vote in which Senator Flávio Bolsonaro, son of former president Jair Bolsonaro, advanced to a runoff against incumbent Luiz Inácio Lula da Silva, according to The Guardian. Jair Bolsonaro served as a federal deputy from 1991 to 2018 before winning the presidency.

**「Impact」** The first-round result points to a runoff between Lula and a Bolsonaro-family candidate, leaving Brazil&\#x27;s policy direction unresolved for now. Flavio Bolsonaro has said he would work with both the US and China as president, a stance that matters for investors in Brazilian assets and for trade ties with both powers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jair_Bolsonaro">Jair Bolsonaro - Wikipedia</a></li>
<li><a href="https://www.theguardian.com/world/2026/oct/05/flavio-bolsonaro-brazilian-presidency-election-shock-first-round-victory">Flávio Bolsonaro poised to win Brazilian presidency... | The Guardian</a></li>
<li><a href="https://www.economist.com/the-americas/2026/10/08/brazil-falls-into-magas-orbit">Brazil falls into MAGA’s orbit</a></li>
<li><a href="https://www.independent.co.uk/news/world/americas/brazil-election-results-bolsonaro-lula-b3061216.html">Brazil heads to runoff as Bolsonaro leads Lula in... | The Independent</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-10-08/brazil-election-bolsonaro-says-he-d-work-with-us-china-as-president">Brazil Election : Bolsonaro Says He’d Work With US... - Bloomberg</a></li>

</ul>
</details>

**Tags**: `#Brazil`, `#elections`, `#politics`, `#emerging markets`, `#Bolsonaro`

---

<a id="item-finance-news-4"></a>
### [The Economist: Europe Needs More Than Trade Weapons for New China Shock](https://www.economist.com/leaders/2026/10/08/how-europe-should-deal-with-the-new-china-shock) ⭐️ 7.0/10

The Economist argues in a leader that Europe needs a strategy beyond stockpiling &quot;second-strike&quot; retaliatory trade weapons to handle a new wave of Chinese economic pressure. The article, dated October 8, 2026, offers no concrete figures or detailed policy proposals in the supplied headline and subheading.

rss · The Economist · Oct 8, 13:01

**「Background」** The phrase &quot;China shock&quot; originally described the wave of cheap Chinese imports that hurt manufacturing jobs in the 2000s. The Economist&\#x27;s leader argues that Europe now faces a new version of that pressure and that building up &quot;second-strike&quot; trade weapons—retaliatory measures held in reserve—is not a sufficient response.

**「Impact」** European industries that depend on Chinese rare earths and magnets could face supply disruptions if trade tensions escalate, since the EU&\#x27;s anti-coercion instrument allows it to restrict goods and services exports but has never been used. The European Parliament has warned that relations with Beijing have reached a &quot;critical point.&quot;

<details><summary>References</summary>
<ul>
<li><a href="https://www.ft.com/content/4416101f-5072-4ee0-aa12-5b1daf25b31b?syn-25a6b1a6=1">Germany and France agree on last-resort tool against trade threats</a></li>
<li><a href="https://www.euronews.com/2026/10/07/meps-urge-tougher-action-against-china-as-tensions-hit-critical-point">MEPs urge tougher action against China as tensions hit... | Euronews</a></li>

</ul>
</details>

**Tags**: `#EU trade policy`, `#China`, `#trade tensions`, `#industrial policy`

---

<a id="item-finance-news-5"></a>
### [JD.com&\#x27;s $2.5 Billion Ceconomy Deal Awaits Final EU Decision by November 4](https://www.ithome.com/1/010/783.htm) ⭐️ 7.0/10

JD.com&\#x27;s roughly $2.5 billion acquisition of German electronics retailer Ceconomy has cleared German, French and Italian regulators and now awaits a final European Commission decision under the Foreign Subsidies Regulation by November 4. JD.com launched a voluntary cash offer in July 2025 at €4.60 per share, valuing Ceconomy at about €2.2 billion, and expects to hold roughly 85.2% of the company after completion.

rss · IT HOME · Oct 9, 01:03

**「Background」** The European Commission opened an in-depth investigation in May 2026 and issued a statement of objections to JD.com in July, examining whether past favorable financing, tax breaks or government subsidies gave JD.com an unfair edge in the purchase; JD.com has since offered remedies, including opening its European logistics and technology capabilities to Ceconomy at market prices and letting smaller rivals use those services on fair, non-discriminatory terms.

**「Impact」** If approved, the deal would give JD.com control of Ceconomy&\#x27;s MediaMarkt and Saturn consumer-electronics chains, expanding its European retail footprint, while the EU&\#x27;s conditions on consumer-data isolation and in-EU storage would shape how that data is handled.

**Tags**: `#M&amp;A`, `#EU regulation`, `#retail`, `#cross-border investment`, `#JD.com`

---