---
layout: default
title: "Horizon Summary: 2026-08-18 (EN)"
date: 2026-08-18
lang: en
---

> From 197 items, 10 important content pieces were selected

---

**Technology News**
1. [Mojo Programming Language Goes Open Source](#item-tech-news-1) ⭐️ 9.0/10
2. [GitLab 紧急修复严重漏洞，可未授权删除项目](#item-tech-news-2) ⭐️ 9.0/10
3. [Linux 7.3 Boosts VRAM Overcommit Performance](#item-tech-news-3) ⭐️ 8.0/10
4. [Qwen 3.8 27B Matches GPT-5.6 Luna on AI Index](#item-tech-news-4) ⭐️ 8.0/10
5. [Asana completes 5 years of engineering work in 2 weeks with Codex](#item-tech-news-5) ⭐️ 8.0/10
6. [Rust GPU Offload Framework: Safe, Portable, Fast](#item-tech-news-6) ⭐️ 8.0/10
7. [China Orders Early Removal of Custom Windows 10 from Agencies](#item-tech-news-7) ⭐️ 8.0/10

**Technology Blog**
1. [The Benchmarkpocalypse](#item-tech-blog-1) ⭐️ 9.0/10
2. [Unbricking a Framework Laptop with a $20 Tool](#item-tech-blog-2) ⭐️ 8.0/10
3. [CSS Bombs in Email: Client-Side Attacks](#item-tech-blog-3) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Mojo Programming Language Goes Open Source](https://www.modular.com/blog/mojo-open-source) ⭐️ 9.0/10

Modular has open-sourced the Mojo programming language, releasing its compiler and toolchain under the Apache 2 license. This follows the release of Mojo 1.0 last week and fulfills a promise made in May 2023. Originally intended as a superset of Python, Mojo has evolved into its own language optimized for GPU programming with Python-inspired syntax, though not fully compatible with existing Python code. The open-sourcing is a significant milestone for the AI/ML ecosystem, potentially accelerating adoption and community contributions.

rss · Lobsters · Aug 18, 16:34

**「Background」** Mojo is a programming language developed by Modular Inc., designed for AI and machine learning workloads with a focus on high performance and GPU programming. It was first announced in May 2023 with the goal of being a superset of Python, allowing existing Python code to run directly. However, around August 2025, Modular revised this vision, stating that Mojo may not become a full superset of Python, and instead positioned it as its own language with Python-inspired syntax. In March 2024, Modular had already open sourced the Mojo standard library under the Apache 2.0 license, but the compiler and toolchain remained proprietary until now.

**「Impact」** Developers and organizations in the AI/ML space can now freely use, modify, and contribute to Mojo, potentially accelerating its adoption and ecosystem growth. The Apache 2 license permits commercial use, which may encourage enterprise adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_%28programming_language%29">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.modular.com/blog/mojo-open-source">Modular: Mojo🔥 is now open source!</a></li>

</ul>
</details>

**Tags**: `#programming-languages`, `#ai`, `#open-source`, `#mojo`, `#machine-learning`

---

<a id="item-tech-news-2"></a>
### [GitLab 紧急修复严重漏洞，可未授权删除项目](https://www.ithome.com/0/991/362.htm) ⭐️ 9.0/10

GitLab 于 2026 年 8 月 17 日发布紧急安全更新，修复了社区版（CE）和企业版（EE）中的两个漏洞。其中严重漏洞 CVE-2026-19478（CVSS 评分 9.4）允许未认证攻击者通过单个恶意请求远程修改或删除公共项目及用户数据，甚至停用或封禁用户账号，可能引发供应链攻击；高危漏洞 CVE-2026-19650（CVSS 评分 7.1）是 GraphQL 多路复用查询处理器中的 CSRF 漏洞，允许通过 GET 请求执行变更操作，但需要用户交互。两个漏洞影响 GitLab CE/EE 从 18.2 至 18.11.11 之前、19.0 至 19.0.8 之前、19.1 至 19.1.6 之前、以及 19.2 至 19.2.4 之前的所有版本，修复版本为 19.2.4、19.1.6、19.0.8 和 18.11.11。官方强烈建议所有自托管实例立即升级。目前 PoC 和技术细节已公开，据奇安信鹰图资产测绘平台数据，国内风险资产总数为 108658 个，全球风险资产总数为 401607 个。官方尚未发现漏洞被在野利用的证据。

rss · IT HOME · Aug 18, 15:52

**「Background」** GitLab is a widely used DevOps platform that provides source code management, CI/CD, and project collaboration features. It is available in a self-hosted Community Edition \(CE\) and Enterprise Edition \(EE\). GraphQL is an API query language used by GitLab to allow clients to request and manipulate data. The vulnerability CVE-2026-19478 is a code injection flaw in the GraphQL layer, specifically in the handling of the @gl\_introduced directive, which can be exploited by an unauthenticated attacker to modify or delete public projects and user data.

**「Impact」** Self-hosted GitLab CE/EE instances running versions 18.2 through 18.11.10, 19.0 through 19.0.7, 19.1 through 19.1.5, or 19.2 through 19.2.3 are exposed to unauthenticated attackers who can delete or modify public projects and user data, potentially enabling supply-chain attacks on open-source projects. With over 400,000 at-risk instances globally \(including more than 108,000 in China\) and public PoC details, immediate upgrade to 19.2.4, 19.1.6, 19.0.8, or 18.11.11 is critical; no in-the-wild exploitation has been confirmed yet.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/gitlab-graphql-vulnerability/">Critical GitLab GraphQL Vulnerability Allow Attackers to ...</a></li>
<li><a href="https://app.opencve.io/cve/CVE-2026-19478">CVE-2026-19478 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://threataft.com/articles/gitlab-graphql-code-injection-data-manipulation-cve-2026-19478">CVE-2026-19478 — Critical GitLab GraphQL Vulnerability ...</a></li>
<li><a href="https://www.securityweek.com/gitlab-patches-critical-code-injection-vulnerability/">GitLab Patches Critical Code Injection Vulnerability</a></li>
<li><a href="https://cybersecuritynews.com/gitlab-graphql-vulnerability/">Critical GitLab GraphQL Vulnerability Allow Attackers to ...</a></li>
<li><a href="https://www.techtimes.com/articles/324811/20260818/gitlab-emergency-patch-third-graphql-flaw-2026-lets-unauthenticated-attackers-delete-projects.htm">GitLab Emergency Patch: Third GraphQL Flaw of 2026 Lets ...</a></li>

</ul>
</details>

**Tags**: `#GitLab`, `#security`, `#CVE`, `#vulnerability`, `#supply chain`

---

<a id="item-tech-news-3"></a>
### [Linux 7.3 Boosts VRAM Overcommit Performance](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux kernel version 7.3 introduces performance improvements for VRAM overcommit, addressing GPU memory pressure issues. The update enhances handling of memory allocation when VRAM is exhausted, which is critical for GPU-intensive workloads. While specific technical details are not provided in the source, the improvement is expected to reduce performance degradation during memory pressure. This development follows the recent release of 7.2, which included other performance and gaming-related enhancements. The community anticipates the upstreaming of these changes, though Nvidia users note that their drivers currently lack paging support.

hackernews · flaburgan · Aug 18, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49342719)

**「Background」** VRAM overcommit occurs when applications, especially games, request more video memory than physically available on the GPU. Traditionally, the Linux kernel would either fail the allocation or rely on swapping to system RAM, which could cause severe performance degradation or crashes. The upcoming Linux 7.3 kernel includes patches from developer Vock that improve VRAM management by allowing the kernel to handle overcommit more gracefully, reducing the performance hit when GPU memory limits are exceeded. This work builds on earlier efforts to enhance video memory management in the Linux GPU driver stack.

**「Impact」** Linux users running GPU-intensive applications, such as machine learning or gaming, will experience smoother performance when VRAM is fully utilized, reducing stutters and crashes. However, Nvidia users may not benefit immediately due to lack of paging support in their drivers.

**「Community Discussion」** Commenters praise the improvement and express enthusiasm for upcoming kernel releases, contrasting with negative sentiment toward Windows updates. Some share the author&\#x27;s view that applications should inform the kernel about VRAM stickiness, and others hope for similar fixes for system RAM exhaustion. Nvidia users highlight ongoing VRAM paging limitations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management ...</a></li>
<li><a href="https://www.nitin-rachabathuni.com/blog/linux-kernel-vram-overcommit-performance">Optimizing VRAM Overcommit: How Linux Kernel Improvements ...</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM</a></li>

</ul>
</details>

**Tags**: `#linux`, `#kernel`, `#vram`, `#gpu`, `#performance`

---

<a id="item-tech-news-4"></a>
### [Qwen 3.8 27B Matches GPT-5.6 Luna on AI Index](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B, a compact 27-billion-parameter model, scored 52 on the Artificial Analysis Intelligence Index, matching the score of GPT-5.6 Luna \(max\) and trailing just one point behind GLM-5.2 \(max\) and DeepSeek V4 Pro 0813 \(max\). The GLM-5.2 model has 753B parameters and DeepSeek V4 Pro 0813 has 1.7T parameters, while Luna&\#x27;s size is unknown but presumably much larger than 27B. This achievement highlights the efficiency of smaller models, as Qwen 3.8 27B delivers competitive performance despite its relatively small size. The result was reported by Simon Willison, who described the model as &\#x27;a truly astonishing model&\#x27; in a previous post.

rss · Simon Willison · Aug 17, 23:58

**「Background」** The Artificial Analysis Intelligence Index is a benchmark that measures the overall intelligence of AI models across various tasks. Qwen 3.8 27B is a 27-billion-parameter dense, open-weight vision-language model from Alibaba&\#x27;s Qwen family, designed for coding, professional work, research, and long-horizon agentic tasks, with a native 262K-token context window. It is part of the Qwen3.8 generation, which emphasizes deployment-friendly size while maintaining strong performance.

**「Impact」** This benchmark result suggests that organizations and developers can achieve frontier-level AI performance with significantly smaller and more cost-effective models, potentially reducing the computational resources and costs required for deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers-ai/models/qwen3.8-27b/">qwen3.8-27b (Qwen) · Cloudflare AI docs · Cloudflare Workers ...</a></li>
<li><a href="https://www.jetson-ai-lab.com/models/qwen3-8-27b/">Qwen3.8 27B - Jetson AI Lab</a></li>
<li><a href="https://lmstudio.ai/models/qwen3.8">Qwen3.8 - lmstudio.ai</a></li>

</ul>
</details>

**Tags**: `#qwen`, `#llm`, `#benchmark`, `#ai`, `#efficiency`

---

<a id="item-tech-news-5"></a>
### [Asana completes 5 years of engineering work in 2 weeks with Codex](https://openai.com/index/asana) ⭐️ 8.0/10

Asana used OpenAI Codex to replace an outdated testing system in just two weeks, completing work that was expected to take five years, at a cost of about $12,000. This case study highlights the significant productivity gains possible with AI coding tools in a real engineering organization. The project involved modernizing a legacy testing infrastructure, a task that would have required substantial manual effort. The success demonstrates the potential for AI-assisted development to accelerate large-scale refactoring and system upgrades. However, it is a specific case study rather than a general benchmark, and results may vary depending on the complexity and context of the engineering work.

rss · OpenAI Blog · Aug 18, 07:00

**「Background」** Asana is a work management platform that relies on a large codebase, and its testing system had become outdated, requiring significant maintenance and slowing down development. OpenAI Codex is an AI coding tool that can generate and modify code based on natural language prompts, enabling developers to automate repetitive and complex coding tasks. This case study illustrates how AI tools can be applied to legacy system modernization, a common challenge in software engineering.

**「Impact」** For Asana, this project saved an estimated five years of engineering time and reduced costs to about $12,000, likely freeing up developers to focus on higher-value work. For the broader software engineering community, it provides a concrete example of AI coding tools&\#x27; potential to accelerate large-scale refactoring, though the generalizability to other organizations and codebases remains uncertain.

**Tags**: `#AI coding`, `#OpenAI Codex`, `#software engineering`, `#productivity`, `#case study`

---

<a id="item-tech-news-6"></a>
### [Rust GPU Offload Framework: Safe, Portable, Fast](https://arxiv.org/pdf/2608.13759) ⭐️ 8.0/10

A new paper introduces a zero-overhead, multi-vendor GPU compilation framework built natively into the Rust compiler \(rustc\) and LLVM backends. It leverages Rust&\#x27;s type system, ownership model, and strict aliasing guarantees \(noalias\) to manage and optimize data transfers through LLVM&\#x27;s Offload infrastructure. The framework addresses cross-vendor ABI lowering mismatches between host and device targets with a two-pass compilation pipeline that safely handles both manual and compiler-generated memory movements. Evaluated on RAJAPerf, the rustc-based solution generates competitive LLVM IR for GPU kernels, achieving solid kernel performance against native, hand-optimized CUDA and HIP C++ baselines. This work offers a novel approach to combining memory safety with high-performance GPU programming without vendor lock-in.

rss · Lobsters · Aug 18, 12:16

**「Background」** Traditional GPU programming requires a trade-off between execution efficiency and memory safety. While Rust provides compile-time memory safety for host CPUs through its ownership model, applying these guarantees to massively parallel GPU environments has previously required vendor-locked domain-specific languages \(DSLs\) or explicit unsafe raw pointers. This paper presents a framework that integrates GPU offloading directly into rustc and LLVM, aiming to provide safety and portability without performance penalties.

**「Impact」** This framework could enable Rust developers to write safe, portable GPU kernels that perform comparably to hand-optimized CUDA and HIP C++ code, potentially reducing the need for vendor-specific DSLs and unsafe code in GPU computing. The integration into rustc and LLVM suggests it may influence future Rust GPU development and adoption in high-performance computing.

**Tags**: `#Rust`, `#GPU programming`, `#compilers`, `#LLVM`, `#memory safety`

---

<a id="item-tech-news-7"></a>
### [China Orders Early Removal of Custom Windows 10 from Agencies](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 8.0/10

China&\#x27;s Ministry of State Security has ordered some government-affiliated agencies to uninstall a customized version of Windows 10 ahead of schedule, moving up the planned discontinuation from February 2027 by several months. The directive stems from data security concerns, though specific vulnerabilities were not disclosed. Microsoft stated it has found no security incidents affecting the product and that it continues to receive regular security updates. This action affects Microsoft&\#x27;s presence in Chinese government sectors and underscores rising data security scrutiny.

telegram · zaihuapd · Aug 18, 06:22

**「Background」** China&\#x27;s Ministry of State Security has ordered some government-linked agencies to uninstall a customized version of Windows 10, known as the Government Edition, ahead of the originally planned retirement in February 2027. The directive reportedly stems from data security concerns, though no specific vulnerabilities were disclosed. Microsoft has stated that it has not found any security incidents affecting the product and that it continues to receive regular security updates. This move is part of a broader trend of China reducing reliance on foreign technology in government and state-linked sectors.

**「Impact」** Affected Chinese government agencies must accelerate migration away from the customized Windows 10, potentially disrupting operations and increasing reliance on domestic alternatives. The move may also signal broader regulatory pressure on foreign software in China, affecting Microsoft&\#x27;s government business.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/operating-systems/china-reportedly-orders-state-agencies-to-uninstall-its-government-only-edition-of-windows-10">China reportedly orders state agencies to uninstall its government-only edition of Windows 10 — Beijing accelerates planned retirement over data security concerns | Tom&#x27;s Hardware</a></li>
<li><a href="https://thenextweb.com/news/china-removes-microsoft-windows-10-state-agencies">China is removing Microsoft’s Windows 10 from state agencies</a></li>
<li><a href="https://wccftech.com/china-state-agencies-uninstall-windows-10-cmit-government-edition/">China’s State-Linked Firms Are Moving Away From Windows 10 Due To Security Concerns, Despite The Custom OS Developed By Microsoft Under Stringent Supervision</a></li>

</ul>
</details>

**Tags**: `#China`, `#Windows 10`, `#government policy`, `#data security`, `#Microsoft`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [The Benchmarkpocalypse](https://danluu.com/benchpocalypse/) ⭐️ 9.0/10

rss · Lobsters · Aug 18, 00:47

**「Background」** In the tech industry, benchmarks are often treated as objective measures of performance, guiding decisions from library selection to system design. However, Dan Luu argues that this over-reliance on benchmarks can distort engineering priorities, leading teams to optimize for metrics that don&\#x27;t reflect real-world usage or user value.

**「Solution」** Luu illustrates how benchmarks can be gamed or become outdated, citing examples where optimizing for a benchmark led to worse real-world performance. He suggests that instead of blindly trusting benchmarks, engineers should understand what they actually measure, consider the workload they represent, and validate results against realistic scenarios. He advocates for a more nuanced approach that combines benchmarks with profiling, load testing, and domain-specific reasoning, emphasizing that benchmarks are tools, not truths.

**「Takeaway」** The core thesis is that benchmarks, while useful, are often misused and can lead to misaligned incentives and overfitting. Engineers should treat them with skepticism and complement them with contextual evaluation to make better technical decisions.

**Tags**: `#benchmarks`, `#engineering culture`, `#incentives`, `#evaluation`, `#critical thinking`

---

<a id="item-tech-blog-2"></a>
### [Unbricking a Framework Laptop with a $20 Tool](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 8.0/10

hackernews · Lobsters · Aug 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49345220)

**「Background」** A Framework laptop with an AMD 7040-series processor can become bricked by a faulty BIOS update, leaving the device unusable. The author faced this problem and found that official support offered little help, prompting a search for a practical recovery method.

**「Solution」** The author successfully recovered the laptop using a $20 SPI flash programmer, a common and inexpensive tool. The process involved disassembling the laptop to access the SPI flash chip, connecting the programmer, and rewriting the firmware. The article provides detailed steps, including identifying the correct chip and using open-source software to flash the backup. The author notes that this approach requires technical skill and carries risks, such as potential damage to the chip or motherboard. They also discuss alternatives like sending the laptop to a repair service, but highlight the cost and time savings of DIY recovery. The success demonstrates that many bricked laptops can be revived with the right tools and knowledge, even when manufacturer support is lacking.

**「Takeaway」** The author concludes that with modest investment and technical effort, users can recover from firmware failures that would otherwise render a laptop e-waste, underscoring the value of repair skills and the need for better vendor support.

**Tags**: `#Framework laptop`, `#BIOS recovery`, `#SPI flash`, `#firmware`, `#hardware repair`

---

<a id="item-tech-blog-3"></a>
### [CSS Bombs in Email: Client-Side Attacks](https://portswigger.net/research/css-the-bomb-inside-your-inbox) ⭐️ 8.0/10

rss · Lobsters · Aug 18, 13:30

**「Background」** Email clients render HTML and CSS, which opens a door for attackers to exploit CSS features for malicious purposes. Traditional defenses focus on server-side filtering, but the author argues that CSS itself can be weaponized to exfiltrate data or manipulate the user interface, posing a significant risk to email security.

**「Solution」** The author demonstrates how CSS can be abused in email clients to perform data exfiltration and UI redressing attacks. By using CSS selectors and attribute selectors, attackers can infer sensitive information from the rendered page, such as the presence of certain elements or values. For example, they can craft CSS rules that make network requests based on the state of the page, leaking data to an external server. Additionally, CSS can be used to overlay fake UI elements, tricking users into clicking malicious links. The author provides practical examples and explains the underlying mechanisms, showing how these attacks bypass traditional security measures. They also discuss limitations, such as the need for user interaction or specific email client configurations, and suggest mitigations like disabling remote content or using stricter CSS parsing.

**「Takeaway」** The author concludes that CSS is a powerful attack vector in email clients, capable of compromising user privacy and security. They emphasize the need for email clients to adopt stricter CSS handling and for users to be aware of the risks, as these attacks are practical and can be executed with minimal user interaction.

**Tags**: `#CSS`, `#email security`, `#client-side attacks`, `#web security`, `#exploitation`

---