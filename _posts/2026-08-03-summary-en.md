---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 30 items, 7 important content pieces were selected

---

**Technology News**
1. [Karpathy highlights simple pinball prompt as LLM physical-world benchmark](#item-tech-news-1) ⭐️ 7.0/10
2. [Kakehashi: Run macOS CLI binaries on Linux ARM](#item-tech-news-2) ⭐️ 7.0/10
3. [eBay harassment campaign results in $56M payout and prison sentences](#item-tech-news-3) ⭐️ 7.0/10
4. [Open Letters Split AI Industry Over Open-Weight Model Policy](#item-tech-news-4) ⭐️ 7.0/10

**Financial News**
1. [Goldman Sachs traders on pace for record year after equities revenue jumps 72%](#item-finance-news-1) ⭐️ 8.0/10
2. [AI Chip Count Expected to Reach 200 Million by 2028](#item-finance-news-2) ⭐️ 7.0/10
3. [China proposes expanding housing provident fund to flexible workers and broader uses](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Karpathy highlights simple pinball prompt as LLM physical-world benchmark](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

A tweet by Andrej Karpathy calling attention to a simple prompt, “create a pinball game,” has sparked discussion about a new kind of benchmark for evaluating large language models’ understanding of the physical world. Frontier LLMs often generate the right components but fail to arrange them into a truly playable game, such as placing a wall in front of the launch chute, making flippers pivot the wrong way, or leaving gaps that let the ball fall past the flippers. Community commenters report that Anthropic’s Opus 5 is the first model they have seen “one shot” the prompt successfully, albeit in a specific harness. The discussion frames this as a qualitative and subjective measurement that could track future progress beyond image generation, though one commenter cautions that Anthropic models may have been specifically trained to generate three.js code, limiting what such demos prove. The tweet generated 318 comments, indicating significant community interest in using simple game-generation tasks as practical AI evaluation tools.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**「Background」** Andrej Karpathy, a prominent AI researcher and former Tesla AI director, has a history of experimenting with frontier large language models; for instance, he reportedly used Claude Opus 5 with a 1M token budget to procedurally generate a Three.js rendering of the first paragraph of The Lord of the Rings. The linked tweet appears to have sparked a community discussion about a new informal benchmark: asking LLMs to create a fully playable pinball game, which tests whether models can reason about physical constraints such as flipper orientation, launch chutes, and ball trajectories. This benchmark is seen as moving beyond image generation to expose LLMs&\#x27; deeper understanding of physical world mechanics, with community members reporting that Anthropic&\#x27;s Opus 5 is the first model they have seen &\#x27;one shot&\#x27; the task.

**「Impact」** For AI researchers and developers, the simple “create a pinball game” prompt is becoming a concrete qualitative benchmark for gauging frontier model improvement in physical reasoning, with Opus 5 the first reported model to handle it in one attempt. The benchmark’s subjective nature means results should be interpreted cautiously, especially because performance may reflect specialized training on three.js code rather than general physical-world understanding.

**「Community discussion」** Commenters largely agree that poor end products are the point, as the prompt exposes physical-world understanding better than image generation, though the measurement is qualitative and subjective. Some counterexamples and caveats emerged, including a warning that Anthropic models appear specifically trained for three.js generation, which could make their pinball demos less indicative of broader capability.

<details><summary>References</summary>
<ul>
<li><a href="https://techstacks.io/posts/18035/karpathy-s-pelican">Karpathy’s Pelican - techstacks.io</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#benchmark`, `#AI evaluation`, `#physical world`, `#frontier models`

---

<a id="item-tech-news-2"></a>
### [Kakehashi: Run macOS CLI binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi is an experimental userspace compatibility layer that aims to run macOS command-line binaries natively on Linux ARM machines. The project currently demonstrates working prototypes for 7-Zip, curl, and Xcode Tools Git: 7-Zip passes multi-threaded compression tests on an 8,000-file tree but remains about 5.2x slower than native Linux execution, while curl passes over 200 commands and options in an automated Docker test script. The developer has outlined an optimization plan to reduce the performance gap, but the project is still early and incomplete. This approach matters because it offers a potential path to running macOS CLI tools on Linux ARM without full system virtualization.

hackernews · vlad\_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**「Background」** Kakehashi is an experimental userspace translation layer that runs macOS ARM64 binaries on Linux aarch64 systems. Unlike kernel-level or full-system emulation, it loads Darwin Mach-O executables directly, provides a minimal freestanding libSystem, and translates BSD syscalls to Linux, with no JIT compilation. It is similar in spirit to the Darling project, which aims to run macOS software on Linux, but Kakehashi is CLI-first and currently focuses on simple tools like 7-Zip and curl.

**「Impact」** Developers and researchers interested in macOS-on-Linux compatibility may gain a new experimental route for ARM-based systems, though the current performance penalties and limited tool coverage mean it is not yet practical for production use.

**「Community Discussion」** Commenters drew comparisons to WINE/Proton for Windows and the existing Darling project, asking whether efforts could be combined, while others expressed long-term hopes for running macOS audio plugins on Linux, such as via a yabridge-like layer. Several acknowledged that Kakehashi is still early and are watching its progress closely.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">wie- project / kakehashi : Userspace macOS translation layer for Linux ...</a></li>

</ul>
</details>

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#compatibility`, `#open source`

---

<a id="item-tech-news-3"></a>
### [eBay harassment campaign results in $56M payout and prison sentences](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay has agreed to pay $56 million and several former members of its global security team have been sentenced to prison after orchestrating a harassment campaign against a couple who publicly criticized the company. The campaign, described as including threatening messages and surveillance, was carried out by eBay&\#x27;s security personnel in response to critical coverage by the couple. The case highlights the serious ethical and legal failures within corporate security teams and has sparked widespread discussion about accountability in the technology industry.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**「Background」** In 2019, eBay’s global security team, led by former senior executives, orchestrated a coordinated harassment and stalking campaign against Ina and David Steiner, a Massachusetts couple who published an online newsletter critical of the company. The campaign involved threatening messages, surveillance, and other intimidation tactics, leading to criminal prosecutions and guilty pleas from several involved employees. The civil lawsuit brought by the Steiners against eBay, its former CEO, and other former leaders was settled for $55.7 million, as reported by the Boston Globe and other outlets.

**「Impact」** The settlement and prison sentences establish a clear precedent that corporate security teams can face criminal liability for targeting online critics, making this a significant warning for technology companies and their employees.

**「Community Discussion」** Commenters expressed skepticism that this was an isolated incident, questioning whether eBay ran similar campaigns against other critics and whether the former police officers involved warrant further investigation. One commenter also pointedly criticized eBay&\#x27;s fee structure, noting it can amount to about 13% of a sale, though this was tangential to the main discussion.

**Tags**: `#security`, `#tech industry`, `#legal`, `#eBay`, `#ethics`

---

<a id="item-tech-news-4"></a>
### [Open Letters Split AI Industry Over Open-Weight Model Policy](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 7.0/10

Simon Willison summarizes a Microsoft-shepherded open letter dated July 24th and signed by 235 AI-adjacent companies, including NVIDIA, Amazon, Y Combinator, The Linux Foundation, and later OpenAI, opposing potential US bans or limits on open-weight models and defending distillation as a legitimate technique. Anthropic did not sign and published its own position three days later, warning about risks from authoritarian governments and industrial-scale distillation while stating it has never advocated a ban. On July 28, a separate open letter called &\#x27;Pacing the Frontier&\#x27; appeared with 1,324 employees of frontier AI companies requesting US government support for international efforts to pace automated AI development. The letters reflect growing industry clashes over open-weight model policy and the speed of frontier AI progress.

rss · Simon Willison · Aug 2, 04:16

**「Background」** Open-weight models are AI models whose trained parameters are released publicly so researchers and developers can inspect, modify, and use them, unlike closed models that are only accessible through APIs. The US government had reportedly considered restricting such models over safety concerns, and Simon Willison cites an earlier directive that suspended access to Claude Fable 5 as motivating the industry letter.

**「Impact」** The open letter and &\#x27;Pacing the Frontier&\#x27; response illustrate a concrete split among AI companies and researchers over how to govern open-weight and frontier AI, which could influence US regulatory decisions on model release and distillation.

**Tags**: `#AI policy`, `#open weights`, `#open source`, `#Microsoft`, `#industry`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Goldman Sachs traders on pace for record year after equities revenue jumps 72%](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 8.0/10

Goldman Sachs reported a 72% jump in equities trading revenue to a record $7.42 billion in the second quarter, putting its trading desks on pace for a record year. The figure is an actual reported result and was the biggest driver of the bank&\#x27;s performance.

rss · CNBC Finance · Aug 2, 13:52

**「Background」** Equities trading is part of Goldman&\#x27;s Global Banking &amp; Markets division, its largest, which brought in $15.5 billion in revenue last quarter — more than 75% of the bank&\#x27;s total.

**「Impact」** The strong showing is part of a broader trend: the report says many other top Wall Street banks are also on track for their best year ever in trading revenue.

**Tags**: `#Goldman Sachs`, `#earnings`, `#trading revenue`, `#investment banking`, `#financial sector`

---

<a id="item-finance-news-2"></a>
### [AI Chip Count Expected to Reach 200 Million by 2028](https://www.nytimes.com/interactive/2026/07/29/technology/ai-chips-data-center-boom.html) ⭐️ 7.0/10

The global AI chip count is expected to grow from about 20 million today to roughly 200 million by the end of 2028, doubling about every nine months, according to Epoch AI; separately, IDC forecasts worldwide AI infrastructure investment will surpass $1 trillion in 2029, up from $318 billion a year earlier.

telegram · zaihuapd · Aug 2, 01:01

**「Background」** These figures come from technology-research firm Epoch AI, which publishes open data on AI chip sales and computing trends, and from market-research firm IDC, which tracks quarterly AI infrastructure spending.

**「Impact」** The rapid buildout is already linked to higher electricity prices and environmental disputes, and economists cited in the report warn that spending may outpace profits.

<details><summary>References</summary>
<ul>
<li><a href="https://epoch.ai/data">Data on the Trajectory of AI | Epoch AI Database</a></li>
<li><a href="https://epoch.ai/data/ai-chip-sales">Data on AI Chip Sales | Epoch AI</a></li>
<li><a href="https://www.idc.com/resource-center/blog/ai-infrastructure-spending-caps-historic-year-at-90-billion-in-q4-2025-2029-spending-to-eclipse-1-trillion/">IDC - AI Infrastructure Spending Caps Historic Year at ~$90 Billion in Q4 2025; 2029 Spending to Eclipse $1 Trillion</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#data center investment`, `#Epoch AI`, `#IDC forecast`, `#technology infrastructure`

---

<a id="item-finance-news-3"></a>
### [China proposes expanding housing provident fund to flexible workers and broader uses](https://weibo.com/1642634100/RbwfKezfq) ⭐️ 7.0/10

China’s housing authority has published a draft revision of the housing provident fund rules for public comment, proposing that flexible workers such as self-employed people, delivery riders and ride-hailing drivers can voluntarily contribute, and that withdrawals can cover renovation and property fees, not just home purchase or rent.

telegram · zaihuapd · Aug 2, 06:32

**「Background」** The housing provident fund is a state-managed housing savings scheme; existing rules generally focus on salaried employees and limit withdrawals largely to buying or renting a home.

**「Impact」** If adopted, the changes would let non-salaried workers build up housing savings and allow existing savers to use their funds for renovation and property maintenance.

**Tags**: `#housing provident fund`, `#policy revision`, `#flexible employment`, `#housing consumption`, `#China`

---