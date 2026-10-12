---
layout: default
title: "Horizon Summary: 2026-10-12 (EN)"
date: 2026-10-12
lang: en
---

> From 175 items, 10 important content pieces were selected

---

**Technology News**
1. [华为线下展出麒麟9050 Pro逻辑折叠芯片](#item-tech-news-1) ⭐️ 8.0/10
2. [Japan Declares Cyberspace Emergency After Attack Surge](#item-tech-news-2) ⭐️ 8.0/10

**Technology Blog**
1. [Sliced-Wasserstein Embeddings and HNSW for Painting Color Search](#item-tech-blog-1) ⭐️ 8.0/10
2. [Mapping North Korea in OpenStreetMap: A Cartographer&\#x27;s Account](#item-tech-blog-2) ⭐️ 7.0/10
3. [Reverse Engineering a Commercial Spatial Audio Effect](#item-tech-blog-3) ⭐️ 7.0/10
4. [A 414k-Parameter Transformer Learns Boids, But Probes May Mislead](#item-tech-blog-4) ⭐️ 7.0/10

**Financial News**
1. [Amazon in Talks to Acquire AI Startup Decart at Reported ~$7 Billion Valuation](#item-finance-news-1) ⭐️ 7.0/10
2. [China Opens Consultation on Major Food Safety Law Revision](#item-finance-news-2) ⭐️ 7.0/10
3. [Turkey Bans Social Media Accounts for Children Under 15](#item-finance-news-3) ⭐️ 7.0/10
4. [Foreign Investors Pull About $131 Billion From Korean Stocks This Year](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [华为线下展出麒麟9050 Pro逻辑折叠芯片](https://www.ithome.com/1/011/756.htm) ⭐️ 8.0/10

华为于10月12日在上海练秋湖举行的终端创新技术沟通会上，线下展出了号称全球首款逻辑折叠芯片的麒麟9050 Pro，其“真身”位于HUAWEI Mate XT 2 \| ULTIMATE DESIGN非凡大师三折叠手机展台。这是华为时隔多年再次公开展示麒麟芯片，但当天芯片内容不多，官方专场安排在次日上午。作为参考，麒麟9050 Pro已于9月7日随Mate XT 2首发亮相，并在10月1日Mate 90系列发布会上确认搭载于Mate 90 Pro Max典藏版与Mate 90 RS非凡大师；该芯片集成灵犀CPU、马良GPU和达芬奇架构NPU，马良GPU计算单元与缓存翻倍，NPU支持端侧部署30B参数混合专家架构大模型。华为公布的数据显示，Mate 90 Pro Max整机性能较上代提升31%，Mate 90 Pro提升20%，Mate 90标准版提升27%。

rss · IT HOME · Oct 12, 01:28

**「背景」** 麒麟是华为自研的移动芯片系列，此前多年未在公开场合展示。所谓“逻辑折叠”是华为对麒麟9050 Pro芯片的一项新描述，但具体技术含义尚未在本次沟通会上披露。该芯片此前已随Mate XT 2三折叠手机首发，并在Mate 90系列发布会上公布部分规格。

**「影响」** 对关注国产半导体和芯片设计的读者而言，此次展出是麒麟芯片多年后首次线下公开亮相，但“逻辑折叠”的具体技术细节和官方规格仍需等待次日专场公布。

**Tags**: `#华为麒麟芯片`, `#半导体硬件`, `#芯片设计`, `#智能手机`, `#国产芯片`

---

<a id="item-tech-news-2"></a>
### [Japan Declares Cyberspace Emergency After Attack Surge](https://www.ft.com/content/2d4333d1-8119-44a4-a5a5-2ee9ef2544fa?syn-25a6b1a6=1) ⭐️ 8.0/10

Japan declared a &quot;cyberspace state of emergency&quot; after a surge of cyberattacks hit more than 20 major companies and government facilities in recent weeks, spanning rail, automotive, healthcare, and government sectors, with tens of millions of customer records potentially exposed. JR East said its ticket booking system may have leaked the email addresses of 1.67 million customers, and multiple incidents have been linked to a ransomware attack on SoftBank subsidiary IDC Frontier. The Financial Services Agency instructed banks to stop accepting driver&\#x27;s licenses as identity proof for new account openings and instead require chip-equipped documents. Experts described Japan&\#x27;s defenses as weak and said AI is lowering the barrier to complex attacks, though no evidence currently links the latest attacks to AI.

telegram · zaihuapd · Oct 11, 06:32

**「Background」** Japan has faced repeated ransomware and data breach incidents in recent years, but the scale and breadth of the latest wave—crossing critical infrastructure and government facilities—prompted an emergency declaration. The attacks coincide with growing concern that generative AI tools could help less-skilled actors craft more sophisticated intrusions, though that link remains unproven here.

**「Impact」** Japanese banks must now change their new-account identity verification processes, and affected companies face potential exposure of tens of millions of customer records, including 1.67 million JR East customer emails.

**Tags**: `#cybersecurity`, `#Japan`, `#ransomware`, `#data breach`, `#critical infrastructure`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Sliced-Wasserstein Embeddings and HNSW for Painting Color Search](https://www.reddit.com/r/MachineLearning/comments/1x39uu6/sliced_wasserstein_embeddings_hnsw_for/) ⭐️ 8.0/10

reddit · r/MachineLearning · /u/Potential-Barber8658 · Oct 11, 14:39

**「Background」** Palette Atlas searches public-domain paintings by color scheme, reducing each image to 128 equal-weight colors. The natural distance between such palettes is the Earth Mover&\#x27;s Distance \(EMD\), but at roughly 6 ms per pair it is far too slow for nearest-neighbor search across 48,695 items.

**「Solution」** The author&\#x27;s insight is to replace exact EMD with a sliced-Wasserstein embedding that lower-bounds it. Colors in OKLab are projected onto 8 directions on a Fibonacci hemisphere, sorted, and averaged into 16 quantiles; the L1 distance between two such vectors approximates the 1D Wasserstein distance averaged over directions. Against exact EMD on 240 queries, this sliced 8x16 L1 embedding achieved 78% top-10 overlap with the exact ranking and a 1.8% distance penalty, versus 69%/3.4% for L2, 45%/13.5% for a soft Hellinger color histogram, and 3%/161% for mean color. The author then wrote an HNSW index from scratch \(M=16, efConstruction=200\), reaching recall@10 of 1.000 at ef=32 and 0.25 ms per query against 14 ms for brute force. Because the vectors&\#x27; intrinsic dimension is about 11, the hierarchy still helps, though the author cites Munyampirwa et al. 2025 on when it does not. One deviation from the standard HNSW paper: the top layer holds 8 k-means landmarks instead of randomly drawn nodes, giving the same search cost \(2,558 vs 2,556 distance computations on average\) while making the top layer one typical painting per color family.

**「Takeaway」** The author argues that a sliced-Wasserstein embedding can preserve most of EMD&\#x27;s ranking quality while making approximate nearest-neighbor search practical, and that a small, measured HNSW modification can improve interpretability without sacrificing performance.

**Tags**: `#sliced-wasserstein`, `#hnsw`, `#approximate-nearest-neighbor`, `#color-embeddings`, `#information-retrieval`

---

<a id="item-tech-blog-2"></a>
### [Mapping North Korea in OpenStreetMap: A Cartographer&\#x27;s Account](https://cartographers-nk.wonyoung.so/) ⭐️ 7.0/10

hackernews · edent · Oct 11, 19:46 · [Discussion](https://news.ycombinator.com/item?id=50047091)

**「Background」** OpenStreetMap \(OSM\) is a collaborative, open-source world map built by volunteers, and its coverage of North Korea—a country with severe restrictions on information—has long puzzled observers. This interactive first-person account by a mapper known as Wonyoung documents how that coverage was assembled, and why it matters.

**「Solution」** The account reconstructs the remote mapping effort through the author&\#x27;s own experience and contributor correspondence. A letter from a mapper identified as &quot;P791&quot; reveals a striking motivation: &quot;I map North Korea to help North Koreans. I select areas that look like they might be good points to escape. In particular, the detailed mapping around Phungso-ri \(풍서리\) is almost entirely my work. I mostly map along the Tumen River, both on the North Korean and Chinese sides. It is important to map the fences, roads, and towns on the Chinese side.&quot; This shows how volunteered geographic information can serve humanitarian ends, with contributors tracing escape routes along a border river. Community commenters found the piece fascinating and praised its layout and navigation, though one noted a preference for a conventional article with static illustrations. The submission provides only the title, URL, and comments rather than the full article text, so the depth of evidence and tradeoffs discussed cannot be fully verified.

**「Takeaway」** The author&\#x27;s account illustrates that OpenStreetMap&\#x27;s detailed coverage of North Korea is not merely a technical achievement but a human one, driven by contributors who map with concrete purposes—in this case, aiding escape along the Tumen River. It underscores the potential of volunteered geographic information to document and support lives in closed societies.

**Tags**: `#OpenStreetMap`, `#North Korea`, `#volunteered geographic information`, `#remote mapping`, `#data visualization`

---

<a id="item-tech-blog-3"></a>
### [Reverse Engineering a Commercial Spatial Audio Effect](http://epestr.com/blog/reverse-engineering-a-commercial-spatial-audio-effect/) ⭐️ 7.0/10

hackernews · epestr · Oct 11, 15:21 · [Discussion](https://news.ycombinator.com/item?id=50044272)

**「Background」** Commercial spatial audio effects are typically shipped as black boxes, so understanding how they actually work requires reverse engineering rather than reading documentation. The author set out to analyze one such effect and explain its internals, a task that demands both DSP knowledge and patience with opaque binaries.

**「Solution」** The write-up is a first-hand account of that reverse-engineering process, walking through how the author probed the effect and reconstructed its signal-processing behavior. Community reaction suggests the piece is technically substantive but leaves some gaps: one commenter wished the article had included an audio comparison at the end, noting they had to record their own voice to hear the result, while another commenter found the processed sound unpleasant, describing it as aggressive &quot;Bose barf&quot;-style processing that trades neutrality for impact on cheap drivers. A separate commenter shared a related 2014 blog post about a commercial spatial audio effect used during mastering of Red Tails, illustrating that such effects can reach professional production despite contested subjective quality. The thread also points to hobbyist interest in downmixing Dolby Atmos to stereo for higher dynamic range, showing the broader context in which these effects are evaluated.

**「Takeaway」** The article offers transferable insight into how a commercial spatial audio effect can be taken apart and understood, but the community response highlights that technical success and subjective sound quality are separate questions, and that before/after comparisons would make such claims easier to judge.

**Tags**: `#audio-dsp`, `#reverse-engineering`, `#spatial-audio`, `#signal-processing`

---

<a id="item-tech-blog-4"></a>
### [A 414k-Parameter Transformer Learns Boids, But Probes May Mislead](https://www.reddit.com/r/MachineLearning/comments/1x39jlu/i_trained_a_414kparameter_transformer_to_fly_a/) ⭐️ 7.0/10

reddit · r/MachineLearning · /u/rage\_81 · Oct 11, 14:25

**「Background」** Boid flocking is a classic multi-agent simulation where simple local rules—cohesion, alignment, and separation—produce emergent group motion. The author built a 12-bird boid simulator in Python and PyTorch and trained a from-scratch transformer \(one token per bird, two attention layers, ~414k weights, laptop CPU\) to predict each bird&\#x27;s next move without being given any boid rules. The goal was to see whether a small model could learn flocking and whether interpretability probes could recover the underlying rules.

**「Solution」** The transformer generalized well: R² 0.990–0.994 on held-out clips across four runs, and it even flew 50 birds despite training only on 12. A small baseline with no attention or positions—seeing only a bird&\#x27;s own move plus the flock average—reached R² 0.40 on one seed. Linear probes found cohesion readable before any training \(R² ~0.85\), while alignment became readable after the first attention layer; ablating the second layer to self-attention removed alignment in all four runs. But the author&\#x27;s first model was not using the flock at all: with 8 ticks of history, a small network seeing only one bird beat the full transformer, suggesting temporal shortcuts can masquerade as flocking. The author remains unsure whether the self-attention ablation is a fair test, since the model never saw that condition during training.

**「Takeaway」** The author&\#x27;s central lesson is that probe-readable rules are not necessarily the rules a model actually uses, and that temporal shortcuts can produce convincing flocking behavior without any multi-agent reasoning. This raises a fair caution for interpretability work: evidence of readable features must be paired with behavioral tests that rule out simpler explanations.

**Tags**: `#interpretability`, `#transformers`, `#multi-agent simulation`, `#ablation methodology`, `#reproducibility`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Amazon in Talks to Acquire AI Startup Decart at Reported ~$7 Billion Valuation](https://www.ithome.com/1/011/720.htm) ⭐️ 7.0/10

Amazon is reportedly in talks to acquire San Francisco-based AI startup Decart at a potential valuation of about $7 billion, according to The Wall Street Journal. Decart makes software that lets developers switch between different AI chips, and the deal could close soon if negotiations proceed without a new bidder.

rss · IT HOME · Oct 11, 23:01

**「Background」** Decart, based in San Francisco, develops software that lets developers switch between different AI chips, and had raised over $400 million from investors including Sequoia Capital, Benchmark, and Radical Ventures, reaching a valuation near $4 billion in a May funding round, according to PitchBook. Anthropic had reportedly discussed acquiring Decart for about $6 billion before abandoning the deal in September, per Bloomberg reports cited by IT Home.

**「Impact」** If completed, the deal would put Decart&\#x27;s cross-chip switching software inside AWS, potentially strengthening Amazon&\#x27;s own Trainium chips against Nvidia while raising questions about its hardware-agnostic pitch to cloud customers. The talks remain unconfirmed and could still fall through.

<details><summary>References</summary>
<ul>
<li><a href="https://runtimewire.com/article/amazon-decart-acquisition-talks-7-billion-ai-chip-software">Amazon talks to buy Decart for $7B as chip software draws a ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/amazon-talks-acquire-ai-startup-235502420.html?fr=sycsrp_catchall">Amazon in talks to acquire AI startup Decart for $7 bln- WSJ</a></li>

</ul>
</details>

**Tags**: `#M&amp;A`, `#AI chips`, `#Amazon`, `#startups`, `#semiconductors`

---

<a id="item-finance-news-2"></a>
### [China Opens Consultation on Major Food Safety Law Revision](https://weibo.com/1642634100/Rm8MOi0jg) ⭐️ 7.0/10

China&\#x27;s market regulator opened public consultation on a draft revision of the Food Safety Law, which for the first time would bring livestream food sales and a school meal companion-dining system under regulation. The draft, a major systemic revision since the law took effect in 2009, would make school principals and kindergarten heads responsible for campus food safety and require staff to dine with students at primary and kindergarten group meals.

telegram · zaihuapd · Oct 11, 06:02

**「Background」** China&\#x27;s Food Safety Law took effect in 2009, and this draft is described as another large-scale, systemic revision. The State Administration for Market Regulation drafted it after research and soliciting opinions, and it is now open for public comment rather than enacted.

**「Impact」** If enacted, the draft would extend liability to livestream food sellers and platform operators, and require school principals and teachers to dine with students, affecting online food merchants and schools nationwide. The text remains a consultation draft, so no obligations apply yet.

<details><summary>References</summary>
<ul>
<li><a href="https://npcobserver.com/wp-content/uploads/2025/10/2025-Food-Safety-Law-Amendment_Gazette.pdf">npcobserver.com/wp-content/uploads/2025/10/2025-Food-Safety-Law...</a></li>
<li><a href="https://www.aikanai.com/fr/aikanbot/item/%E6%88%91%E5%9B%BD%E9%A3%9F%E5%93%81%E5%AE%89%E5%85%A8%E6%B3%95%E4%BF%AE%E8%AE%A2%E8%8D%89%E6%A1%88%E5%85%AC%E5%BC%80%E5%BE%81%E6%B1%82%E6%84%8F%E8%A7%81%E6%B6%89%E5%8F%8A-ai-%E7%9B%91%E7%AE%A1%E6%A0%A1%E5%9B%AD%E9%A3%9F%E5%93%81%E5%AE%89%E5%85%A8%E7%AD%89-1303">我国 食 品 安 全 法 修 订 草案公开征求意见，涉及 AI 监 管 、 校 园 食 品 安 全 等</a></li>
<li><a href="https://pub.timedg.com/a/2025-03/19/AP67dabbede4b09ef8b6dc04eb.html">事关 直 播 带 货 、 食 堂用 餐 、外卖等 食 品 安 全 ，中办、国办印发意见</a></li>

</ul>
</details>

**Tags**: `#food safety regulation`, `#China policy`, `#livestream e-commerce`, `#school meals`, `#public consultation`

---

<a id="item-finance-news-3"></a>
### [Turkey Bans Social Media Accounts for Children Under 15](https://edremit65.meb.gov.tr/www/sosyal-ag-saglayici-tarafindan-cocuklara-ozgu-ayristirilmis-hizmet-sunulmasina-ve-yas-dogrulamaya-iliskin-yonetmelik/icerik/2602/tr) ⭐️ 7.0/10

Turkey&\#x27;s presidency issued a regulation barring social media platforms from serving children under 15, requiring users aged 15 and older to verify their age through the e-Devlet \(e-government\) system. Existing accounts must complete age verification by March 31, 2027, and accounts belonging to users under 15 will be closed.

telegram · zaihuapd · Oct 11, 07:02

**「Background」** The regulation was published in Turkey&\#x27;s Official Gazette, the government&\#x27;s journal for announcing new rules, and takes effect on November 1, 2026, according to news reports citing the text.

**「Impact」** Social media platforms operating in Turkey will need to build age-verification systems linked to the e-Devlet government portal and close accounts belonging to users under 15 by March 31, 2027. Turkish users aged 15 to 17 will be routed to separate services with stricter privacy defaults, including limits on public accounts, live streaming, continuous-scroll recommendations, and personalized advertising.

<details><summary>References</summary>
<ul>
<li><a href="https://fakti.bg/en/world/1088558-turkey-bans-social-media-for-children-under-15">Turkey bans social media for children under 15 - Факти</a></li>
<li><a href="https://www.hurriyetdailynews.com/turkiye-sets-rules-for-under-15-social-media-ban-227953">Türkiye sets rules for under-15 social media ban - Türkiye News</a></li>
<li><a href="https://sypnow.com/en/news/turkey-social-media-age-ban-under-15">Turkey Bans Social Media for Under-15s - sypnow.com</a></li>
<li><a href="https://www.youtube.com/watch?v=IquZvOIn4KY">Social Media Banned for Under 15s! - What Happens Now? - YouTube</a></li>
<li><a href="https://turkishminute.com/2026/10/10/turkeys-social-media-ban-for-under-15s-takes-effect-november-1/">Turkey ’s social media ban for under-15s takes effect... - Turkish Minute</a></li>

</ul>
</details>

**Tags**: `#Turkey`, `#social media regulation`, `#child online safety`, `#age verification`, `#tech policy`

---

<a id="item-finance-news-4"></a>
### [Foreign Investors Pull About $131 Billion From Korean Stocks This Year](https://m.gelonghui.com/live/2705107) ⭐️ 7.0/10

Foreign investors have net withdrawn roughly $131 billion \(about 876.7 billion yuan\) from South Korean equities this year, according to Gelonghui. The KOSPI fell about 22% in the second half, turning from one of the year&\#x27;s best-performing major indexes into one of the worst, while trading volume dropped 70% from its late-May peak.

telegram · zaihuapd · Oct 11, 12:13

**「Background」** The Korean market is heavily concentrated in two memory-chip makers, Samsung Electronics and SK Hynix, and Samsung&\#x27;s foreign ownership has fallen to 46.38%, its lowest in about 18 years, reflecting reduced overseas confidence in Korea&\#x27;s AI-related rally even as Samsung&\#x27;s quarterly operating profit rose nearly tenfold year-on-year.

**Tags**: `#South Korea equities`, `#foreign capital flows`, `#semiconductors`, `#Samsung Electronics`, `#market selloff`

---