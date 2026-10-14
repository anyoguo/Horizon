---
layout: default
title: "Horizon Summary: 2026-10-14 (EN)"
date: 2026-10-14
lang: en
---

> From 138 items, 25 important content pieces were selected

---

**Technology News**
1. [Google releases Gemini 4 Argon for robotics with 87% ERQA score](#item-tech-news-1) ⭐️ 9.0/10
2. [Anthropic replaces Git with custom Scion version control system](#item-tech-news-2) ⭐️ 9.0/10
3. [11-year-old unsoundness bug found in Rust borrow checker](#item-tech-news-3) ⭐️ 8.0/10
4. [AWS Lambda Web Functions launch for low-latency HTTP handling](#item-tech-news-4) ⭐️ 8.0/10
5. [China&\#x27;s MOHRSS Launches &\#x27;AI Adaptation Employment Action&\#x27; Policy](#item-tech-news-5) ⭐️ 8.0/10
6. [Top AI Researchers Launch RSI Startups Amid $30B+ in Six-Month Funding](#item-tech-news-6) ⭐️ 8.0/10
7. [Character.AI files Chapter 11, Disney bids $20M for non-exclusive IP license](#item-tech-news-7) ⭐️ 8.0/10
8. [Unitree&\#x27;s Wang Xingxing: Biggest Past Mistake Was Underestimating AI](#item-tech-news-8) ⭐️ 8.0/10
9. [First Stargardt patient implanted with PRIMA visual prosthesis reads words post-surgery](#item-tech-news-9) ⭐️ 8.0/10

**Financial News**
1. [Visa Approved to Solely Prepare China&\#x27;s Bank Card Clearing Institution](#item-finance-news-1) ⭐️ 9.0/10
2. [Hong Kong Regulator Freezes $4.38B in Assets Amid Tea百道 IPO Manipulation Probe](#item-finance-news-2) ⭐️ 9.0/10
3. [China&\#x27;s Solar Industry: Largest Installed Capacity, Largest Losses](#item-finance-news-3) ⭐️ 8.0/10
4. [Chinese NEV Makers Shift from Exporting Cars to Building Local Operations in Latin America](#item-finance-news-4) ⭐️ 8.0/10
5. [US drug price controls reshape China biotech valuations](#item-finance-news-5) ⭐️ 8.0/10
6. [Nanyang Rural Commercial Banks Accused of Systemic &\#x27;Loan-Back&\#x27; Fraud Targeting Elderly Farmers](#item-finance-news-6) ⭐️ 7.0/10
7. [China&\#x27;s AI Models Face Low C-End Pay Rates but Gain in B/G-End and Cost Advantages](#item-finance-news-7) ⭐️ 7.0/10
8. [Thailand Plans 15% Civil Service Cut by 2032](#item-finance-news-8) ⭐️ 7.0/10
9. [海底捞向控股股东张勇提供1亿元短期贷款](#item-finance-news-9) ⭐️ 7.0/10
10. [Why Blaming Real Estate for All Economic Problems Is Misplaced](#item-finance-news-10) ⭐️ 7.0/10
11. [China&\#x27;s supermarket private labels hit 380 billion yuan in 2025](#item-finance-news-11) ⭐️ 7.0/10
12. [Shenzhen&\#x27;s Role in &\#x27;Guangdong Cars Going South&\#x27; Policy](#item-finance-news-12) ⭐️ 7.0/10
13. [China&\#x27;s Wind and Solar Installation Slows Sharply in First Half of 2026](#item-finance-news-13) ⭐️ 7.0/10
14. [China-EU Hybrid Car Trade Deal Clarified](#item-finance-news-14) ⭐️ 7.0/10
15. [European Pharma Executives Demand Policy Reform Amid Innovation Decline](#item-finance-news-15) ⭐️ 7.0/10
16. [Campus Stores Boost Coffee/Tea Chain Sales Amid Industry-Wide Contraction](#item-finance-news-16) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Google releases Gemini 4 Argon for robotics with 87% ERQA score](https://developers.googleblog.com/gemini-4-argon-for-robotics/) ⭐️ 9.0/10

Google has released Gemini 4 Argon, a new multimodal model optimized for physical reasoning and robotics, achieving 87% on the embodied reasoning benchmark ERQA. It is available globally via the Gemini API and Gemini App for Pro+ and Ultra subscribers, and in Antigravity for Ultra users; it integrates with Boston Dynamics Spot robots and is accessible through the google-genai SDK. Pricing is $2 per million input tokens and $10 per million output tokens. The model improves real-robot task success rate from 56% to 75% and reduces average task time from 35 seconds to 24 seconds.

telegram · zaihuapd · Oct 13, 16:08

**「Background」** Gemini 4 Argon is the latest iteration in Google&\#x27;s Gemini series of multimodal foundation models, succeeding earlier versions such as Gemini 1.5 and Gemini 2.0 that emphasized long-context understanding and general-purpose reasoning. Unlike prior Gemini releases focused on broad language and vision tasks, Argon is explicitly designed for embodied AI—integrating physical reasoning, real-world robot control, and simulation-aware code generation.

**「Impact」** Developers building robotic systems now have a production-ready, API-accessible model that demonstrably improves real-world task performance on Spot robots—requiring no custom training but demanding integration with Google’s SDK and budgeting for its relatively high output-token cost.

**「Community discussion」** Commenters highlight Argon’s exceptional clarity and structured prose—calling it &\#x27;not RL-fried&\#x27; and praising its simulation-building behavior—while one user notes its image-to-HTML capability is &\#x27;B tier&\#x27;, below GPT-6.1 Sol but above some contemporaries; another observes its cost-per-task is significantly higher than alternatives despite comparable intelligence gains.

**Tags**: `#artificial-intelligence`, `#robotics`, `#multimodal-models`, `#google-deepmind`, `#embodied-ai`

---

<a id="item-tech-news-2"></a>
### [Anthropic replaces Git with custom Scion version control system](https://www.anthropic.com/engineering/redesigning-source-control) ⭐️ 9.0/10

Anthropic has fully replaced Git with its internally built, server-driven version control system Scion across its main codebase, completing the migration within five months from May to September 2026. Scion reduces CPU and memory usage to 1/200 of the prior Git-based infrastructure, accelerates CI detection by ~100×, and cuts CI compute usage by 25%. Daily merges increased from ~2,500 in May 2026 to over 30,000 in September 2026, managed by a team of seven engineers.

telegram · zaihuapd · Oct 14, 02:30

**「Background」** Git is a widely adopted, distributed version control system originally designed for human-paced collaborative development. Anthropic’s shift to Scion was driven by an order-of-magnitude increase in merge volume—fueled in part by AI-assisted coding from Claude—which exposed scalability limits in their existing Git-based infrastructure.

**「Impact」** Anthropic engineers now experience ~100× faster CI detection and use 1/200 the CPU and memory previously required for Git operations, enabling a five-month scaling of daily merges from ~2,500 to &gt;30,000—though this requires ongoing maintenance of a custom VCS instead of relying on widely supported, battle-tested tooling.

**「Community discussion」** Some commenters question the necessity of replacing Git—citing available optimization paths between vanilla Git and a ground-up rewrite—while others frame the shift as emblematic of changing engineering tradeoffs under AI-augmented development, where custom tooling costs may decrease relative to adaptation effort.

<details><summary>References</summary>
<ul>
<li><a href="https://officechai.com/ai/anthropic-builds-in-house-version-of-git-called-scion-after-code-merges-rise-12x-in-4-months/">Anthropic Builds In-house Version Of Git Called Scion After ...</a></li>

</ul>
</details>

**Tags**: `#version-control`, `#infrastructure`, `#ai-engineering`, `#distributed-systems`

---

<a id="item-tech-news-3"></a>
### [11-year-old unsoundness bug found in Rust borrow checker](https://github.com/rust-lang/rust/issues/164250) ⭐️ 8.0/10

An 11-year-old unsoundness bug in Rust&\#x27;s borrow checker was disclosed in issue \#164250, allowing code that violates lifetime rules to compile without error. The bug resides in the compiler’s implementation—not the formal type system—and affects all Rust versions since at least 2015; it is now confirmed fixed in nightly Rust as of October 2026. The fix involves tightening borrow checking logic to reject the previously accepted unsafe pattern, with no change to Rust’s lifetime semantics or stable language guarantees.

hackernews · formerly\_proven · Oct 13, 10:27 · [Discussion](https://news.ycombinator.com/item?id=50069499)

**「Rust&\#x27;s borrow checker and unsoundness issues」** Rust’s borrow checker enforces memory safety at compile time by statically verifying that references do not outlive the data they point to, based on lifetime annotations and ownership rules. Since Rust 1.0 \(2015\), the compiler has maintained a list of known unsoundness bugs—instances where it incorrectly accepts code that violates these rules—many of which have persisted for years due to complexity in the trait solver and borrow-checker implementation. The issue referenced \(rust-lang/rust\#164250\) is one such long-standing case, classified under the &\#x27;I-unsound&\#x27; label used to track violations of memory safety guarantees.

**「Impact」** The bug allows field assignment to bypass a struct’s lifetime bounds, enabling code that should be rejected by the borrow checker to compile and potentially execute with undefined behavior; fixing it may break existing crates that rely on the unsound behavior, though no widespread breakage has been reported yet.

**「Community discussion」** Commenters note that while the bug is longstanding, it reflects a known class of ~100 labeled unsoundness issues in Rust’s issue tracker, some of which may be unblocked for fixing by the new trait solver; others emphasize that real-world impact remains unclear, as no affected crates have yet been reported to break upon the fix.

<details><summary>References</summary>
<ul>
<li><a href="https://braindetox.kr/en/posts/rust_borrow_checker_soundness_bugs_11_years_2026.html">Rust #164250: Borrow Checker Unsoundness Open Since 1.4</a></li>

</ul>
</details>

**Tags**: `#rust`, `#memory-safety`, `#type-systems`, `#compiler-bugs`, `#programming-languages`

---

<a id="item-tech-news-4"></a>
### [AWS Lambda Web Functions launch for low-latency HTTP handling](https://aws.amazon.com/blogs/aws/announcing-aws-lambda-web-functions-for-fast-consistent-web-app-performance-anywhere/) ⭐️ 8.0/10

AWS launched Lambda Web Functions, a new execution mode for Lambda that handles HTTP requests natively without requiring API Gateway or Application Load Balancer as intermediaries. It is available in all AWS Regions where Lambda runs, supports existing Lambda runtimes \(Node.js, Python, Java, .NET, Ruby, Go, and custom runtimes\), and includes built-in request/response serialization and automatic binary support. The feature is generally available as of the October 13, 2026 announcement, and integrates with existing Lambda tooling, CI/CD pipelines, and permissions models—no code rewrite is required to adopt it for compatible workloads.

hackernews · HatchedLake721 · Oct 13, 10:07 · [Discussion](https://news.ycombinator.com/item?id=50069318)

**「Prerequisite: AWS Lambda and API Gateway architecture」** AWS Lambda has historically required an external HTTP front-end—most commonly Amazon API Gateway or Application Load Balancer—to expose functions as web endpoints, adding latency, configuration complexity, and cost. Lambda’s original design treats functions as stateless compute units triggered by events \(e.g., S3 uploads, SQS messages\), not as long-lived HTTP servers; request handling relied on serialization/deserialization layers outside the function runtime.

**「Who is affected and how」** Developers building HTTP APIs on Lambda can now reduce median latency by eliminating API Gateway proxy overhead and achieve more consistent cold-start behavior for web workloads; those using Function URLs or ALB integrations may need to evaluate migration paths, as Web Functions introduce a new handler contract and require minor code adjustments to use the native HTTP event format.

**「Key community perspectives」** Commenters noted competitive pressure from Cloudflare Workers and questioned AWS’s choice to deepen code-centric serverless rather than push containers further, while others highlighted real-world cost and operational simplicity benefits—especially for small-scale backends that previously relied on Function URLs + CloudFront.

**Tags**: `#serverless`, `#aws`, `#web-development`, `#cloud-computing`, `#lambda`

---

<a id="item-tech-news-5"></a>
### [China&\#x27;s MOHRSS Launches &\#x27;AI Adaptation Employment Action&\#x27; Policy](https://www.huxiu.com/article/4897385.html?f=rss) ⭐️ 8.0/10

China&\#x27;s Ministry of Human Resources and Social Security \(MOHRSS\) has launched the &\#x27;Adaptation to Artificial Intelligence Development for Employment Promotion Action&\#x27;, formally acknowledging that AI-driven labor displacement is already occurring—not merely a future risk. The policy introduces mandatory &\#x27;AI literacy for all workers&\#x27;, requires pre-deployment employment impact assessments for major AI projects, and targets 10 million annual subsidized vocational training slots and 40 million new skill certifications over the 2026–2030 &\#x27;15th Five-Year Plan&\#x27; period. It responds directly to observed labor market shifts: editing, customer service, and graphic design job postings fell 29%, 23%, and 21% year-on-year in Q1 2026, while AI-related roles \(e.g., AI product managers, engineers, trainers\) grew 73–81%. The policy does not guarantee job preservation but institutionalizes reskilling as a national priority with concrete metrics and accountability mechanisms.

rss · 虎嗅 · Oct 14, 04:30

**「Background」** This action follows years of China&\#x27;s &\#x27;stabilize employment&\#x27; \(wen jiuye\) policy framework focused on aggregate job creation and unemployment rate control; the explicit addition of &\#x27;adaptation to AI&\#x27; marks a strategic pivot toward managing structural labor reallocation driven by automation. It builds on earlier MOHRSS initiatives like the 2021 &\#x27;Digital Skills Training Program&\#x27; but significantly escalates scope, mandate, and integration with investment decision-making—requiring formal employment impact assessments for major projects, a new procedural requirement.

**「Impact」** Entry-level job seekers—including recent graduates and career switchers—face sharply reduced opportunities in AI-affected fields like machine learning \(−71.43% demand for &lt;1-year experience roles in Jan–May 2026\) and software testing \(−52.94%\), making foundational work experience harder to obtain without prior AI-augmented skills.

**「Community Discussion」** No community comments were available for analysis.

**Tags**: `#artificial-intelligence`, `#labor-economics`, `#public-policy`, `#software-engineering-impact`

---

<a id="item-tech-news-6"></a>
### [Top AI Researchers Launch RSI Startups Amid $30B+ in Six-Month Funding](https://www.huxiu.com/article/4897378.html?f=rss) ⭐️ 8.0/10

Over the past six months, elite AI researchers from DeepMind, Meta, OpenAI, Anthropic, and Google have founded startups focused on Recursive Self-Improvement \(RSI\), raising over $30 billion in funding—$50 billion if counted from年初 2026. Notable examples include Recursive Superintelligence \($650M\), Discovery Loop \($1B\), Ineffable Intelligence \($1.1B\), and超衍智能 \(¥400M in ~3 months\). These companies have no shipped products or verified RSI闭环; valuations are speculative \(e.g., Mirendil reportedly negotiating a $5B valuation after one quarter\), and all remain in pre-product, pre-closed-loop R&amp;D stages. Investment includes sovereign funds \(UK AI Sovereign Fund\), chipmakers \(NVIDIA, AMD\), and government-backed funds \(Shanghai Future Industry Fund\), signaling institutional recognition of RSI as a strategic paradigm shift—not yet an engineering reality.

rss · 虎嗅 · Oct 14, 04:10

**「What is RSI?」** RSI \(Recursive Self-Improvement\) is the concept that an AI system can autonomously improve its own architecture, training process, or capabilities—potentially including designing and training successor models—creating a self-reinforcing cycle of advancement. It traces back to I. J. Good’s 1965 speculation about an &\#x27;intelligence explosion&\#x27;, where the first superintelligent machine would be humanity’s &\#x27;last invention&\#x27;. While long confined to theoretical and philosophical discussion, RSI has recently gained traction as an engineering objective, driven by observed progress in AI-assisted research \(e.g., AlphaGo Zero’s self-play, automated prompt engineering, and AI-generated code for model training pipelines\).

**「Impact」** Early-stage RSI startups are receiving massive seed funding—up to $11 billion—despite having no shipped products or verified closed-loop self-improvement, shifting investor valuation from model performance or user metrics to the speculative potential of AI-driven AI development.

**Tags**: `#AI research`, `#recursive self-improvement`, `#venture capital`, `#AI startups`, `#systems AI`

---

<a id="item-tech-news-7"></a>
### [Character.AI files Chapter 11, Disney bids $20M for non-exclusive IP license](https://www.huxiu.com/article/4897356.html?f=rss) ⭐️ 8.0/10

Character.AI filed for Chapter 11 bankruptcy in Delaware on October 12, 2026, and initiated a court-supervised auction of its assets under Section 363 of the U.S. Bankruptcy Code, with Disney acting as the stalking horse bidder at $20 million for a non-exclusive, perpetual license to certain intellectual property—excluding the company entity, app, or user data. The auction is scheduled to conclude in late November to early December 2026; if no higher bid emerges, the platform will shut down, risking loss of millions of user-created characters and chat histories. The company’s liabilities and assets are each estimated between $50 million and $100 million, and its operational continuity during the auction is conditional on finding a buyer willing to sustain the service.

rss · 虎嗅 · Oct 14, 03:13

**「Background」** Character.AI was founded in 2021 by Noam Shazeer and Daniel De Freitas, core authors of the Transformer architecture and former Google researchers behind LaMDA and Meena. It launched publicly in 2022 as a consumer-facing platform enabling user-generated AI characters, rapidly scaling to ~28 million monthly active users by mid-2024. Its business model relied on light monetization \(a $9.99/month subscription\) amid extremely high inference costs, and its technical foundation shifted after an August 2024 agreement with Google: the founders and core research team joined DeepMind, and Character.AI abandoned self-hosted large language model development in favor of fine-tuning open models from Meta and others.

**Tags**: `#AI startups`, `#generative AI`, `#bankruptcy`, `#AI infrastructure`, `#IP licensing`

---

<a id="item-tech-news-8"></a>
### [Unitree&\#x27;s Wang Xingxing: Biggest Past Mistake Was Underestimating AI](https://www.36kr.com/p/4024115259592584) ⭐️ 8.0/10

Unitree founder Wang Xingxing stated at the China Industry Expo on October 12, 2026, that his biggest strategic error over the past decade was insufficient belief in AI. He predicted the inflection point for embodied intelligence will arrive within one to two years, citing rapid AI advancement—including internal testing of Unitree’s UnifoLM-X1-0 model and integration of GPT-6—and physical constraints of on-device compute in humanoid robots. He advocated a strict cloud-edge division of labor: motion control remains on-device for real-time responsiveness, while complex decision-making relies on cloud-based large models. This reflects Unitree’s current &\#x27;base model + optional compute&\#x27; product strategy and ongoing factory pilots with automotive companies.

rss · 36氪 24小时热榜 · Oct 13, 14:02

**「Background」** Unitree is a leading Chinese robotics company known for its quadruped robots \(e.g., Go1, B1\) and now entering mass production of humanoid robots; it went public on the STAR Market in August 2026. Embodied intelligence refers to AI systems that learn and act through physical interaction with the real world—requiring tight hardware-software co-design, real-world data, and scalable compute architectures.

**「Impact」** Unitree’s shift toward cloud-dependent decision-making and reduced on-device compute mandates changes to robot architecture design, requiring developers to build APIs and infrastructure for low-latency cloud inference, and pushing customers to adopt hybrid deployment models rather than fully autonomous edge-only units.

**Tags**: `#具身智能`, `#人形机器人`, `#AI硬件协同`, `#边缘计算`, `#大模型落地`

---

<a id="item-tech-news-9"></a>
### [First Stargardt patient implanted with PRIMA visual prosthesis reads words post-surgery](https://science.xyz/news/stargardt-first-rehab/) ⭐️ 8.0/10

Science Corporation implanted the PRIMA retinal prosthesis in the first Stargardt disease patient, a procedure performed in May 2026 at Sydney Eye Hospital in Australia. The patient progressed from perceiving individual letters during initial rehabilitation to reading whole words during subsequent sessions, as announced by CEO Max Hodak. PRIMA is approved in Europe for age-related macular degeneration but has not received regulatory authorization for Stargardt disease; this implantation is part of an ongoing clinical trial. The report confirms functional visual recovery in a condition with no approved disease-modifying therapy.

telegram · zaihuapd · Oct 14, 04:30

**「Background」** Stargardt disease is an inherited retinal dystrophy causing progressive central vision loss due to degeneration of photoreceptors and retinal pigment epithelium, with no approved disease-modifying therapy. PRIMA is a subretinal wireless photovoltaic implant developed by Pixium Vision \(acquired by Science Corporation\) that bypasses damaged photoreceptors by converting light into electrical stimulation for surviving inner retinal neurons; it received CE marking in 2020 for geographic atrophy secondary to age-related macular degeneration.

**「Impact」** Stargardt disease patients—currently without any approved treatment to restore vision—now have early clinical evidence that PRIMA may provide functional letter and word recognition, potentially expanding its use beyond its current European indication for age-related macular degeneration.

**Tags**: `#medical-device`, `#neuroprosthetics`, `#retinal-disease`, `#ai-healthcare`, `#clinical-trial`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Visa Approved to Solely Prepare China&\#x27;s Bank Card Clearing Institution](https://www.huxiu.com/article/4897363.html?f=rss) ⭐️ 9.0/10

On October 13, 2026, the People’s Bank of China approved Visa to solely prepare a domestic bank card clearing institution—the first time a foreign firm has received such approval without a Chinese joint venture partner. This is a preparatory license, not an operational one, and final approval depends on Visa passing strict data security and system compliance reviews.

rss · 虎嗅 · Oct 14, 03:32

**「Background」** China opened its bank card clearing market in 2015, but prior entrants—American Express \(2020\) and Mastercard \(2024\)—did so only through joint ventures with Chinese partners, retaining local control over governance and data.

**「Impact」** This approval directly pressures China UnionPay and domestic banks to strengthen global rule-making influence and cross-border payment infrastructure, as Visa’s potential entry could shift premium and international transaction volume away from existing dual-brand cards.

**Tags**: `#金融开放`, `#支付清算`, `#人民币国际化`, `#中美经贸`, `#金融基础设施`

---

<a id="item-finance-news-2"></a>
### [Hong Kong Regulator Freezes $4.38B in Assets Amid Tea百道 IPO Manipulation Probe](https://www.huxiu.com/article/4897319.html?f=rss) ⭐️ 9.0/10

Hong Kong’s Securities and Futures Commission \(SFC\) has suspended trading of Cha Ba Dao \(02555.HK\) and frozen approximately HK$4.379 billion in assets linked to a suspected fraud group, alleging the company’s IPO demand was artificially inflated and proceeds were illegally funneled back to IPO cornerstone investors or their affiliates.

rss · 虎嗅 · Oct 14, 01:10

**「Background」** Cha Ba Dao listed on the Hong Kong Stock Exchange in April 2024 with a HK$25.86 billion IPO but saw weak investor demand—only 0.50x retail subscription and no cornerstone investors—and its stock has since fallen 77% from its HK$17.50 issue price.

**「Impact」** The freeze and suspension directly affect shareholders—who cannot trade—and 6,038 franchisees whose confidence and financial viability may erode as brand credibility collapses amid regulatory findings of IPO misconduct.

**Tags**: `#IPO监管`, `#证券欺诈`, `#港股市场风险`

---

<a id="item-finance-news-3"></a>
### [China&\#x27;s Solar Industry: Largest Installed Capacity, Largest Losses](https://www.huxiu.com/article/4897387.html?f=rss) ⭐️ 8.0/10

As of July 2026, China’s photovoltaic \(PV\) installed capacity reached 12.86 billion kW—surpassing coal power \(12.85 billion kW\) to become the nation’s largest power source; yet 13 major PV firms reported a combined net loss of ¥184.73 billion in H1 2026, with losses widening 14.43% year-on-year.

rss · 虎嗅 · Oct 14, 04:30

**「Background」** This paradox stems from massive, homogenous capacity expansion driven by local government incentives and weak industry rules, triggering a price war that pushed component prices below cash costs across the supply chain.

**「Impact」** Households and utilities face delayed solar deployment benefits due to supplier instability, while investors in PV manufacturers confront heightened credit and equity risk amid widespread unprofitability and uncertain policy enforcement.

**Tags**: `#光伏产业`, `#产能过剩`, `#价格战`, `#产业政策`, `#行业协会治理`

---

<a id="item-finance-news-4"></a>
### [Chinese NEV Makers Shift from Exporting Cars to Building Local Operations in Latin America](https://www.huxiu.com/article/4897308.html?f=rss) ⭐️ 8.0/10

In July 2026, BYD’s plant in Camaçari, Brazil—operational for less than a year—produced its 100,000th locally made new energy vehicle and employed 5,500 Brazilian workers, marking a strategic shift from exporting finished vehicles to establishing integrated local manufacturing, supply chains, and service ecosystems in Latin America.

rss · 虎嗅 · Oct 14, 00:30

**「Background」** Latin America is not a single market: Brazil prioritizes local manufacturing and employment, Mexico faces rising tariffs and North American trade rule pressures, and Chile and Colombia focus on public fleet electrification through government procurement.

**Tags**: `#automotive-industry`, `#emerging-markets`, `#supply-chain-localization`, `#electric-vehicles`, `#trade-policy`

---

<a id="item-finance-news-5"></a>
### [US drug price controls reshape China biotech valuations](https://www.huxiu.com/article/4897293.html?f=rss) ⭐️ 8.0/10

The US finalized a three-tier drug pricing control system by October 2026: 100% tariffs on most imported branded drugs \(effective October 2026\), MFN pricing agreements covering ~89% of the US branded drug market \(with eight comparator countries’ second-lowest net prices as the benchmark\), and new customs rules ending duty-free personal import of prescription drugs starting October 22, 2026.

rss · 虎嗅 · Oct 13, 23:41

**「Background」** The US built this system to isolate its domestic drug payment system from global prices—using tariffs as punishment for easily replicable imports, MFN agreements as a conditional exchange for tariff exemptions and Medicare model waivers, and customs enforcement to close the personal import loophole.

**「Impact」** For Chinese biotech firms, MFN pricing—already adopted by BeiGene—directly lowers the US payment benchmark used in licensing deal valuations, milestone calculations, and royalty forecasts, pressuring transaction values globally.

**Tags**: `#美国医药政策`, `#创新药出海`, `#药品定价管制`, `#Biotech估值`, `#MFN定价`

---

<a id="item-finance-news-6"></a>
### [Nanyang Rural Commercial Banks Accused of Systemic &\#x27;Loan-Back&\#x27; Fraud Targeting Elderly Farmers](https://www.huxiu.com/article/4897389.html?f=rss) ⭐️ 7.0/10

Investigative reporting by Jiemian News found that multiple rural commercial banks in Nanyang, Henan—including in Tanghe, Xinye, Nanzhao, Zhenping, and Wancheng districts—systematically induced elderly rural residents to sign blank or misleading loan guarantee documents, resulting in at least one verified case of RMB 390,000 forcibly deducted from a senior’s bank account in 2024; the National Financial Regulatory Administration’s Nanyang branch confirmed severe failures in the banks’ ‘three checks’ \(pre-loan investigation, mid-loan review, post-loan inspection\).

rss · 虎嗅 · Oct 14, 04:45

**「Background」** Rural commercial banks in Henan—many recently merged into the provincial &\#x27;Henan Agricultural Commercial Bank&\#x27;—face pressure to meet lending targets for agriculture and small businesses, and some local branches allegedly prioritized signatures over verifying borrowers’ identities, repayment capacity, or actual loan use.

**「Impact」** Dozens of rural elderly in Nanyang have suffered forced asset seizures, damaged credit records, and legal liability despite having no knowledge of or benefit from the loans—prompting a city-wide special rectification campaign and judicial re-examination of at least one case.

**Tags**: `#金融监管`, `#农村金融`, `#信贷欺诈`, `#消费者权益`, `#基层治理`

---

<a id="item-finance-news-7"></a>
### [China&\#x27;s AI Models Face Low C-End Pay Rates but Gain in B/G-End and Cost Advantages](https://www.huxiu.com/article/4897380.html?f=rss) ⭐️ 7.0/10

Chinese AI firms earned about $11 billion annually from six major companies in 2024—just 10% of OpenAI and Anthropic’s combined revenue—while their token usage on OpenRouter reached 65% of the global total, driven by low pricing and high volume rather than consumer subscriptions.

rss · 虎嗅 · Oct 14, 04:15

**「Background」** Unlike U.S. consumers—who average 4.5 digital subscriptions and pay $84/month—Chinese users show a 3–13% C-end AI付费 rate \(vs. 15–40% in North America\), reflecting decades of free super-app services and resistance to paying for tools.

**「Impact」** Chinese AI firms are shifting focus to B/G-end markets—where data sovereignty, private deployment, and信创 \(information technology innovation\) mandates create urgent, non-substitutable demand—bypassing C-end monetization bottlenecks.

**Tags**: `#AI商业化`, `#信创`, `#算力成本`, `#用户付费习惯`, `#中美AI比较`

---

<a id="item-finance-news-8"></a>
### [Thailand Plans 15% Civil Service Cut by 2032](https://www.huxiu.com/article/4897372.html?f=rss) ⭐️ 7.0/10

Thailand plans to reduce its civil service by 15% by the 2032 fiscal year, primarily through a voluntary early retirement program, as public debt nears the 70% of GDP ceiling and civil service wages consume one-third of the national budget.

rss · 虎嗅 · Oct 14, 03:48

**「Background」** Thailand employs about 3 million public sector workers—roughly 5% of its 41-million-person labor force—but their compensation accounts for one-third of total government spending, straining finances amid slowing GDP growth \(2% in Q3 2026\) and rising debt.

**「Impact」** Current and future Thai civil service applicants face reduced job security and career paths, while fiscal consolidation may delay public investment and social spending.

**Tags**: `#公共财政`, `#公务员改革`, `#AI就业影响`, `#东南亚经济`, `#人口结构`

---

<a id="item-finance-news-9"></a>
### [海底捞向控股股东张勇提供1亿元短期贷款](https://www.huxiu.com/article/4897370.html?f=rss) ⭐️ 7.0/10

On October 12, 2026, Haidilao \(06862.HK\) announced it would provide its controlling shareholder Zhang Yong with a RMB 100 million, 30-day short-term loan; this follows a HK$2.75 billion share sale by Zhang’s wife’s family trust in early September.

rss · 虎嗅 · Oct 14, 03:47

**「Background」** The loan comes one month after Zhang Yong’s wife’s Rose Trust sold HK$2.75 billion worth of shares — a transaction linked to upcoming tax reporting deadlines for offshore trusts under China’s July 24, 2026 tax notice, which requires residents to declare and pay tax on offshore trust gains by October 22, 2026.

**「Impact」** Morgan Stanley downgraded Haidilao to &\#x27;in line with market&\#x27; and cut its target price by 36% to HK$10.5 per share, citing governance concerns from the timing and nature of the related-party loan and prior share sale.

**Tags**: `#公司治理`, `#关联交易`, `#税务政策影响`, `#港股监管`, `#股东行为`

---

<a id="item-finance-news-10"></a>
### [Why Blaming Real Estate for All Economic Problems Is Misplaced](https://www.huxiu.com/article/4897366.html?f=rss) ⭐️ 7.0/10

The article argues that China&\#x27;s real estate sector is unfairly scapegoated for broad economic and social challenges, citing data showing its historical role in urbanization and growth—and its current systemic entanglement with local finances, household balance sheets, and industrial chains—not isolated policy failure or market distortion.

rss · 虎嗅 · Oct 14, 03:40

**「Background」** Real estate became central to China’s growth model as rapid urbanization \(67.89% urbanization rate in 2025\) drove housing demand, infrastructure investment, and land-based local government financing—making it a visible proxy for deeper structural issues like fiscal reliance on land sales and high household leverage \(62% in 2021\).

**Tags**: `#房地产调控`, `#居民资产负债表`, `#土地财政`, `#城镇化`, `#宏观经济结构`

---

<a id="item-finance-news-11"></a>
### [China&\#x27;s supermarket private labels hit 380 billion yuan in 2025](https://www.huxiu.com/article/4897364.html?f=rss) ⭐️ 7.0/10

China&\#x27;s supermarket private label sales reached 380 billion yuan in 2025, up 17% year-on-year, accounting for 9.2% of total supermarket sales.

rss · 虎嗅 · Oct 14, 03:35

**「Background」** This growth reflects a strategic shift from traditional &\#x27;renting shelf space&\#x27;—where supermarkets earned fees from brand suppliers—to developing their own products amid declining channel fees and rising consumer demand for value.

**「Impact」** Consumers gain more affordable, trusted options in categories like bottled water and paper towels, while small- and medium-sized supermarkets face pressure to build supply chain capabilities or risk being outcompeted by players with stronger private-label execution.

**Tags**: `#零售业转型`, `#自有品牌`, `#渠道变革`, `#消费降级与升级并存`, `#供应链重构`

---

<a id="item-finance-news-12"></a>
### [Shenzhen&\#x27;s Role in &\#x27;Guangdong Cars Going South&\#x27; Policy](https://www.huxiu.com/article/4897362.html?f=rss) ⭐️ 7.0/10

In June 2026, the &\#x27;Guangdong Cars Going South&\#x27; policy expanded to include Shenzhen among all nine Guangdong–Hong Kong–Macao Greater Bay Area cities, raising the daily quota for vehicles entering Hong Kong市区 from 100 to 200; the policy remains restricted to entry via the Hong Kong–Zhuhai–Macau Bridge珠海口岸, with no direct Shenzhen–Hong Kong road access yet permitted.

rss · 虎嗅 · Oct 14, 03:28

**「Background」** &\#x27;Guangdong Cars Going South&\#x27; is the reciprocal counterpart to the 2023 &\#x27;Hong Kong Cars Going North&\#x27; scheme, and as of mid-2025 had generated over 13,000 vehicle crossings under its two-phase rollout: &\#x27;arrive-and-transfer&\#x27; \(November 2025\) and &\#x27;enter-the-city&\#x27; \(December 2025\).

**「Impact」** Shenzhen drivers face an extra ~100 km detour via the Shenzhen–Zhongshan Bridge and Hong Kong–Zhuhai–Macau Bridge to access Hong Kong, delaying direct cross-border car travel while proposals for &\#x27;Shenzhen–Zhuhai closed-loop&\#x27;, &\#x27;HeTao two-way pilot&\#x27;, and &\#x27;northern metropolis zoned access&\#x27; remain conceptual or in early planning stages.

**Tags**: `#粤港澳大湾区`, `#跨境交通政策`, `#深港融合`, `#制度型开放`, `#区域经济`

---

<a id="item-finance-news-13"></a>
### [China&\#x27;s Wind and Solar Installation Slows Sharply in First Half of 2026](https://www.huxiu.com/article/4897355.html?f=rss) ⭐️ 7.0/10

In the first half of 2026, China’s new photovoltaic \(PV\) installations fell 66% year-on-year to 72.07 GW, and wind installations dropped 24.8% to 38.62 GW; several central SOEs—including大唐新能源, 甘肃能源, and 湖北能源—reported near-zero new wind or solar capacity additions.

rss · 虎嗅 · Oct 14, 03:15

**「Background」** This slowdown follows years of rapid PV expansion driven by short construction timelines and low entry barriers, but rising grid curtailment, falling midday electricity prices, and policy-driven market reforms \(e.g., Document No. 136 mandating full renewable participation in power markets\) are now reshaping investment logic from scale-first to profitability-first.

**「Impact」** New project cancellations and development rights revocations—such as 5.5 GW of PV projects withdrawn in Yunnan in September—directly affect utility-scale developers’ near-term revenue and capital allocation plans.

**Tags**: `#新能源政策`, `#电力市场`, `#央国企战略`

---

<a id="item-finance-news-14"></a>
### [China-EU Hybrid Car Trade Deal Clarified](https://www.huxiu.com/article/4897337.html?f=rss) ⭐️ 7.0/10

China and the EU agreed on a hybrid car export quota for China to the EU, anchored at 302,000 units in 2025 and rising annually, with China’s quota guaranteed not to fall below that of any other supplier; the &\#x27;halving&\#x27; claim stems from the EU’s unsupported linear projection, not the negotiated terms.

rss · 虎嗅 · Oct 14, 02:45

**「Background」** The EU had proposed using a global safeguard measure to impose import limits, but China insisted on basing the quota on actual 2025 imports \(302,000 units\) rather than past growth trends, securing an upward-adjusting, non-discriminatory arrangement.

**Tags**: `#中欧贸易`, `#新能源汽车`, `#贸易谈判`, `#WTO规则`, `#出口配额`

---

<a id="item-finance-news-15"></a>
### [European Pharma Executives Demand Policy Reform Amid Innovation Decline](https://www.huxiu.com/article/4897328.html?f=rss) ⭐️ 7.0/10

In September 2026, nine major European pharmaceutical companies—including Roche, Novartis, AstraZeneca, and GSK—jointly called for urgent reform of Europe’s investment and regulatory environment after new drug output fell to 87 approvals \(2021–2025\), far below the US \(140\) and China \(133\).

rss · 虎嗅 · Oct 14, 02:30

**「Background」** Europe’s share of global pharmaceutical R&amp;D dropped from 43% in 1990 to 31% in 2025, and its share of commercial clinical trials fell from 22% \(2013\) to 12% \(2023\), per EFPIA data.

**「Impact」** Patients in Europe face delays of nearly 600 days on average between regulatory approval and access to new medicines, with only 28% receiving full public reimbursement.

**Tags**: `#制药产业`, `#欧盟政策`, `#创新药竞争`, `#临床试验`, `#跨国药企`

---

<a id="item-finance-news-16"></a>
### [Campus Stores Boost Coffee/Tea Chain Sales Amid Industry-Wide Contraction](https://www.huxiu.com/article/4897329.html?f=rss) ⭐️ 7.0/10

Ruixing Coffee achieves ~800 cups per day at Tianjin University of Finance and Economics—1.7× its national average of 462 cups per day in Q2 2025—while the broader tea and coffee sector closed 43,200 net stores in one year and posted revenue growth without profit growth \(9.0% revenue increase but 2% net profit decline across six listed brands in H1 2026\).

rss · 虎嗅 · Oct 14, 01:56

**「Background」** After years of rapid expansion, the tea and coffee chain industry entered a &\#x27;survival mode&\#x27; in 2026, marked by widespread store closures, shrinking profitability, and intensified competition for stable, high-traffic locations like university campuses.

**「Impact」** University campuses are becoming critical testing grounds for operational efficiency—brands with strong campus execution \(e.g., Ruixing\) gain outsized sales volume and lower customer acquisition costs, while others face compressed margins due to seasonal closures and policy-driven uncertainty.

**Tags**: `#retail strategy`, `#consumer behavior`, `#food and beverage industry`, `#campus economics`, `#profitability crisis`

---