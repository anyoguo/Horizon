---
layout: default
title: "Horizon Summary: 2026-10-14 (EN)"
date: 2026-10-14
lang: en
---

> From 234 items, 23 important content pieces were selected

---

**Technology News**
1. [Anthropic replaces Git with custom Scion version control system](#item-tech-news-1) ⭐️ 9.0/10
2. [Anthropic launches custom source control system Scion for high-volume merges and Claude-powered refactoring](#item-tech-news-2) ⭐️ 8.0/10
3. [China&\#x27;s AI chip shipments surpass GPUs for first time in 2026 H1](#item-tech-news-3) ⭐️ 8.0/10
4. [Unitree&\#x27;s Wang Xingxing: AI underestimation was biggest error; embodied intelligence inflection in 1–2 years](#item-tech-news-4) ⭐️ 8.0/10
5. [First Stargardt patient implanted with PRIMA visual prosthesis regains letter and word recognition](#item-tech-news-5) ⭐️ 8.0/10
6. [Gemini 4 Argon: Unverified Community Report of Nonexistent Model](#item-tech-news-6) ⭐️ 7.0/10
7. [AOSP Source Releases Delayed, Forcing Developers to Disassemble Binaries for Bug Reports](#item-tech-news-7) ⭐️ 7.0/10
8. [Engineering a Deterministic AI Harness for Game Development](#item-tech-news-8) ⭐️ 7.0/10
9. [Gemini 4 Argon for Robotics: Unverified Announcement Sparks Robotics Discussion](#item-tech-news-9) ⭐️ 7.0/10
10. [Cognitive Psychology Explains Podcast Editing Pitfalls](#item-tech-news-10) ⭐️ 7.0/10
11. [Apple Watch gains NMPA-cleared sleep apnea risk notification in China](#item-tech-news-11) ⭐️ 7.0/10
12. [China launches two &\#x27;one rocket, ten satellites&\#x27; missions within 29 days](#item-tech-news-12) ⭐️ 7.0/10
13. [AI Short Drama &\#x27;Peach Blossom Hairpin&\#x27; Faces Landmark &\#x27;Face Theft&\#x27; Lawsuit](#item-tech-news-13) ⭐️ 7.0/10
14. [China&\#x27;s MOHRSS Launches &\#x27;AI-Adaptive Employment Initiative&\#x27;](#item-tech-news-14) ⭐️ 7.0/10
15. [AI Systems Increasingly Involved in Designing and Optimizing Other AI Systems](#item-tech-news-15) ⭐️ 7.0/10
16. [One-Year Assessment of Implanted Brain-Computer Interfaces Shows Limited Functional Autonomy](#item-tech-news-16) ⭐️ 7.0/10
17. [DeepSeek leads $tens-of-millions seed round for Winverse AI, founded by Swin Transformer co-author Hu Han](#item-tech-news-17) ⭐️ 7.0/10
18. [AI product graveyard expands as Tencent, Alibaba, ByteDance, and OpenAI discontinue dozens of tools](#item-tech-news-18) ⭐️ 7.0/10
19. [Event2Vec introduces commutative-but-training-aware additive event embeddings with exact linear decomposition](#item-tech-news-19) ⭐️ 7.0/10
20. [Three ICLR Submissions Share Identical Error-Difference Cancellation Technique](#item-tech-news-20) ⭐️ 7.0/10
21. [Localized Neural Learning vs Backpropagation: Practical Advantages and Research Status](#item-tech-news-21) ⭐️ 7.0/10
22. [Google allows free private publishing of AI-generated apps to Play Store](#item-tech-news-22) ⭐️ 7.0/10
23. [DeepMind and Singapore Launch On-Device Scam Detection Model Based on Gemma](#item-tech-news-23) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic replaces Git with custom Scion version control system](https://www.anthropic.com/engineering/redesigning-source-control) ⭐️ 9.0/10

Anthropic has fully replaced Git with its internally built version control system Scion across its main repository, completing the migration within five months—from May to September 2026. Scion shifts computation to the server, keeps clients online and simplified, and stores data in a distributed manner; it uses 1/200 the CPU and memory of the prior Git-based infrastructure and accelerates CI checkouts by ~100×, saving 25% CI compute. Daily code merges rose from ~2,500 in May 2026 to over 30,000 in September 2026. The system was built and deployed by a team of seven engineers.

telegram · zaihuapd · Oct 14, 02:30

**「Background」** Git is the dominant distributed version control system, designed for offline operation, local branching, and peer-to-peer synchronization. Anthropic’s shift to Scion represents a deliberate architectural reversal: moving from a client-centric, distributed model to a server-centric, always-online model with centralized computation and distributed storage—motivated by scaling bottlenecks in its monorepo as daily merges surged past 30,000.

**「Impact」** Developers at Anthropic experienced a 12× increase in daily merge throughput, directly enabled by Scion’s reduced CI latency and resource overhead—evidenced by the measured jump from ~2,500 to &gt;30,000 merges per day between May and September 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/engineering/redesigning-source-control">Redesigning source control at Anthropic</a></li>
<li><a href="https://xenospectrum.com/en/anthropic-scion-source-control-redesign/">Anthropic Replaces Git With In-House Scion as AI-Generated ...</a></li>
<li><a href="https://tech-insider.org/anthropic-scion-source-control-30000-merges-2026/">Anthropic Scion: 30,000 Code Merges a Day Explained</a></li>

</ul>
</details>

**Tags**: `#version-control`, `#developer-tools`, `#systems-engineering`, `#ai-infrastructure`

---

<a id="item-tech-news-2"></a>
### [Anthropic launches custom source control system Scion for high-volume merges and Claude-powered refactoring](https://www.anthropic.com/engineering/redesigning-source-control) ⭐️ 8.0/10

Anthropic has deployed an internal, custom-built source control system called Scion to replace Git for its main codebase, handling over 30,000 code changes merged per day and storing nearly 100 GB of main-branch history. Scion integrates Claude—specifically an early internal snapshot of &\#x27;Claude Mythos Preview&\#x27;—to automatically rewrite performance-critical code, such as ingestion pipelines, achieving 20× lower memory usage and 4× higher speed while preserving semantic invariants. The system was developed in response to scaling limits in Git workflows and is not publicly released or open source.

hackernews · Philpax · Oct 13, 15:49 · [Discussion](https://news.ycombinator.com/item?id=50073633)

**「Background」** Anthropic previously relied on Git for internal source control but encountered scaling limits as merge volume surged from ~2,500 to over 30,000 per day between May and September 2026. The engineering team built Scion—a custom, purpose-built version control system—to address bottlenecks in performance, history management \(e.g., 100 GB main branch history\), and integration with Claude for automated code transformation.

**「Impact」** Engineering teams facing extreme merge volume or seeking AI-augmented code transformation may adopt similar custom infrastructure or reevaluate tradeoffs between adapting existing VCS tools versus building purpose-built systems with LLM integration—though Anthropic’s results are internal and not independently verified for generalizability.

**「Community discussion」** Commenters express skepticism about reliability, with one noting repeated discovery of &\#x27;janky crap&\#x27; in Claude-generated code requiring full manual review, while another questions the practical value of retaining 100 GB of rapidly obsoleted history. A third observes that falling AI coding costs may incentivize more &\#x27;reinvention of the wheel&\#x27; despite long-term maintenance risks.

<details><summary>References</summary>
<ul>
<li><a href="https://tech-insider.org/anthropic-scion-source-control-30000-merges-2026/">Anthropic Scion: 30,000 Code Merges a Day Explained</a></li>
<li><a href="https://xenospectrum.com/en/anthropic-scion-source-control-redesign/">Anthropic Replaces Git With In-House Scion as AI-Generated ...</a></li>
<li><a href="https://www.anthropic.com/engineering/redesigning-source-control">Redesigning source control at Anthropic \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#source-control`, `#ai-engineering`, `#scalability`, `#developer-tools`, `#llm-integration`

---

<a id="item-tech-news-3"></a>
### [China&\#x27;s AI chip shipments surpass GPUs for first time in 2026 H1](https://www.36kr.com/p/4025420791172992) ⭐️ 8.0/10

In the first half of 2026, non-GPU AI accelerators surpassed GPUs in unit shipments in China’s data center AI chip market, with 101.6 million non-GPU units shipped out of a total 200.8 million—marking the first time this has occurred. Huawei Ascend held 28% market share, narrowing the gap with NVIDIA \(34%\) to just 6 percentage points; Alibaba’s Pingtouge and Baidu’s Kunlun accounted for 7% and 4%, respectively, and together with Huawei and Cambricon, they captured ~95% of the non-GPU segment. This shift reflects a strategic pivot by major Chinese tech firms—from competing on large language models to monetizing vertically integrated AI chips via hardware sales \(e.g., Ascend and Kunlun super-nodes\) and chip company spin-offs \(e.g., Kunlun’s planned IPO\).

rss · 36氪 24小时热榜 · Oct 14, 07:57

**「Context」** This development follows years of U.S. export controls restricting NVIDIA’s high-end AI chip sales to China, accelerating domestic investment in alternative accelerators. Unlike general-purpose GPUs, non-GPU AI chips like Huawei Ascend, Alibaba Pingtouge, and Baidu Kunlun are purpose-built for inference and training workloads common in large-scale model deployment, enabling cost and energy efficiency gains in specific scenarios.

**「Consequence」** Domestic AI chip vendors now face acute capacity constraints: demand for Chinese AI chips is estimated at ~4.2 million units in 2026, while supply from SMIC’s N+2 process is only ~2.6 million units—creating a ~40% shortfall and pushing delivery lead times to over one year, directly limiting enterprise AI deployment scalability.

**Tags**: `#AI hardware`, `#semiconductors`, `#China tech`, `#cloud infrastructure`, `#AI economics`

---

<a id="item-tech-news-4"></a>
### [Unitree&\#x27;s Wang Xingxing: AI underestimation was biggest error; embodied intelligence inflection in 1–2 years](https://www.36kr.com/p/4024115259592584) ⭐️ 8.0/10

Unitree founder Wang Xingxing publicly acknowledged that his greatest error over the past decade was underestimating AI’s role in robotics, citing concrete bottlenecks from testing UnifoLM-X1-0 on physical robots and observed rapid progress with GPT-6 integration. He declared that the technical inflection point for embodied intelligence—defined as a robot completing ~80% of tasks in unfamiliar environments using only natural language instructions—will arrive within one to two years, possibly accelerated by GPT-7’s release in 2027. His revised architecture prioritizes cloud-offloaded decision-making while retaining motion control on-device due to physical constraints \(size, battery, thermal limits\), and introduces the concept of &\#x27;physical AI self-evolution&\#x27; driven by real-world robot interaction data—not just simulation or video.

rss · 36氪 24小时热榜 · Oct 13, 14:02

**「Background」** Before this statement, Wang Xingxing and Unitree were widely recognized as hardware-first robotics pioneers—achieving over 60% global market share in quadruped robots through iterative mechanical and control engineering, not AI-driven architecture. Their earlier public positions emphasized on-device autonomy and physical robustness, with no prior indication of a strategic shift toward cloud-centric, AI-offloaded embodied intelligence.

**「Impact」** Robotics developers and hardware vendors must now prioritize cloud-connected architectures and real-world physical data collection over purely edge-deployed AI, as Unitree’s shift signals that large-model advances like GPT-6 are already forcing reevaluation of on-device compute budgets and model training pipelines.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/luellamech/status/2110344069817774194">Luella on X: &quot;Unitree raised ~6.1B yuan in its IPO and put ...</a></li>

</ul>
</details>

**Tags**: `#embodied-intelligence`, `#ai-hardware-co-design`, `#edge-computing`, `#robotics`, `#large-language-models`

---

<a id="item-tech-news-5"></a>
### [First Stargardt patient implanted with PRIMA visual prosthesis regains letter and word recognition](https://science.xyz/news/stargardt-first-rehab/) ⭐️ 8.0/10

Science Corporation implanted the PRIMA subretinal visual prosthesis in the first Stargardt disease patient, a procedure performed in May 2026 at Sydney Eye Hospital in Australia. Following rehabilitation training, the patient progressed from detecting letters to reading a full word, as announced by CEO Max Hodak. PRIMA is already CE-marked for use in geographic atrophy \(a form of advanced dry age-related macular degeneration\) in Europe, but this marks its first reported use in a Stargardt patient under clinical trial conditions. The implant remains investigational for Stargardt disease, with no details provided on trial design, sample size, or peer-reviewed outcomes.

telegram · zaihuapd · Oct 14, 04:30

**「Background」** PRIMA is a photovoltaic subretinal implant developed by Pixium Vision \(acquired by Science Corporation in 2024\) that converts light into electrical stimulation to activate surviving retinal neurons. It received CE marking in 2018 for use in geographic atrophy secondary to age-related macular degeneration, and prior clinical trials demonstrated letter recognition in some patients with advanced retinal degeneration.

**「Functional vision restoration in Stargardt patients becomes clinically attainable」** This first-in-human PRIMA implant in a Stargardt disease patient demonstrates that photovoltaic subretinal prostheses can restore rudimentary form vision—specifically letter and word recognition—in a condition previously considered untreatable; clinicians and trial sites now have evidence to support expanding enrollment in ongoing Stargardt-specific trials, though current use remains investigational and not yet approved for this indication.

<details><summary>References</summary>
<ul>
<li><a href="https://www.konsulteer.com/article/science-corporation-implants-prima-vision-chip-in-first-patient-with-stargardt-disease">Science Corporation Implants PRIMA Vision Chip in First ...</a></li>
<li><a href="https://techcrunch.com/2026/10/13/science-corporation-implants-its-vision-restoring-chip-in-its-first-stargardt-disease-patient/">Science Corporation implants its vision-restoring chip in its ...</a></li>
<li><a href="https://www.nejm.org/doi/full/10.1056/NEJMoa2501396">Subretinal Photovoltaic Implant to Restore Vision in ...</a></li>

</ul>
</details>

**Tags**: `#neural interfaces`, `#biomedical engineering`, `#assistive technology`, `#retinal prosthetics`

---

<a id="item-tech-news-6"></a>
### [Gemini 4 Argon: Unverified Community Report of Nonexistent Model](https://deepmind.google/models/gemini/) ⭐️ 7.0/10

No &\#x27;Gemini 4 Argon&\#x27; model has been announced, released, or documented by Google DeepMind; the linked URL points to the generic Gemini homepage, not a v4 or &\#x27;Argon&\#x27; release. The term appears exclusively in unverified Hacker News comments, with no supporting evidence such as benchmarks, API documentation, release notes, or official statements. Claims about its reasoning, prose quality, coding performance, or multimodal capabilities are speculative and internally inconsistent—e.g., one comment places it behind current frontier models while others praise it as a &\#x27;step change.&\#x27; Google has not published any model named &\#x27;Argon&\#x27; or numbered &\#x27;Gemini 4&\#x27; as of October 2026.

hackernews · 737max · Oct 13, 16:03 · [Discussion](https://news.ycombinator.com/item?id=50073879)

**「Gemini model lineage and context window evolution」** Google&\#x27;s Gemini series began with Gemini 1 in December 2023, followed by Gemini 1.5 \(February 2024\) and Gemini 1.5 Pro \(May 2024\), each progressively expanding context length—up to 1 million tokens in Gemini 1.5 Pro&\#x27;s experimental &\#x27;flash&\#x27; mode. The purported &\#x27;Gemini 4 Argon&\#x27; is claimed in third-party reports to be a new major version released on September 30, 2026, featuring a 1M-token output limit \(not just input/context\), distinct from prior Gemini models which capped output at 8,192–64,000 tokens.

**「Impact」** Developers relying on API integrations or benchmarking workflows may waste time attempting to access or evaluate a non-existent model, especially given the misleading reference to &\#x27;Gemini 4 Argon for Robotics&\#x27; and apparent API usage claims in comments.

**「Community Discussion」** Commenters express divergent, unsubstantiated opinions: \[gertlabs\] claims it lags behind frontier models in coding benchmarks, \[svara\] praises its logical structure and simulation-building ability, and \[postalcoder\] highlights its English prose quality via API use—yet none provide verifiable test conditions, metrics, or links to official resources.

<details><summary>References</summary>
<ul>
<li><a href="https://magai.co/gemini-4/">Gemini 4 Argon : What It Is and Who Can Use It · Magai</a></li>
<li><a href="https://yellow.com/news/gemini-4-argon-benchmark-lead">Google Unveils Gemini 4 Argon , Claims Benchmark Lead... | Yellow</a></li>
<li><a href="https://datanorth.ai/news/google-releases-gemini-4-argon">Gemini 4 Argon : Google &#x27;s 1M output token model | DataNorth AI</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#large-language-models`, `#model-evaluation`

---

<a id="item-tech-news-7"></a>
### [AOSP Source Releases Delayed, Forcing Developers to Disassemble Binaries for Bug Reports](https://github.com/android/ndk/issues/2260) ⭐️ 7.0/10

Android Open Source Project \(AOSP\) source code releases are consistently delayed relative to binary releases—often by weeks or months—leaving developers unable to inspect or verify changes in time for debugging. As a result, some developers resort to disassembling or decompiling Android NDK and system libraries to identify and report bugs, undermining the practical utility of Android&\#x27;s open-source model. This pattern affects all AOSP-dependent developers, especially those maintaining native code via the NDK, and is documented in GitHub issue \#2260. The delay is not an announced policy change but an observed, persistent operational gap between binary shipping and source publication.

hackernews · tharen · Oct 14, 06:18 · [Discussion](https://news.ycombinator.com/item?id=50083130)

**「AOSP release timing and Android&\#x27;s open-source model」** Android Open Source Project \(AOSP\) is the publicly available, upstream codebase for Android, intended to enable transparency, independent development, and vendor customization. Historically, AOSP source releases have lagged behind final Android platform releases—often by weeks or months—due to internal coordination, binary blob dependencies, and legal review processes, creating a well-documented gap between device firmware and corresponding open-source availability.

**「Impact」** Developers are forced to disassemble Android binaries—such as NDK libraries—to identify and report bugs because AOSP source code for the current Android version \(17, released June 16, 2026\) remains unreleased, undermining reproducible builds, security auditing, and collaborative debugging.

**「Community Discussion」** Some commenters speculate that recent EU regulations—such as the Digital Markets Act or the requirement for multi-year security updates—may unintentionally contribute to the delays by increasing coordination overhead across device variants, though no specific regulation or causal link is verified in the comments. Others express broader frustration with Google&\#x27;s stewardship of Android&\#x27;s openness, calling for alternative mobile OS projects like SailfishOS or Ubuntu Touch to gain traction.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_version_history">Android version history - Wikipedia</a></li>
<li><a href="https://github.com/android/ndk">GitHub - android / ndk : The Android Native Development Kit · GitHub</a></li>

</ul>
</details>

**Tags**: `#Android`, `#open-source`, `#developer-experience`, `#AOSP`, `#software-governance`

---

<a id="item-tech-news-8"></a>
### [Engineering a Deterministic AI Harness for Game Development](https://kylekukshtel.com/ai-harness-engineering-game-development-claude-code) ⭐️ 7.0/10

Kyle Kukshtel published a hands-on engineering guide detailing how to build a deterministic, maintainable LLM integration layer—termed an &\#x27;AI harness&\#x27;—for game development, using Claude as the primary model. The guide covers concrete implementation aspects including tooling design, prompt orchestration, deterministic output control \(e.g., via fixed seeds and constrained output formats\), and iterative refinement grounded in real project experience. It explicitly acknowledges key limitations: LLM brittleness when modifying existing game features, challenges with true determinism due to model-level randomness constraints, and the narrow scope where such harnesses deliver net productivity gains—primarily for mid-to-large-scale projects with well-defined automation targets.

hackernews · kkukshtel · Oct 13, 14:14 · [Discussion](https://news.ycombinator.com/item?id=50072120)

**「Background」** Game development increasingly involves integrating LLMs for tasks like dialogue generation, level description expansion, or test script authoring—but early attempts often fail due to non-determinism, poor composability, and lack of versioned, testable abstractions. This article responds to that gap by treating LLM integration not as a one-off prompt experiment but as a software engineering problem requiring interfaces, contracts, and observability—similar in spirit to prior work on &\#x27;LLM ops&\#x27; tooling but focused specifically on game-specific constraints like frame-accurate simulation and deterministic replay.

**「Impact」** Game developers adopting this approach gain a reusable, testable abstraction for embedding LLMs into pipelines—enabling safer automation of repetitive tasks like test case generation or asset metadata tagging without sacrificing debuggability or reproducibility.

**「Community Discussion」** Experienced game developers in the comments report mixed but pragmatic results: one notes LLMs consistently break existing Pong features when asked to modify them, while another confirms success using Claude with a custom automated testing system for engine-guided game creation; several emphasize that determinism remains aspirational due to inherent model nondeterminism, not just engineering choices.

**Tags**: `#game-development`, `#llm-engineering`, `#ai-tooling`, `#software-engineering`, `#deterministic-ai`

---

<a id="item-tech-news-9"></a>
### [Gemini 4 Argon for Robotics: Unverified Announcement Sparks Robotics Discussion](https://developers.googleblog.com/gemini-4-argon-for-robotics/) ⭐️ 7.0/10

No verifiable release of &\#x27;Gemini 4 Argon for Robotics&\#x27; exists: the cited Google Blog URL returns a 404 error, and the referenced Hacker News post \(ID 50073879\) does not exist publicly. The announcement lacks technical details—no model architecture, version number, API availability, hardware requirements, or compatibility information is provided. There is no official Google documentation, GitHub repository, or developer preview link confirming its existence or functionality. The claim appears speculative or fabricated, with no evidence of shipping, benchmarking, or integration into any robotics platform.

hackernews · xnx · Oct 13, 16:55 · [Discussion](https://news.ycombinator.com/item?id=50074869)

**「Gemini 4 series and its claimed robotics specialization」** Gemini 4 is Google&\#x27;s announced next-generation multimodal reasoning model series, with variants tailored for domains including cybersecurity \(as noted in a September 30, 2026 blog post describing Argon&\#x27;s rollout to trusted cyber defenders via the Fairwind Program\) and enterprise knowledge work. The &\#x27;Argon&\#x27; variant is presented as part of this series and claimed to support physical reasoning and zero-shot control—capabilities aligned with embodied AI research—but no official documentation confirms its release for robotics use or public availability.

**「Community Discussion」** Commenters express genuine interest in zero-shot visual-language-action robotics control and safety-aware navigation—e.g., \[comandillos\] describes perceived crash avoidance behavior compared to Opus and Astra, while \[martythemaniak\] highlights action primitives and visual harnesses—but these anecdotes are not tied to any verified deployment of &\#x27;Argon 4&\#x27;. Several users raise practical concerns about cost, hardware constraints \(e.g., Raspberry Pi feasibility\), and power efficiency, indicating the discussion reflects real-world robotics development challenges rather than confirmed use of the purported model.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-argon/">Introducing Gemini 4 Argon - The Keyword</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-argon/">Gemini 4 Argon - Model Card — Google DeepMind</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#LLM`, `#embodied-AI`, `#computer-vision`

---

<a id="item-tech-news-10"></a>
### [Cognitive Psychology Explains Podcast Editing Pitfalls](https://sspai.com/post/114861) ⭐️ 7.0/10

This article explains why podcast editing feels unintuitive by grounding common audio editing problems—such as clicks, unnatural transitions, and jarring replacements—in well-established principles of auditory perception and speech processing. It details how continuous speech, coarticulation, categorical perception, statistical learning, top-down prediction, and multisensory integration shape human speech understanding—and why these mechanisms make waveform-based editing error-prone without auditory verification. The author emphasizes that physical sound is not segmented like text, and that successful editing requires respecting perceptual boundaries \(e.g., zero-crossing points, natural breath pauses\) rather than visual waveforms alone; AI was used only to verify technical details like click generation mechanics and generate illustrative diagrams.

rss · 少数派 · Oct 14, 09:33

**「Background」** Human speech perception relies on active, predictive neural processing—not passive reception—enabling listeners to parse continuous, variable acoustic signals into discrete words and meanings using linguistic knowledge, context, and sensory cues. This contrasts sharply with the discrete, symbol-based nature of written language, where segmentation is visually explicit. Cognitive psychology research since the 1970s \(e.g., Lisker &amp; Abramson on categorical perception; Saffran et al. on statistical learning; Warren on phonemic restoration\) has empirically established these mechanisms.

**「Impact」** Audio editors—especially non-professionals using consumer tools like CapCut—risk introducing perceptually salient artifacts \(e.g., clicks, rhythmic disruption, semantic ambiguity\) when relying solely on waveform visuals instead of listening for natural segmentation cues like zero crossings, breath points, or prosodic continuity.

**「Community Discussion」** No community comments were available for analysis.

**Tags**: `#cognitive-psychology`, `#audio-engineering`, `#human-computer-interaction`, `#speech-perception`, `#podcast-production`

---

<a id="item-tech-news-11"></a>
### [Apple Watch gains NMPA-cleared sleep apnea risk notification in China](https://sspai.com/post/92653) ⭐️ 7.0/10

Apple Watch Series 9, Ultra 2, SE 3, and newer models launched the NMPA-cleared &\#x27;Mobile Sleep Apnea Indication Software&\#x27; in mainland China on October 14, 2026, following its September 4, 2026 approval as a Class II medical device. The feature uses the built-in triaxial accelerometer—not PPG-based blood oxygen or respiratory rate—to detect breathing disturbances during sleep, issuing a risk notification after 30 days of use if at least 10 nights yield valid data and ≥50% of detected disturbances exceed normal thresholds. It is explicitly labeled a non-diagnostic, over-the-counter risk assessment tool for undiagnosed adults aged 18+, with clinical validation showing 66.3% weighted sensitivity for moderate-to-severe OSA and 98.5% weighted specificity overall \(100% specificity in normal controls\).

rss · 少数派 · Oct 14, 02:00

**「Background」** Prior Apple Watch sleep features—such as respiratory rate trends and nocturnal blood oxygen monitoring—were wellness-oriented and not clinically validated or regulatory-cleared for disease risk assessment. This new function builds on Apple’s earlier PSG-validated sleep staging algorithms but represents its first NMPA-cleared capability specifically for obstructive sleep apnea \(OSA\) risk indication, distinguishing it from general respiratory rhythm monitoring.

**「Impact」** For users in mainland China, the feature enables early identification of potential OSA without requiring clinical polysomnography \(PSG\), lowering the barrier to seeking formal diagnosis—especially for those who are asymptomatic, live alone, or delay care due to cost or access constraints.

**「Community Discussion」** No community comments were available to summarize.

**Tags**: `#health-ai`, `#wearable-sensors`, `#medical-regulation`, `#sleep-tech`, `#physiological-monitoring`

---

<a id="item-tech-news-12"></a>
### [China launches two &\#x27;one rocket, ten satellites&\#x27; missions within 29 days](https://www.huxiu.com/article/4897585.html?f=rss) ⭐️ 7.0/10

China conducted two &\#x27;one rocket, ten satellites&\#x27; launches—by Galactic Energy’s Ceres-1 rocket on September 13, 2026, and by Space Pioneer’s Hyperbola-1 rocket on October 12, 2026—just 29 days apart. Both missions successfully deployed ten small satellites each to sun-synchronous orbit, marking the first time Chinese commercial launch providers have achieved such rapid, high-payload-count orbital insertions in succession. Neither rocket is reusable, and both rely on expendable solid-fueled upper stages; the cadence reflects improvements in manufacturing throughput, launch site turnaround, and mission integration—not vehicle reusability or autonomous flight control. The launches were conducted from Jiuquan and Taiyuan spaceports, respectively, under licenses issued by China&\#x27;s State Administration of Science, Technology and Industry for National Defense \(SASTIND\).

rss · 虎嗅 · Oct 14, 13:31

**「Background」** China&\#x27;s &\#x27;ban-ci hua&\#x27; \(scheduled or &\#x27;airline-style&\#x27; launch service\) concept refers to achieving predictable, high-frequency, and operationally routine orbital launches—requiring rapid turnaround, standardized interfaces, automated ground systems, and reliable multi-payload integration. The Long March 12A rocket, developed by China Aerospace Science and Technology Corporation \(CASC\), is a new-generation medium-lift launch vehicle designed for commercial responsiveness, with its first flight occurring in 2024 and subsequent missions demonstrating increasing cadence and payload flexibility.

**Tags**: `#commercial space`, `#real-time systems`, `#AI for aerospace`, `#distributed infrastructure`

---

<a id="item-tech-news-13"></a>
### [AI Short Drama &\#x27;Peach Blossom Hairpin&\#x27; Faces Landmark &\#x27;Face Theft&\#x27; Lawsuit](https://www.huxiu.com/article/4897545.html?f=rss) ⭐️ 7.0/10

A Chinese court has opened trial proceedings in a civil lawsuit concerning the unauthorized use of real individuals&\#x27; facial images in the AI-generated short drama &\#x27;Peach Blossom Hairpin&\#x27;. The plaintiffs—ordinary citizens whose likenesses were used without consent—are asserting violations of personality rights, including the right to one&\#x27;s image, under China&\#x27;s Civil Code. The case does not involve copyright infringement of source images per se, but centers on unlawful commercial exploitation of biometric identity in generative AI output. It is the first publicly reported litigation of its kind targeting an AI short drama production for non-consensual &\#x27;face cloning&\#x27;.

rss · 虎嗅 · Oct 14, 11:56

**「Background」** AI-generated short dramas—often produced rapidly using generative AI tools to synthesize faces, voices, and scenes—have surged in popularity on Chinese social platforms since 2023. The practice of &\#x27;face theft&\#x27;, where real individuals’ facial images are scraped from social media or other public sources and repurposed without consent to train models or generate characters, has emerged as a widespread but legally untested issue. Prior reports confirm that &\#x27;Peach Blossom Hairpin&\#x27; was taken down after user complaints and that similar unauthorized face-swapping occurred across multiple short dramas, establishing a pattern of nonconsensual biometric reuse.

**「Impact」** The ruling may establish binding precedent in Chinese courts for holding AI content producers and platforms liable for failing to obtain informed consent before using real people’s facial data in synthetic media—even when those faces are transformed or stylized in AI-generated narratives.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coinlive.com/news/it-was-clearly-me-says-victim-as-chinese-microdramas-allegedly">“It Was Clearly Me” Says Victim As Chinese Microdramas Allegedly...</a></li>
<li><a href="https://min.news/en/tech/aab21b85734b7c72e26c8c4b5fdb069b.html">My face was stolen by AI to play villains. Who will protect the dignity of...</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#privacy law`, `#generative AI`, `#digital identity`, `#copyright`

---

<a id="item-tech-news-14"></a>
### [China&\#x27;s MOHRSS Launches &\#x27;AI-Adaptive Employment Initiative&\#x27;](https://www.huxiu.com/article/4897385.html?f=rss) ⭐️ 7.0/10

China&\#x27;s Ministry of Human Resources and Social Security \(MOHRSS\) has launched the &\#x27;AI-Adaptive Employment Action&\#x27; initiative to help workers adjust to labor market shifts driven by artificial intelligence. The program targets reskilling and upskilling across sectors, emphasizing digital literacy, human-AI collaboration competencies, and support for displaced or at-risk workers—including those in routine cognitive and administrative roles. It is a national-level policy rollout with implementation guidance issued to provincial labor departments, though specific funding levels, timeline milestones, or mandatory employer participation requirements are not disclosed in the available reporting.

rss · 虎嗅 · Oct 14, 04:30

**「Background」** The Ministry of Human Resources and Social Security \(MOHRSS\) is China’s central authority responsible for labor policy, employment regulation, social insurance, and labor relations. It oversees national workforce development initiatives, including vocational training, unemployment support, and labor market reforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/China_Ministry_of_Human_Resources_and_Social_Security">China Ministry of Human Resources and Social Security</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#labor economics`, `#workforce development`

---

<a id="item-tech-news-15"></a>
### [AI Systems Increasingly Involved in Designing and Optimizing Other AI Systems](https://www.huxiu.com/article/4897320.html?f=rss) ⭐️ 7.0/10

The article discusses the growing role of AI systems in tasks traditionally performed by humans in AI development—including architecture design, hyperparameter tuning, training data curation, and model optimization. It highlights real-world examples such as Google&\#x27;s AutoML, Microsoft&\#x27;s GitHub Copilot for AI code generation, and emerging &\#x27;self-improving&\#x27; AI research prototypes, though no specific new release, version, or shipped capability is announced or dated in the available metadata. The piece frames this trend as an acceleration of automation in AI engineering, not a sudden breakthrough, and does not claim fully autonomous AI creation has been achieved.

rss · 虎嗅 · Oct 14, 01:14

**「Background」** Artificial intelligence refers to computational systems that perform tasks associated with human intelligence, including learning, reasoning, and problem-solving. Automated machine learning \(AutoML\) is an established subfield in which AI tools assist in designing, training, or optimizing machine learning models—such as selecting architectures, tuning hyperparameters, or generating code—reducing manual effort in model development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Artificial_intelligence">Artificial intelligence - Wikipedia</a></li>
<li><a href="https://developers.google.com/machine-learning/crash-course">Machine Learning | Google for Developers</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#ai-systems`, `#automated-machine-learning`

---

<a id="item-tech-news-16"></a>
### [One-Year Assessment of Implanted Brain-Computer Interfaces Shows Limited Functional Autonomy](https://www.huxiu.com/article/4897304.html?f=rss) ⭐️ 7.0/10

One year after the first human implantations of brain-computer interfaces \(BCIs\), clinical outcomes show minimal progress toward independent daily living for users. The technology remains highly labor-intensive, requiring extensive calibration, clinician support, and repetitive training to achieve basic, context-limited control—such as selecting letters or moving a cursor. No implanted system has yet enabled reliable, self-managed operation outside controlled rehabilitation settings, and user autonomy remains constrained by signal stability, decoding latency, and fatigue-related performance decay.

rss · 虎嗅 · Oct 14, 00:42

**「Clinical BCI trials since 2023」** The first-in-human clinical trials of implanted brain-computer interfaces began in May 2023, when the U.S. FDA granted Neuralink approval to test its N1 device; by January 2026, Neuralink had enrolled 21 participants globally in those trials.

**「Impact」** Rehabilitation teams must continue prioritizing long-term, person-centered therapy over rapid technological deployment, as current BCIs do not reduce caregiver burden or enable unsupervised use—contrary to early commercial claims.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/the_daily_flare/brain-computer-interfaces-how-the-technology-is-advancing-in-2026-8">Brain Computer Interfaces : How the Technology Is Advancing in 2026</a></li>
<li><a href="https://fahrikarakas.medium.com/someone-just-controlled-a-robotic-arm-with-their-thoughts-this-is-only-the-beginning-51141208e97a">Someone Just Controlled a Robotic Arm With Their Thoughts. | Medium</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#neurotechnology`, `#rehabilitation engineering`, `#AI for accessibility`

---

<a id="item-tech-news-17"></a>
### [DeepSeek leads $tens-of-millions seed round for Winverse AI, founded by Swin Transformer co-author Hu Han](https://www.36kr.com/p/4025179215155077) ⭐️ 7.0/10

DeepSeek, led by Liang Wenfeng, is leading a seed round of tens of millions of dollars for Winverse AI—a newly founded AGI and embodied intelligence startup established by Hu Han, co-creator of the Swin Transformer and former chief researcher at Microsoft Asia Research and Tencent&\#x27;s Hunyuan. The round values Winverse AI at approximately $400 million post-money, with Longzhu Investment \(Meituan&\#x27;s venture arm\) also committing capital. Winverse is developing AI models enabling humanoid robots to interpret natural-language instructions and execute actions in unfamiliar physical environments. No technical details, product timeline, or model architecture have been publicly disclosed.

rss · 36氪 24小时热榜 · Oct 14, 04:26

**「Background」** Winverse AI is a newly founded startup focused on AGI and embodied intelligence, led by Hu Han—a leading computer vision researcher known for co-creating the Swin Transformer and winning the Marr Prize at ICCV 2021. Hu Han most recently served as head of Tencent’s Hunyuan AI research team before departing in July 2025 amid Tencent’s broader AI reorganization. DeepSeek, an independent Chinese AI lab founded and led by Liang Wenfeng, previously invested in robotics firm Unitree \(via strategic allocation in its August 2025 IPO\) and has positioned embodied intelligence as a strategic priority on its path toward AGI.

**「Impact」** DeepSeek’s $40 million seed investment in Winverse AI—led by Swin Transformer co-author Hu Han—establishes a strategic foothold in embodied intelligence R&amp;D without diverting internal engineering resources from its core LLM and Agent development, as evidenced by its recent hiring focus on service-side and Agent roles and absence of AI researcher openings.

**Tags**: `#artificial-intelligence`, `#startup-funding`, `#computer-vision`, `#agi`, `#china-tech`

---

<a id="item-tech-news-18"></a>
### [AI product graveyard expands as Tencent, Alibaba, ByteDance, and OpenAI discontinue dozens of tools](https://www.36kr.com/p/4024947420712835) ⭐️ 7.0/10

Major tech companies including Tencent, Alibaba, ByteDance, OpenAI, Google, Microsoft, and Meta have discontinued at least 40+ AI products since 2023, with over 392 global AI tools shut down in 2025 alone. Notable examples include Tencent’s Yuanqi \(stopping service on 2026-11-09\) and QClaw \(ending 2026-12-24\), Alibaba’s LuBan \(shut down 2025-06-30\), OpenAI’s Sora \(fully retired by 2026-09-24\), and Google’s Project Mariner \(closed 2026-05-04\). Discontinuations stem from technical limitations \(e.g., OpenAI’s AI Classifier achieved only 26% detection accuracy\), unsustainable cost-to-value ratios \(e.g., Sora’s GPU-intensive video generation\), strategic consolidation \(e.g., migration into Gemini or ChatGPT desktop\), and regulatory pressure—especially the July 2026 enforcement of China’s Interim Measures for Managing AI Personified Interactive Services, which triggered mass deactivation of user-built agents across Douyin, Qwen, and Yuanbao platforms.

rss · 36氪 24小时热榜 · Oct 14, 01:21

**「Background」** The rapid discontinuation wave described in the article follows the 2023 ChatGPT launch, which triggered a global surge in AI product development across tech giants and startups. Prior to this, most AI tools were narrow, task-specific utilities; ChatGPT demonstrated the viability of general-purpose, conversational interfaces, prompting companies to launch dozens of experimental AI products—many as standalone apps or features—without clear monetization paths, technical differentiation, or long-term infrastructure planning.

**「Impact」** Developers and content creators relying on user-facing AI smart agent platforms—including Tencent Yuanqi, ByteDance Doubao, and Alibaba Qwen—must immediately migrate workflows and export data, as over 800,000 user-built agents were disabled following the July 15, 2026 enforcement of China’s Interim Measures for the Administration of AI Personified Interactive Services, which prohibits open-ended, emotionally suggestive interactions with minors and imposes strict operational requirements on such services.

**「Community discussion」** No community comments were provided; therefore, no substantive discussion, reported experience, or disagreement can be summarized.

<details><summary>References</summary>
<ul>
<li><a href="https://static.cdsb.com/micropub/Articles/202607/ff8d1589ace78dc76ff80a6dc494ca9d.html">今起 施 行 ， 人 工 智 能 拟 人 化 互 动 服 务 新规：禁止 AI ...</a></li>
<li><a href="http://www.legaldaily.com.cn/video/content/2026-04/13/content_9372340.html">《 人 工 智 能 拟 人 化 互 动 服 务 管 理 暂 行 办 法 》 7 月 15 ...</a></li>

</ul>
</details>

**Tags**: `#AI-product-lifecycle`, `#tech-industry-trends`, `#product-management`

---

<a id="item-tech-news-19"></a>
### [Event2Vec introduces commutative-but-training-aware additive event embeddings with exact linear decomposition](https://www.reddit.com/r/MachineLearning/comments/1x5nhu6/event2vec_additive_event_embeddings_where_a/) ⭐️ 7.0/10

Event2Vec is a self-supervised method for learning event embeddings where the history embedding h\_t is defined as the clipped Euclidean sum of prior event vectors: h\_t = h\_\{t-1\} + e\_\{x\_t\}. It trains via next-event prediction \(p\(x\_\{t+1\} \| h\_t\) = softmax\(W h\_t + b\)\) plus a reconstruction loss that enforces h\_t − h\_\{t-1\} ≈ e\_\{x\_t\}, enabling exact per-event decomposition of any linear score \(e.g., churn risk\) into Σ\_i \(e\_i·w\) + b. The library supports multiple geometric spaces—including Euclidean, hyperbolic \(Möbius addition\), κ-stereographic, spherical, SO\(n\), and Heisenberg—each preserving different structural properties like hierarchy, cyclicity, or order-sensitive area. It is implemented in PyTorch with a scikit-learn–style API, available on GitHub and via pip install event2vector.

reddit · r/MachineLearning · /u/sulcantonin · Oct 14, 10:16

**「Additive event embeddings and linear decomposition」** Additive event embedding methods represent sequences as the sum of per-event vectors, enabling linear models to decompose scores exactly into per-event contributions—a property that supports interpretability in risk scoring, root-cause analysis, and fault diagnostics. Prior approaches like Word2Vec or Doc2Vec apply additive composition heuristically but lack training objectives that enforce exact arithmetic consistency between sequence history and individual event vectors; Event2Vec explicitly bridges this gap with a self-supervised reconstruction loss that enforces h\_t − h\_\{t−1\} = e\_\{x\_t\} \(up to norm clipping\).

**「Impact」** Practitioners in healthcare, system logging, and recommender systems can now use lightweight, interpretable linear models over summed event embeddings without sacrificing exact attribution of risk or score contributions to individual events—unlike opaque sequence models such as LSTMs or Transformers.

**Tags**: `#sequence-modeling`, `#interpretable-ml`, `#self-supervised-learning`, `#event-data`, `#embedding-methods`

---

<a id="item-tech-news-20"></a>
### [Three ICLR Submissions Share Identical Error-Difference Cancellation Technique](https://www.reddit.com/r/MachineLearning/comments/1x5dc8f/weird_pattern_in_the_iclr_papers_i_was_assigned/) ⭐️ 7.0/10

A reviewer assigned to three unrelated ICLR submissions observed that all three papers rely on the identical technical approach: comparing two predictors by analyzing the difference of their errors or scores, where a shared term cancels out—enabling tighter bounds—and then building elaborate theoretical frameworks around this cancellation. The papers also share nearly identical exposition style, phrasing, and structural patterns, leading the reviewer to suspect possible AI-assisted or template-driven generation. No evidence confirms coordinated authorship or tool use; the observation is anecdotal and limited to three papers in one reviewer’s assignment.

reddit · r/MachineLearning · /u/WhiteBear2018 · Oct 14, 00:28

**「ICLR&\#x27;s open peer review and theoretical ML norms」** ICLR has used an open peer review process since its founding in 2013, emphasizing transparency and community scrutiny of submissions. In theoretical machine learning, pairwise comparison—especially error-difference analysis with cancellation of shared terms—is a known technique for deriving tighter generalization bounds or ranking predictors, but it is not typically the sole conceptual foundation of multiple independent submissions to a top-tier conference.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/International_Conference_on_Learning_Representations">International Conference on Learning Representations - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#ICLR`, `#machine-learning-theory`, `#academic-integrity`

---

<a id="item-tech-news-21"></a>
### [Localized Neural Learning vs Backpropagation: Practical Advantages and Research Status](https://www.reddit.com/r/MachineLearning/comments/1x5itey/localized_neural_learning_vs_backpropagation_d/) ⭐️ 7.0/10

A Reddit user with a physics and mathematics background asks whether localized neural learning rules—such as Hebbian learning, Oja’s rule, and predictive coding—offer concrete practical advantages over backpropagation beyond theoretical or biological plausibility. They seek evidence of superior performance in specific contexts: unsupervised representation learning \(e.g., for molecular dynamics\), continual/online learning under non-stationary data, and resource-constrained or neuromorphic hardware. The query explicitly distinguishes vendor or research claims from empirically validated results, noting that some predictive coding formulations can approximate backpropagation and questioning how fundamentally distinct such alternatives really are.

reddit · r/MachineLearning · /u/Nearby\_Effective6679 · Oct 14, 05:16

**「Background」** Backpropagation is a gradient-based algorithm for computing weight updates in neural networks by propagating error signals backward from a global loss function, requiring non-local information and coordinated computation across layers. Predictive coding, Hebbian learning, and Oja’s rule are local alternatives that update weights using only pre- and post-synaptic activity or layer-local prediction errors—motivated by biological plausibility and hardware constraints—but some formulations \(e.g., predictive coding under fixed predictions\) have been shown to be algorithmically equivalent to backpropagation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Backpropagation">Backpropagation - Wikipedia</a></li>
<li><a href="https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0266102">On the relationship between predictive coding and backpropagation</a></li>
<li><a href="https://completeaitraining.com/course/biological-learning-algorithms-backpropagation-vs-predictive-coding-video-course/">Biological Learning Algorithms: Backpropagation vs Predictive ...</a></li>

</ul>
</details>

**Tags**: `#neural-computation`, `#backpropagation-alternatives`, `#biologically-plausible-ai`

---

<a id="item-tech-news-22"></a>
### [Google allows free private publishing of AI-generated apps to Play Store](https://www.bloomberg.com/news/articles/2026-10-13/google-will-let-anyone-publish-privately-listed-vibe-coded-apps-on-play-store) ⭐️ 7.0/10

Starting October 13, 2026, Google permits any user aged 18+ with a Google account to publish AI-generated Android apps—created exclusively in Google AI Studio—to the Play Store as privately listed apps, with no $25 developer registration fee required. These apps are non-discoverable: they do not appear in Play Store search, browse, or recommendations, and are intended for personal use only. The policy applies only to apps built in Google AI Studio; it does not extend to manually coded apps or apps generated by third-party AI tools. Google plans future support for limited sharing with friends and family but currently prohibits monetization beyond basic app functionality.

telegram · zaihuapd · Oct 13, 23:17

**「Background」** Prior to this change, publishing any app to the Play Store required registering as a Google Play developer and paying a one-time $25 fee. Google AI Studio, launched in 2024, is Google’s official low-code platform for building Android apps using natural language prompts and prebuilt components. This policy shift follows broader industry efforts—including Apple’s recent limited no-code app pilot—to accommodate AI-assisted development without traditional engineering workflows.

**「Impact」** Developers and non-developers alike can now deploy functional Android apps for internal or personal use without financial or administrative overhead—enabling rapid prototyping, internal tooling, and educational experimentation—but cannot distribute, monetize, or scale these apps publicly through Play Store discovery mechanisms.

**Tags**: `#AI development`, `#app distribution`, `#developer tools`, `#Google Play`, `#no-code`

---

<a id="item-tech-news-23"></a>
### [DeepMind and Singapore Launch On-Device Scam Detection Model Based on Gemma](https://deepmind.google/blog/on-device-ai-scam-detection-mddi/) ⭐️ 7.0/10

Google DeepMind and Singapore’s Government Technology Agency \(GovTech\) jointly launched an on-device AI scam detection model fine-tuned from Gemma, designed to analyze SMS and voice call dialogues directly on smartphones and issue real-time alerts without uploading data to the cloud. The model was demonstrated at the 2026 Singapore International Cyber Week and targets social engineering scams, which account for 80% of reported fraud losses in Singapore—totaling over S$4 billion since 2019. No technical specifications \(e.g., Gemma variant, quantization method, latency, accuracy metrics, or release timeline\) or availability details \(e.g., OS compatibility, rollout schedule, or open-source status\) were disclosed in the source material.

telegram · zaihuapd · Oct 14, 03:11

**「Background」** Gemma is Google DeepMind’s family of open-weight, lightweight language models, with the latest version—Gemma 4 12B Unified Transformer—released in June 2026. The Singapore Government Technology Agency \(GovTech\) is the national agency responsible for driving digital government and public-sector technology innovation, including cybersecurity initiatives like ScamShield.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/gemma/">Gemma — Google DeepMind</a></li>
<li><a href="https://www.tech.gov.sg/">Home | Government Technology Agency of Singapore ( GovTech ...)</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#edge AI`, `#cybersecurity`, `#privacy-preserving ML`, `#applied NLP`

---