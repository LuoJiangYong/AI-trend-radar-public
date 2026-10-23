# AI 资讯日报 · 第 004 期

2026-10-22（周四）· 覆盖 10-21 08:00 – 10-22 08:00（北京时间）· 收录 63 条，14/30 个 P1 账号有更新

## 01 今日趋势

过去 24 小时，时间线被一场 AI 发现的安全漏洞刷屏：OpenAI 称其 Patch the Planet 计划中的研究者借助 OpenAI 模型找到了 PHP 引擎的严重漏洞，这条帖子拿到约 1.3 万赞，是今天互动最高的一条；同一天还有印度证书机构弱私钥、Railway 和 TiDB Cloud 密钥泄露、GitLab 满分漏洞接连曝出。产品侧，据宝玉和 Gorden Sun 的帖子，Anthropic 推出会主动找你的个人助理 Claude Duet，「云端个人助理」两个多月里已有四家公司入场；Anthropic 官方同日发布年度公益报告并宣布信托新成员。科研上，OpenAI 的 GPT-Rosalind 给神经退行性疾病提出新线索，DeepMind 用 Gemini 4 Argon 做出交互式 3D 人体解剖图，Mistral 与英伟达合作工业工程 AI。云与算力继续交叉融合：OpenAI 模型登陆 Google Cloud，Meta 工程师确认已在生产中用 Google TPU 跑推理，Codex 的缓存也变得更长、更便宜。可灵 4.0 开放 API 并在 Runway、fal、Higgsfield 等平台上线。评测方面，Artificial Analysis 推出 AA-PersonalityBench，发现最老的几款模型最爱「讨好」用户。

### 一、AI 找漏洞进入「互联网级」：PHP 严重漏洞引爆安全时间线

OpenAI 表示，其 Patch the Planet 计划中的研究者借助 OpenAI 模型发现了 PHP 的严重安全漏洞（PHP 约支撑全球 70% 的网站），过去两个月牵头维护者、研究者和安全厂商提前准备修复，并称这是近年影响最大的漏洞之一，标志着「AI 能找到互联网级影响的安全漏洞」的新阶段；OpenAI 还打包了一个 Codex 技能，帮站长检查网站是否受影响。宝玉整理了细节：PHP 官方 10 月 21 日紧急发布 8.5.12、8.4.27、8.3.36、8.2.35，修补两个免登录即可接管服务器的漏洞（研究者称为 PHP2Shell），安全公司 Calif 用 GPT-5.6 Sol 找到漏洞。歸藏把它和印度证书机构 eMudhra 的弱私钥事件并称为当天安全圈两件大事；Ethan Mollick 说他接触的公司已经在为 AI 防御发现漏洞带来的补丁速度发愁，普通消费者也将经历频繁更新。宝玉当天还提醒了 Railway 密钥系统被入侵、TiDB Cloud 需轮换 API 密钥、GitLab 六周内第三个满分漏洞。

[@OpenAI](https://x.com/OpenAI/status/2112907856018309586) · [@OpenAI](https://x.com/OpenAI/status/2112945805686604033) · [@dotey](https://x.com/dotey/status/2112934529916616991) · [@op7418](https://x.com/op7418/status/2112931729547936037) · [@emollick](https://x.com/emollick/status/2112918582598459644) · [@dotey](https://x.com/dotey/status/2112959547039985972)

### 二、主动式个人助理之争：Claude Duet 登场，Anthropic 多线动态

宝玉介绍，Anthropic 发布新 App Claude Duet，目前是研究预览版：平时 Claude 要你打开对话框才干活，Duet 则会主动找你，美国 Pro 和 Max 用户可排队试用、不另收费；Gorden Sun 补充说它由 Opus 5.5 驱动，类似 Grok Bot。宝玉指出，两个多月里已有四家公司推出同类产品：xAI 的 Grok Bot（8 月 11 日）、Meta 的 Muse（9 月 8 日）、OpenAI 的 Dots（9 月 29 日）和 Anthropic 的 Claude Duet。注意：本期抓取的 @AnthropicAI 帖子中没有 Duet 的官方公告，相关信息来自上述转述。Anthropic 官方当天发布年度公益报告（Public Benefit Report），并宣布前哈佛大学理学院院长、实验物理学家 Christopher Stubbs 加入其长期利益信托；宝玉还整理了 Dario Amodei 回应「做安全还是抢超级智能」质疑的长文，Gorden Sun 则汇总了《华尔街日报》披露的 Anthropic 招股书草案细节。

[@dotey](https://x.com/dotey/status/2112995995017421133) · [@dotey](https://x.com/dotey/status/2113014531853365681) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113051791239872628) · [@AnthropicAI](https://x.com/AnthropicAI/status/2112966949273801086) · [@AnthropicAI](https://x.com/AnthropicAI/status/2112946750264676743) · [@dotey](https://x.com/dotey/status/2112754670338757051)

### 三、AI for Science：药物新线索、3D 解剖与工业仿真

OpenAI 称 GPT-Rosalind 为药物发现提出新线索：与 Perturb AI、斯克里普斯研究所合作，数千个 GPT-Rosalind 智能体并行工作，用 32 分钟把数百万个小鼠脑细胞的基因表达结果与文献联系起来，提出与佩里综合征相关基因 DCTN1 有关的假说——胆固醇可能没能送达神经元需要的位置，双方正扩大合作寻找新药物靶点。Google DeepMind 展示 Gemini 4 Argon 组合三个开源数据集，做出可分层查看、隔离肌肉、放大跳动心脏的交互式 3D 人体解剖可视化。Mistral 宣布与英伟达合作把 AI 带进工业工程：更快的仿真、面向物理 AI 的开放基准与数据集，以及 CAE 和 EDA 领域的智能体评测。

[@OpenAI](https://x.com/OpenAI/status/2112899854569762936) · [@GoogleDeepMind](https://x.com/GoogleDeepMind/status/2112974723659247896) · [@MistralAI](https://x.com/MistralAI/status/2112870261829603589)

### 四、云与算力交叉融合：OpenAI 上 Google Cloud，Meta 用 TPU，缓存更长更便宜

OpenAI 宣布把前沿模型和 Codex 智能体工作流带进 Google Cloud 的 Model Garden，让企业在已有的平台上使用。宝玉转述 Google 10 月 20 日的开发者博客：TPU 版 SGLang 推理引擎发布，Meta 的 PyTorch-TPU 负责人 Zongwei Zhou 表示「SGLang-TorchTPU 今天已经在 Meta 的生产环境中运行」；Gorden Sun 介绍 Google 开源的 TorchTPU，让 PyTorch 代码不必重写就能跑在 TPU 上。成本方面，宝玉称 Codex 和 Work 的登录用户缓存会永久保留，OpenAI API 的提示缓存可保留 12 小时（默认仍为 30 分钟，首次写入收原价 2.5 倍、读取只收 1 成）；Gorden Sun 对比称 Claude 客户端缓存 1 小时、API 5 分钟，DeepSeek API 缓存 3 天。

[@OpenAI](https://x.com/OpenAI/status/2112988118471295323) · [@dotey](https://x.com/dotey/status/2112788283251962092) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2112722598887039420) · [@dotey](https://x.com/dotey/status/2112775224236077393) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2112749963373686913)

### 五、可灵 4.0 开放 API，多平台同步上线

可灵宣布 Kling 4.0 API 正式开放，可接入产品和工作流，并相继宣布在 fal、Higgsfield 上线，还展示了在 Magnific 上的效果；Runway 也上线了「无限量 Kling 4」：新开 Max 或 Team 套餐可获 3 天无限使用，所有套餐 Kling 4 打 75 折。可灵还发布了韩国导演 Sung-soo Kim 的案例：他多年想拍的卡夫卡式「拥挤地铁车厢撞上巨型蠕虫」镜头靠 Kling 4.0 实现；并回顾了 10 月 14 日在洛杉矶科技周与 Oxen AI、Obsidian Studio 讨论 AI 视频如何进入企业内容生产。另外，Artificial Analysis 的视频竞技场迎来两周年。

[@Kling_ai](https://x.com/Kling_ai/status/2112946255257084260) · [@runwayml](https://x.com/runwayml/status/2112925874144030784) · [@Kling_ai](https://x.com/Kling_ai/status/2112928202880401556) · [@Kling_ai](https://x.com/Kling_ai/status/2112769091383836746) · [@Kling_ai](https://x.com/Kling_ai/status/2112861465833312488) · [@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2112992234140475837)

## 02 原始汇总

### 实验室与官方

![头像](https://pbs.twimg.com/profile_images/1991559933473497089/mbrRS49P_normal.jpg) **Hugging Face** (@huggingface) · 10-22 06:49

> Come and build models, datasets, and spaces on the hub, to win $20k in cash and credits! https://t.co/QQHsFaoFX9


♥ 25 · ↻ 7 · 💬 7 · [查看原帖](https://x.com/huggingface/status/2113039952963641570)

---

![头像](https://pbs.twimg.com/profile_images/1885410181409820672/ztsaR0JW_normal.jpg) **OpenAI** (@OpenAI) · 10-22 03:23

> OpenAI models are coming to Google Cloud.
> 
> We're bringing our frontier models and Codex agentic workflows to Google Cloud's Model Garden, so enterprises can use our technology where they already build.
> 
> https://t.co/gjuLVALjDm


♥ 2.6k · ↻ 176 · 💬 208 · [查看原帖](https://x.com/OpenAI/status/2112988118471295323)

---

![头像](https://pbs.twimg.com/profile_images/1695024885070737408/-M-HSH5P_normal.jpg) **Google DeepMind** (@GoogleDeepMind) · 10-22 02:30

> Gemini 4 Argon combined three open-source datasets to build an interactive 3D visualization of human anatomy.
> 
> Toggle different layers in motion, isolate muscles, or zoom inside a beating heart. https://t.co/60nfQ0QVkl

![配图](https://pbs.twimg.com/amplify_video_thumb/2112974557619302400/img/C5NXfnVigLrq4siZ.jpg)

♥ 1.3k · ↻ 110 · 💬 122 · [查看原帖](https://x.com/GoogleDeepMind/status/2112974723659247896)

---

![头像](https://pbs.twimg.com/profile_images/1798110641414443008/XP8gyBaY_normal.jpg) **Anthropic** (@AnthropicAI) · 10-22 01:59

> Anthropic is a Public Benefit Corporation. Today, we’re publishing our annual Public Benefit Report. This report shares our five pillars and takes stock of the actions we’re taking to advance them. 
> 
> Read the full report at this page: https://t.co/MTCgtzCoPH


♥ 1.8k · ↻ 154 · 💬 151 · [查看原帖](https://x.com/AnthropicAI/status/2112966949273801086)

---

![头像](https://pbs.twimg.com/profile_images/1798110641414443008/XP8gyBaY_normal.jpg) **Anthropic** (@AnthropicAI) · 10-22 00:38

> Dr. Christopher Stubbs is joining our Long-Term Benefit Trust. Chris is an experimental physicist and a former Dean of Science at Harvard University. He has also advised the US government on national security and arms control.
> 
> Read more: https://t.co/8RzH8UujRU


♥ 1.5k · ↻ 84 · 💬 122 · [查看原帖](https://x.com/AnthropicAI/status/2112946750264676743)

---

![头像](https://pbs.twimg.com/profile_images/1885410181409820672/ztsaR0JW_normal.jpg) **OpenAI** (@OpenAI) · 10-22 00:35

> If you are wondering whether your website is affected, we have packaged a Codex skill to help check.
> 
> Point your Codex at this repo to guide you through it: https://t.co/XUEbOwXuQC https://t.co/BDaIIaJ4yK


♥ 7.4k · ↻ 907 · 💬 268 · [查看原帖](https://x.com/OpenAI/status/2112945805686604033)

---

![头像](https://pbs.twimg.com/profile_images/1885410181409820672/ztsaR0JW_normal.jpg) **OpenAI** (@OpenAI) · 10-21 22:04

> OpenAI models helped researchers—operating as part of our Patch the Planet initiative—discover critical security flaws in PHP, an open-source programming language used to run an estimated 70% of websites.
> 
> Over the past two months, we led a coalition of maintainers, researchers, and security providers to prepare fixes and protections ahead of disclosure. This duration was necessary because the fix was quite intricate and required a major change to the PHP engine. Every site using PHP can now safely upgrade their version to stay secure, in addition to applying mitigations from various security vendors.
> 
> Due to the severity of these flaws and PHP’s widespread use, we consider this bug to be one of the most impactful vulnerabilities in recent memory. It also marks a new phase, where AI can find security bugs with internet-scale impact. 
> 
> This is an example of the Defender’s Window in action: to our knowledge, frontier AI was able to find this vulnerability ahead of attackers, giving defenders time to prepare.
> https://t.co/TW3jrSbB3f


♥ 13.3k · ↻ 2.7k · 💬 504 · [查看原帖](https://x.com/OpenAI/status/2112907856018309586)

---

![头像](https://pbs.twimg.com/profile_images/1885410181409820672/ztsaR0JW_normal.jpg) **OpenAI** (@OpenAI) · 10-21 21:32

> GPT-Rosalind surfaced a new lead for drug discovery: could restoring cholesterol transport protect neurons from degeneration?
> 
> DCTN1 is a gene linked to Perry syndrome, a rare neurodegenerative disorder. In mouse-brain data, disrupting it increased expression of genes involved in making cholesterol. GPT-Rosalind suggested a possible explanation: cholesterol may not be reaching where neurons need it.
> 
> That gives scientists a specific mechanism to test and, if confirmed, a direction for developing new treatments for neurodegenerative disorders.
> 
> With @perturbai_tx and @scrippsresearch, a team of thousands of GPT-Rosalind agents worked in parallel, connecting gene-expression results from millions of mouse brain cells with scientific literature in just 32 minutes. We’re now expanding this collaboration to identify new drug targets.
> 
> https://t.co/oHdF3ELsMj


♥ 5.4k · ↻ 554 · 💬 320 · [查看原帖](https://x.com/OpenAI/status/2112899854569762936)

---

![头像](https://pbs.twimg.com/profile_images/1996905418065375232/mzwynOLB_normal.jpg) **Mistral AI** (@MistralAI) · 10-21 19:35

> Today we’re announcing a new collaboration with @nvidia to bring AI to industrial engineering: 
> 
> - faster simulation
> - open benchmarks and supporting datasets for physics AI
> - evaluations for agentic AI in CAE and EDA
> 
> More here: https://t.co/HXFVBqJSP1 https://t.co/OTb24yjOUQ

![配图](https://pbs.twimg.com/media/HVJjJIKXUAAWj0d.jpg)

♥ 1.7k · ↻ 150 · 💬 101 · [查看原帖](https://x.com/MistralAI/status/2112870261829603589)

---

### 资讯与分析

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 05:00

> In AA-PersonalityBench, Gemini models are the most Confident and the least likely to Admit Uncertainty of all models measured
> 
> ➤ Most Confident: Gemini 3.8 Flash (100), Gemini 4 Argon (97) and Gemini 3.1 Pro Preview (95)
> ➤ Least likely to Admit Uncertainty: Gemini 3.1 Pro https://t.co/9jclv4e90N

![配图](https://pbs.twimg.com/media/HVLtkxlWEAA2HiD.jpg)

♥ 130 · ↻ 7 · 💬 9 · [查看原帖](https://x.com/ArtificialAnlys/status/2113012534513188912)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 03:39

> Two years ago today we launched the Artificial Analysis Video Arena, the leading crowdsourced comparison for Text to Video models
> 
> Since then, we have added leaderboards for Image to Video, Video with Audio, and Video Editing. Our initial leaderboard featured eight models - we https://t.co/elTmEy5fDC

![配图](https://pbs.twimg.com/amplify_video_thumb/2112992183708213248/img/dfkqSyNdWejj2yP7.jpg)

♥ 49 · ↻ 3 · 💬 6 · [查看原帖](https://x.com/ArtificialAnlys/status/2112992234140475837)

---

![头像](https://pbs.twimg.com/profile_images/1601382188712398850/3AAOlqrX_normal.jpg) **Ethan Mollick** (@emollick) · 10-22 02:04

> This is an interesting question because the answer is not obvious.
> 
> Which, by the way, does not mean AI coding tools are not leading to massive improvements, but, as research keeps showing, the bottlenecks to product improvements are often elsewhere. https://t.co/oluwSaMWRZ


♥ 184 · ↻ 6 · 💬 103 · [查看原帖](https://x.com/emollick/status/2112968222538686592)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 01:35

> HeyGen Voice Turbo takes the #1 spot on the Artificial Analysis Controlled Voice TTS Arena Leaderboard, with their previous model, HeyGen Voice, ranking #2
> 
> Just two weeks after reaching #1 with its previous model, @HeyGen has released HeyGen Voice Turbo, which now leads the https://t.co/wqL6DSHYa0

![配图](https://pbs.twimg.com/tweet_video_thumb/HVK0ulOWAAAFj5U.jpg)

♥ 82 · ↻ 6 · 💬 6 · [查看原帖](https://x.com/ArtificialAnlys/status/2112961069526249973)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 01:35

> In our new benchmark AA-PersonalityBench, GPT-4o, Llama 4 Maverick, and GPT-3.5 Turbo, the three oldest models measured, rank highest on the Sycophantic personality trait. Grok 4.7, Claude Fable 5.1, and Inkling rank lowest
> 
> ➤ @AIatMeta models are highly concentrated near the https://t.co/K248QXesio

![配图](https://pbs.twimg.com/media/HVK-j0SWUAAAqKZ.jpg)

♥ 713 · ↻ 37 · 💬 52 · [查看原帖](https://x.com/ArtificialAnlys/status/2112960933177770071)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 01:23

> Four models unexpectedly added the Sagrada Família’s magic square to their AA-3D scenes, offline and unprompted: Claude Fable 5.1 and Sonnet 5.5 featured it visibly, whereas Grok 4.7 and Step 5 Preview hid it behind a pillar
> 
> The sculptor Josep Maria Subirachs carved the square https://t.co/HI1DZHXbwE

![配图](https://pbs.twimg.com/amplify_video_thumb/2112957407186042881/img/Z2E1b3bYKo7boPRT.jpg)

♥ 80 · ↻ 3 · 💬 17 · [查看原帖](https://x.com/ArtificialAnlys/status/2112957875563987406)

---

![头像](https://pbs.twimg.com/profile_images/378800000261649705/be9cc55e64014e6d7663c50d7cb9fc75_normal.jpeg) **Simon Willison** (@simonw) · 10-22 00:28

> There's a French fork of Battle Drones with new models and music (and a cinematic intro video) and it is SO cool! https://t.co/7r9KELC7Vs
> 
> Here's the old v.s. new Goliath model https://t.co/FS0fNdca9d https://t.co/x9yKXVzeqm

![配图](https://pbs.twimg.com/media/HVKvexMa4AM-HuP.jpg)

♥ 65 · ↻ 8 · 💬 32 · [查看原帖](https://x.com/simonw/status/2112944161670488423)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-21 23:53

> We've updated MLCR-AA, our leaderboard for Wisedocs' Medical Long Context Reasoning benchmark, with Claude Sonnet 5.5 and GPT-6 Astra now tied for the #1 score
> 
> We've updated how MLCR-AA prompts and grades models on @wisedocsai's benchmark, to better reflect how medical record review is done in practice. Models are now prompted as medical record reviewers, and asked to answer each part of a question in one paragraph with their conclusion and the supporting evidence from the record. Answers are graded by a new three-model judge panel, and we reviewed all 60 expert reference answers against their source records, refining 15.
> 
> Claude Sonnet 5.5 (max with fallback) from @AnthropicAI and GPT-6 Astra (max) from @OpenAI are tied at the top with 41.7%, followed by GPT-6.1 Sol (max) at 38.3%. Qwen3.8 2.4T A95B from @Alibaba_Qwen is the leading open weights model at 30.6%.
> 
> Key results from the updated MLCR-AA:
> 
> ➤ Medical record review remains far from solved: an answer passes only when it is both complete and accurate, and no model passes more than 42% of questions and the median model passes under 15%
> 
> ➤ Anthropic models lead on completeness, reaching the expert's conclusion with the right medical reasoning: Claude models hold the top 18 completeness scores across every model and effort level we tested, led by Claude Sonnet 5.5 (max with fallback) at 64.8%. The best non-Anthropic model is GPT-6 Astra (max) at 42.2%
> 
> ➤ OpenAI models lead on accuracy, citing the record without exaggeration or hallucination: OpenAI models hold the top 27 accuracy scores, led by GPT-6.1 Sol (max) at 96.7%, but answer fewer questions completely: GPT-6.1 Sol (max) is complete on 40.0% of questions
> 
> We would like to thank Wisedocs for building MLCR and for their collaboration in bringing it to Artificial Analysis

![配图](https://pbs.twimg.com/media/HVKmYIbb0AAuF42.jpg)

♥ 179 · ↻ 15 · 💬 29 · [查看原帖](https://x.com/ArtificialAnlys/status/2112935427422527584)

---

![头像](https://pbs.twimg.com/profile_images/1601382188712398850/3AAOlqrX_normal.jpg) **Ethan Mollick** (@emollick) · 10-21 22:47

> Companies I talk to are struggling with the rate of patches they need to do thanks to AI defenses finding issues before the inevitable wave of incoming cyberattacks by other AIs.
> 
> Now consumers are going to have the same experience of getting everything updated often & fast. https://t.co/v2AlEk7EGV


♥ 335 · ↻ 17 · 💬 109 · [查看原帖](https://x.com/emollick/status/2112918582598459644)

---

![头像](https://pbs.twimg.com/profile_images/1601382188712398850/3AAOlqrX_normal.jpg) **Ethan Mollick** (@emollick) · 10-21 22:41

> Maybe, finally, voice interfaces in AI apps will kill the monstrosity that is the open office. Or just make them a lot worse as you.
> 
> (Thread of research on the problems of open offices below) https://t.co/uo9F9zWY9O


♥ 200 · ↻ 11 · 💬 73 · [查看原帖](https://x.com/emollick/status/2112917311107842130)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-21 13:10

> Devin Fusion with Claude Opus 5.5 (max) and a GPT-6 Luna (high) sidekick scores 68 on the Coding Agent Index, 2 points above Claude Code with Opus 5.5 (max) at 31% lower cost per task
> 
> @cognition's Devin Fusion runs a frontier lead model alongside a lower-cost sidekick model. The two work in parallel with their own context and tools, with the lead keeping planning, delegation and final review. We benchmarked Devin Fusion CLI with Claude Opus 5.5 (max) + GPT-6 Luna (high).
> 
> It scores 68.1 on the Artificial Analysis Coding Agent Index, closely matched at the top with Claude Code with Claude Sonnet 5.5 (max) at 68.4 and Muse Code with Muse Wonder Full (max) at 68.0. Against Claude Code with Claude Opus 5.5 (max) at 66.0, it costs $9.01 vs. $13.04 per task and averages 55 vs. 65 minutes per task.
> 
> Across the three benchmarks, the Fusion configuration scores higher on DeepSWE v1.1 (72.6% vs. 68.4%) and SWE-Atlas-QnA (69.6% vs. 66.4%) and slightly lower on Terminal-Bench 4.0 (62.1% vs. 63.1%). Its results reflect both models working together, including their combined API cost. Costs are pay-per-token API costs, not subscription prices.

![配图](https://pbs.twimg.com/media/HVIUH4dbkAAD8PY.jpg)

♥ 527 · ↻ 21 · 💬 105 · [查看原帖](https://x.com/ArtificialAnlys/status/2112773422698606736)

---

### 中文创作者

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 07:36

> Claude也发布云端个人助理了，名叫Claude Duet，类似Grok Bot，由Opus 5.5驱动，目前美国Pro和Max用户可以申请使用 https://t.co/EFqZv4GdwO


♥ 1 · ↻ 1 · 💬 1 · [查看原帖](https://x.com/Gorden_Sun/status/2113051791239872628)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 07:15

> 不聊天、只会涂答题卡的 AI：Jev 讲明白
> 
> Jev 其实发布有一阵了，还是值得科普一下，做了个简单的科普视频。
> 视频2 是中文版
> 
> Jev 只干一件事：像我们考试涂答题卡一样，在程序出好的选项里涂圈，涂的深浅就是它有几成把握。
> 
> 这期用一张答题卡讲清楚：
> 只会做选择题有什么用？ https://t.co/MICv24BAdz

![配图](https://pbs.twimg.com/amplify_video_thumb/2113045923337015296/img/aU2-wJ5LYAn_CKOe.jpg)
![配图](https://pbs.twimg.com/amplify_video_thumb/2113045941498306560/img/PrGRmSujF2R7yDqY.jpg)

♥ 17 · ↻ 2 · 💬 11 · [查看原帖](https://x.com/dotey/status/2113046543007641942)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 06:37

> Railway 存密钥的系统被入侵，部分可能已被解密；官方让所有用户立刻换掉全部密钥，部署暂停中
> 
> 在 Railway 上跑程序的开发者，现在就该把存在 Railway 里的环境变量全部换掉，包括 API 密钥、数据库密码和私有镜像仓库（存放打包好的程序）的登录凭证，再查查这些服务的日志。Railway 10 月 21 https://t.co/iCCzeLjqSd


♥ 15 · ↻ 2 · 💬 11 · [查看原帖](https://x.com/dotey/status/2113036984524423462)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 06:15

> 用 TiDB Cloud 的公司，现在就该去控制台把管理用的 API 密钥换一遍。PingCAP 10 月 20 日通知所有客户“不必等单独通知”，立刻轮换密钥、删掉不用的密钥、查日志有没有陌生操作。
> 
> TiDB Cloud 是 PingCAP https://t.co/c3R23U4ZrC


♥ 11 · ↻ 0 · 💬 5 · [查看原帖](https://x.com/dotey/status/2113031479685005601)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 05:08

> 两个多月里，四家公司都推出了同一类产品：xAI 的 Grok Bot（8 月 11 日）、Meta 的 Muse（9 月 8 日）、OpenAI 的 Dots（9 月 29 日），加上今天 Anthropic 的 Claude Duet。 https://t.co/CQoowSwn0e


♥ 138 · ↻ 14 · 💬 25 · [查看原帖](https://x.com/dotey/status/2113014531853365681)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 04:57

> GitLab 六周内第三个满分漏洞：不用登录就能控制服务器，2014 年以来的自建版本都要升级
> 
> 如果你们公司装了 GitLab，得赶紧升级了。10 月 21 日，GitLab 修复了一个满分 10 分的漏洞：在某些条件下，外人不用登录，就能在服务器上运行任意程序。2014 年的 7.0 版到现在，所有自建版本都受影响，10 月 https://t.co/6r4ONsCuJ7


♥ 29 · ↻ 5 · 💬 5 · [查看原帖](https://x.com/dotey/status/2113011845267116172)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 03:54

> Anthropic 推出 Claude Duet：会主动找你的 AI 助理，美国 Pro 和 Max 用户排队试用，不另收费
> 
> Anthropic 发布了一个新 App，叫 Claude Duet，目前是研究预览版，也就是早期测试版。
> 
> 平时用 Claude，是你打开对话框它才干活。Duet https://t.co/WL1byqkcKa


♥ 61 · ↻ 4 · 💬 24 · [查看原帖](https://x.com/dotey/status/2112995995017421133)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 02:49

> 这是Tim本人吗？ https://t.co/zBMNUS9oTA


♥ 8 · ↻ 0 · 💬 11 · [查看原帖](https://x.com/dotey/status/2112979572707013113)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 01:29

> 印度发证机构 eMudhra 8 枚“网站公章”密码小于 256，谁拿到都能冒充任何网站；浏览器已堵上，App 和设备要等更新
> 
> 你在手机上登录银行、购物网站，地址栏会有一把小锁。这把锁保证你连上的真是这家银行，没有人半路冒充。哪怕连的是咖啡馆里来路不明的 https://t.co/saAKBEC1Ac


♥ 28 · ↻ 4 · 💬 5 · [查看原帖](https://x.com/dotey/status/2112959547039985972)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 23:50

> PHP 曝两个免登录就能接管服务器的漏洞，AI 参与发现，所有 PHP 网站要马上升级
> 
> PHP 官方 10 月 21 日紧急发布 8.5.12、8.4.27、8.3.36、8.2.35，修补两个严重漏洞（CVE-2026-109618、CVE-2026-109619，研究者叫它 PHP2Shell）。按 PHP 官方的说法，攻击者不用登录，发特制请求就可能在服务器上执行任意代码，等于拿到整台服务器。WordPress、Drupal、Magento 都跑在 PHP 上，OpenAI 引用的估算是约 70% 的网站在用它。
> 
> 【我的 PHP 网站受影响吗】
> 
> 基本都在范围内。PHP 官方说，凡是对外处理网页请求的 PHP 都有风险，PHP-FPM、Apache mod_php、LiteSpeed 等常见跑法全包括，mod_php 风险最高。按 Wiz 和 Sansec 的说法，2012 年发布的 PHP 5.4 以来的版本都受影响。
> 
> 问题出在 PHP 引擎本身，好比大楼门锁坏了，你家装修得再好也没用。Wiz 和 Calif 已在最新版 WordPress、Drupal、Laravel 等上演示了免登录攻击。
> 
> 【现在该做什么】
> 
> 自己管服务器的：立刻升级到上面四个版本之一。PHP 8.1 及更早版本官方已停止维护，只给了 7.4、8.0、8.1 的源码补丁；用 Ubuntu、Debian 等发行版自带 PHP 的，看发行版的安全更新。
> 
> 用虚拟主机、托管 WordPress 的普通站长：PHP 由主机商管，装插件、改网站代码都修不了。去控制面板看 PHP 版本，或直接问主机商补了没有。
> 
> PHP 官方给的临时配置只能降低风险，官方明确说升级才是唯一完整的办法。Cloudflare 给所有用户（含免费版）上了拦截规则，但它自己也说只是临时挡一下，而且只管经过 Cloudflare 的流量，攻击者绕开它直连服务器就挡不住。
> 
> 【AI 立了什么功】
> 
> OpenAI 说，安全公司 Calif 在它的 Patch the Planet 计划里用 GPT-5.6 Sol 找到漏洞。据 Sansec 整理的时间线，Calif 8 月 11 日就报给了 PHP；Wiz 也独立发现并上报，用的是 Gemini 4 Argon 和 GPT-5.6 Sol 等工具。OpenAI 称两个月来牵头协调维护者和安全厂商准备修复，认为这是近年影响最大的漏洞之一，也是 AI 抢在攻击者前面发现漏洞的例子。
> 
> 【提前泄露了吗】
> 
> 属实。漏洞原定 10 月 22 日公开，20 日有人在 Hacker News 发帖提前曝光，帖子删了但截图已传开，PHP 官方随即把发布提前到 21 日。
> 
> 攻击已经开始。Cloudflare CTO 在补丁发布前几小时就说看到早期攻击；安全公司 watchTowr 说已有人用 AI 辅助写的工具发起攻击，"目前还没人成功，但不会太久"。荷兰政府的 DigiD 等网站先自行下线避险。
> 
> PHP 官方公告：https://t.co/UZYhjf3CWO
> OpenAI 原文：https://t.co/jKdbrEaMB8
> Wiz 技术说明：https://t.co/SrODSYiXOv


♥ 120 · ↻ 24 · 💬 27 · [查看原帖](https://x.com/dotey/status/2112934529916616991)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-21 23:49

> 笑死！即刻这哥们说
> 
> 问题的严重程度分别是轻度、中度、重度和印度 https://t.co/nFmyX3ZPFe https://t.co/YE7keZfX8m

![配图](https://pbs.twimg.com/media/HVKmkQvbEAAttgZ.jpg)

♥ 24 · ↻ 0 · 💬 2 · [查看原帖](https://x.com/op7418/status/2112934386475946308)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-21 23:43

> 全世界 70% 的网站都是 PHP 的，所以这个漏洞的影响真的很大 https://t.co/YE7keZfX8m


♥ 5 · ↻ 0 · 💬 2 · [查看原帖](https://x.com/op7418/status/2112932713900744986)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-21 23:39

> 今天安全领域的整个时间线上都是两件大事，对所有的互联网用户和产品应该都有影响。
> 
> 第一个是有个印度证书颁发机构用了一个非常容易被猜到的数字当做私钥：
> 
> 强度极弱，基本上任何人都能猜出来。
> 
> 其中一个私钥就是个位数"4"，原本长达七十多位的密钥变成了单个数字 4；剩下的也是 56、66、115、155 这种数字。
> 
> 这相当于给保险柜设了个密码"4"，试不到十下就能试出来。
> 
> 更离谱的是，多次审计居然都没发现这几个私钥有问题。
> 
> 目前 Chrome 和 Firefox 已经在几个小时内把这些私钥拉黑了，官方也把这 8 个私钥全部吊销。
> 
> 真是很难想象这个机构草台班子到了什么程度。
> 
> 现在浏览器端是安全的，但非浏览器端可能需要排查一下，尤其是你自己的项目如果涉及类似证书，建议让 AI 帮忙查一下。
> 
> 第二个是严重 PHP 漏洞：
> 
> 这个漏洞极其严重，官方说唯一真正安全的做法是立刻升级，但很多老旧网页已经多年没有升级过了。
> 更关键的是，有研究人员在 PHP 官方还没修复漏洞的情况下就直接公开了细节，导致所有人都能利用它发起攻击。
> 
> 该漏洞是 OpenAI 资助的 Patch the Plane 项目用 GPT-5.6 Sol 发现的，无需登录即可远程拿下服务器。
> 
> 漏洞覆盖面极大，比如大量依赖 PHP 的 WordPress 站点都会受到攻击。
> 
> 目前荷兰议会、荷兰国家安全中心、芬兰中央政府网站，以及日本著名的 Pixiv 应用都因此关闭了一段时间。
> 
> 感觉 AI 出来以后，攻防对抗变得异常剧烈，漏洞暴露和修复的频率都极快。
> 
> OpenAI 还表示，他们已经发现了更多具有这种规模效应的漏洞。

![配图](https://pbs.twimg.com/media/HVKkM-WaQAAKD6S.jpg)
![配图](https://pbs.twimg.com/media/HVKkM-VbQAETHgq.jpg)

♥ 60 · ↻ 6 · 💬 6 · [查看原帖](https://x.com/op7418/status/2112931729547936037)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-21 20:56

> 看了一堆解禁的 iPhone Duo 测评
> 
> 他妈的，还得是龙哥呀，一点儿不适配


♥ 87 · ↻ 0 · 💬 21 · [查看原帖](https://x.com/op7418/status/2112890839269888361)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 18:35

> 大肥鱼小法庭开庭啦！ https://t.co/PkUK0kadCN

![配图](https://pbs.twimg.com/amplify_video_thumb/2112855065547755520/img/MYEFkcWj8uYMOBh9.jpg)

♥ 36 · ↻ 3 · 💬 1 · [查看原帖](https://x.com/Gorden_Sun/status/2112855260066894157)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-21 17:15

> 最近让 AI 给电视去广告很火。
> 
> 昨天发了项目以后，很多朋友还是有一些问题，所以录了一个详细的教程 https://t.co/EZdW6gI5wD https://t.co/WhHDW317f3

![配图](https://pbs.twimg.com/amplify_video_thumb/2112835050668728320/img/kR6GYB_0caGdSyFk.jpg)

♥ 201 · ↻ 27 · 💬 30 · [查看原帖](https://x.com/op7418/status/2112835248870592903)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 17:13

> OrcaCyber-Nano-1.0：开源网络安全模型
> 
> 专为防御性网络安全打造的27B参数端侧视觉推理模型，支持输入文本和图片。
> 本地运行，支持逆向工程反编译、漏洞分析及代码审查，还能直接识别网络拓扑与反编译界面的截图。
> 
> 模型：https://t.co/HKfeJ1Cwoc


♥ 7 · ↻ 0 · 💬 7 · [查看原帖](https://x.com/Gorden_Sun/status/2112834702881226948)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 14:17

> 盘点AI公司的估值和营收 https://t.co/9GDpXsFRhi

![配图](https://pbs.twimg.com/amplify_video_thumb/2112789707491008512/img/QOCMn6-8yT4gJkzQ.jpg)

♥ 107 · ↻ 5 · 💬 10 · [查看原帖](https://x.com/Gorden_Sun/status/2112790406748684496)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 14:09

> Meta 工程师确认：Meta 已在正式业务里用 Google TPU 跑 AI 推理
> 
> 10 月 20 日，Google 在开发者博客发布 TPU 版 SGLang 推理引擎，文中引用了 Meta 的 PyTorch-TPU 负责人 Zongwei Zhou 的原话："SGLang-TorchTPU 今天已经在 Meta 的生产环境中运行。"这是目前唯一的一手确认。
> 
> TPU 是 Google 自研的 AI 芯片，对手是英伟达 GPU。推理就是 AI "上岗干活"，你每问一个问题，它算出答案就是一次推理。
> 
> Zongwei Zhou 没说规模多大、用在哪些产品、TPU 是租的还是买的。The Information 今年 2 月报道过，Meta 和 Google 签了多年、数十亿美元的 TPU 租用合同，两家没有公开细节。
> 
> Google 开发者博客：https://t.co/1pKn6zeugg
> PyTorch 博客：https://t.co/9MglhcELsd


♥ 46 · ↻ 3 · 💬 48 · [查看原帖](https://x.com/dotey/status/2112788283251962092)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 13:17

> 这些天以来目前为止最有价值更新：Codex 和 Work 的登录用户，缓存会永久保留，回到几小时前的旧对话或恢复会话，都保证命中缓存，没有“惩罚”（我理解是不会按照缓存失效收费）。
> 
> 怀疑是保存到磁盘了，那也很牛👍
> 
> 除此之外，OpenAI 开发者官方账号宣布，API 的提示缓存现在可以保留 12 小时，默认仍是 30 分钟。首次写入收原价 2.5 倍，之后读取缓存只收 1 成。
> 
> 官方文档：https://t.co/W2vqQNzbzQ


♥ 87 · ↻ 5 · 💬 82 · [查看原帖](https://x.com/dotey/status/2112775224236077393)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 12:12

> fin 的 AI 半导体终局推演系列都写到 4 了，这次讲的核心问题是：DeepSeek 这类谁都能下载的开源模型越来越便宜，OpenAI、Anthropic 会不会赚不到钱、没钱买 GPU？
> 
> fin 认为不会。
> 
> 第一个理由：价格降，成本降得一样快。
> 
> 每代新芯片让同样的电多产出约一倍的 token，软件优化每年再砍一半成本，利润率守得住。1GW 数据中心跑旗舰模型一年能卖 800 亿美元，硬件摊销每年只要约 80 亿。
> 
> 第二个理由：便宜模型和旗舰模型是两个市场。
> 
> 开源只能在低端打价格战，旗舰层只有 OpenAI 和 Anthropic 在争，价格稳。
> 
> 第三个理由：开源占 token 用量 20% 以上，按实际花的钱只占 5% 到 10%。
> 
> 模型越强，能接的长任务越多，需求还会涨。


♥ 132 · ↻ 8 · 💬 46 · [查看原帖](https://x.com/dotey/status/2112758776432304188)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 12:07

> DeepSeek 确实挺了不起的👍 https://t.co/aiOrjrN4NV


♥ 94 · ↻ 4 · 💬 11 · [查看原帖](https://x.com/dotey/status/2112757762677748106)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 11:55

> Anthropic 被质问“是在做安全还是在抢超级智能”，Dario 回应：三处沟通失误认了，路线不改
> 
> AI 安全组织 Encode 的法律总顾问 Nathan Calvin 10 月 19 日在 X 上发长文，质问 Anthropic 到底是安全组织，还是一心抢先造出超级智能的竞赛选手。Anthropic CEO Dario Amodei 随后亲自回复。
> 
> 起因是 Anthropic 私下给国会传阅的一份联邦 AI 法案草案。据 Politico 报道，按这份草案，政府要叫停一个 AI 模型，必须证明它迫在眉睫地可能造成 50 人以上死亡或重伤，或超过 10 亿美元损失。Calvin 认为门槛太高。
> 
> 【Calvin 的质疑】
> 
> Calvin 认为，Anthropic 过去一年的行动更像在全力赛跑，安全排在后面。Calvin 举的例子包括：签下约 5000 亿美元的算力协议；内部 AI 研发里由 Claude 主导的比例，从年初几乎为零涨到 8 月的 26%；改版安全规则，删掉了“风险控制不住就主动暂停”的承诺。
> 
> Calvin 的核心问题是：Anthropic 每次犯错，为什么都恰好对自己有利？法案里那么多太宽松的条款，为什么没有一处错在太严的方向？
> 
> 【Dario 的回应】
> 
> Dario 承认有些事是失误，但不同意 Calvin 的结论。
> 
> Dario 说，Anthropic 的策略一直是“向上竞争”：自己先做出负责任的样板，逼整个行业抬高标准，而这只有站在最前沿才管用。所以买算力、做芯片、用 AI 加速研发，在 Dario 看来是这条路线的正常动作。
> 
> Dario 还列了 Anthropic 为安全付出的商业代价：生物安全过滤严到生物学家拿来开玩笑；最强的 Mythos 级模型压了几个月才大范围开放；不向中国控股公司卖 AI 服务；本周拿出公司 5% 股份成立公益基金。
> 
> Dario 承认没处理好的是三件事：一封给国会的信、一句“没法在第二名的位置上做安全”，以及这份法案草案。Dario 说这些是话没写仔细、团队之间没同步，作为 CEO 他负责。删掉暂停承诺这一项，Dario 认为可以讨论，但坚持旧规则太死板，改是对的。
> 
> Calvin 原帖：https://t.co/d7vZNQQJzm


♥ 31 · ↻ 2 · 💬 20 · [查看原帖](https://x.com/dotey/status/2112754670338757051)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-21 11:43

> 今天看了 Every 的这篇《How Codex Happened》，整理的相当详细，其中对我感触最深的是关于 Codex Desktop 的这一段，看完才知道 Codex App 背后操刀的原来是 Tibo 和 Andrew Ambrosino。
> 
> 当时流行的都是 Cursor 这样的 IDE 内置聊天，但 Tibo 偏偏做了一件意外的决定：做一款原生桌面应用。
> 
> 他看到，模型能完成的任务越来越长，人们很快会同时开好几个智能体，一整天都和它们待在一起。他说：那就必须是一个非常丰富的界面，而不是一个 1970 年代的纯文本窗口。
> 
> 为此，他找来了设计师、程序员、前创业者 Andrew Ambrosino。
> 
> 他们没有像 Cursor 那样从 VS Code Fork 一个版本出来，虽然那是当时的标准做法；他们选择了参考聊天软件：左边是任务，每个任务一个智能体；右边是对话。
> 
> 然后，是最冒险的决定：应用里不放代码编辑器。
> 
> 想改代码？只能让智能体去改。
> 
> 因为一旦能敲代码，你就会期待编辑器的一切，一个四人小团队根本做不到。Codex 不可能靠当一个糟糕的编辑器取胜，它必须好到让你根本不想念编辑器。
> 
> 每天 Ambrosino 一进办公室就挨个问同时：“你在主力用 Codex 吗？”
> 
> 一开始，所有人的回答都是：没有。
> 
> 有同事在 Slack 上抱怨，就为了替换一句话，还得去提示 Codex。连 Ambrosino 自己也写道：不能编辑文件，是这次发布里我最怀疑的一点。
> 
> 2025 年 11 月，Google 发布了 Antigravity，一款把智能体和完整编辑器结合在一起的工具。主导它的，正是离开 Windsurf 的那批人。
> 
> Ambrosino 都开始自我怀疑：“我们是不是犯了一个巨大的错误？”
> 
> 更要命的是模型。就算应用做完了，以当时模型的质量，它也“无法发布”。
> 
> 然后，事情开始变了。11 月，GPT-5.1-Codex-Max 发布，能连续编码好几个小时。12 月，GPT-5.2-Codex 发布。独立的模型线，让团队不用顾虑八亿 ChatGPT 用户，可以迭代得更快。
> 
> 12 月，那位抱怨的同事改口了：我现在大多数改动，只留一条行内评论，飞快。Glaese 说：5.2 是个转折点。
> 
> 那年圣诞假期，整个行业迎来拐点：开发者们用 Opus 4.5 和 GPT-5.2 从头到尾搭出完整的应用，一行代码都不用自己写。
> 
> 2 月，Codex 应用在 OpenAI 内部流行开来。研究员 Noam Brown 说，他已经完全切换。Brockman，一个忠实的终端加 Emacs 用户，说回到老工作流，感觉像穿越回了过去。Altman 后来说，这是他们做过的最受内部喜爱的产品。
> 
> 可是别忘了，Codex Cloud 当初在内部也很受欢迎，结果一发布，就扑了街。
> 
> 这一次，会不一样吗？
> 
> ----
> 
> 完整的内容可以看原文 https://t.co/FAwjVxHjCW ，这个视频是我基于原文相应章节去搜集资料剪辑的。

![配图](https://pbs.twimg.com/amplify_video_thumb/2112748208300433408/img/1prW0pQv8NuY7JWC.jpg)

♥ 195 · ↻ 30 · 💬 68 · [查看原帖](https://x.com/dotey/status/2112751585671409696)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 11:36

> 普通用户使用Codex，是永久缓存命中了。通过API使用，则是缓存12小时。会非常节省费用，尤其是历史的长对话。
> Claude客户端目前是缓存1小时，API是缓存5分钟。
> DeepSeek API是缓存3天。 https://t.co/YCdUsUPMmQ


♥ 48 · ↻ 1 · 💬 34 · [查看原帖](https://x.com/Gorden_Sun/status/2112749963373686913)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 10:21

> phonon-31m-en：能在手机和浏览器本地流畅朗读的TTS模型
> 
> Gradium 团队基于 Pocket TTS 与 Mimi 音频编解码技术开发了 phonon-31m-en，把模型文件压缩到只有 64.5 MB，不需要显卡，可以直接运行在手机和电脑。
> 
> 支持边生成边播放的流式输出，声音自然清晰，即使在普通手机、笔记本电脑甚至浏览器网页标签页里也能丝滑运行，不需要联网就能独立完成英文语音合成。在多项盲测评分和生僻词朗读准确率上，表现都超过了 Kokoro 等同类开源模型，并且完全支持商用。仅支持英文。
> 
> 模型：https://t.co/qUdq37RTiQ


♥ 38 · ↻ 1 · 💬 11 · [查看原帖](https://x.com/Gorden_Sun/status/2112730896474481111)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 10:04

> Ornith-1.5-122B：媲美Qwen3.8-Flash-Next的开源模型
> 
> 122B总参数，10B激活参数，大多数评分超过Qwen3.8-Flash-Next。
> 上一代的Ornith-1.0版本基于Qwen3.5和Gemma4，这一代应该是做了更多的后训练。
> 
> 模型：https://t.co/rOl3A48xMp https://t.co/qDwj8dZDde

![配图](https://pbs.twimg.com/media/HVHp0HyasAEnrfL.jpg)

♥ 36 · ↻ 3 · 💬 6 · [查看原帖](https://x.com/Gorden_Sun/status/2112726791316209818)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 09:48

> 谷歌开源TorchTPU：让主流AI框架直接跑在谷歌TPU上
> 
> 目前绝大多数AI开发者都习惯使用PyTorch来编写和训练模型，但这类代码通常专门为英伟达显卡优化，很难直接高效运行在谷歌自研的TPU加速芯片上。
> 
> 谷歌团队开源了TorchTPU工具包，通过在底层定制专用的计算内核并接入代码编译缓存，用户只需在云端TPU主机上通过pip或构建工具Bazel安装该扩展包，就能无缝衔接现有工作流。
> 
> 接入后，开发者无需重写核心算法，就能直接调用谷歌TPU来训练和运行主流大模型（如Llama、Qwen等）。模型能够自动发挥TPU硬件在数据并行和张量并行上的多芯片协同加速能力，同时兼容主流的编译优化接口，大幅降低了使用谷歌硬件运行前沿AI模型的门槛和调试成本。
> 
> 项目地址：https://t.co/JyXAIjyY8K

![配图](https://pbs.twimg.com/media/HVHl_bQaYAA--AO.jpg)

♥ 21 · ↻ 1 · 💬 11 · [查看原帖](https://x.com/Gorden_Sun/status/2112722598887039420)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 09:35

> EAGLE-4：LLM推理加速工具
> 
> EAGLE-4 推理加速框架的核心机制是让一个小巧的辅助模型在前面飞速猜词，主模型只负责批量检查。用户不需要去改动底层模型，直接通过 Python 安装名为 eagle_harness 的扩展包，再搭配 SGLang 或 vLLM 这类主流大模型运行引擎就能启动。
> 
> 加速后的模型不仅不会降低回答质量，文字吐出速度还能直接翻倍。官方在英伟达顶级显卡上用 Qwen 模型实测，单人提问时生成速度能达到原本的近 3 倍；多任务并发处理时，每秒生成的文字数量也普遍比原本高出 35% 到 90%，大幅缩短了等待完整回答的时间。
> 
> 项目地址：https://t.co/UqqFxRDIUt

![配图](https://pbs.twimg.com/media/HVHjCiGaQAAC7hK.jpg)

♥ 32 · ↻ 5 · 💬 6 · [查看原帖](https://x.com/Gorden_Sun/status/2112719341649338707)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-21 09:28

> Anthropic上市前瞻
> 
> 根据《华尔街日报》披露的草拟招股书（S-1）细节，AI巨头 Anthropic 正加速推进其重磅 IPO 进程，市场预期估值或高达 2 万亿美元。
> 
> 1、营收爆发式增长，客户集中度偏高
> 
> · 上半年营收飙升：2026年上半年，公司营收达到约 163 亿美元，而去年同期仅为 11 亿美元，实现了爆发式跨越。
> · 客户高度集中：2026年上半年约五分之一（20%）的营收仅来自两家大客户。公司在招股书中直言，在可预见的未来，相当大比例的收入仍将依赖少数关键客户。
> 
> 2、财务表现：天量账面亏损与算力成本
> 
> · 807 亿美元净亏损：2026年上半年净亏损高达 807 亿美元（2025年同期为 130 亿美元）。不过，这一亏损主要由可转换票据及其他融资工具公允价值变动所产生的 720 亿美元非现金会计调整驱动，并非纯粹的实际现金消耗。
> · 激增的实际算力投入：2026年上半年，公司在计算能力和基础设施上的实际支出接近 90 亿美元，不仅远高于2025年同期的 23 亿美元，甚至直接超过了2025年全年的 73 亿美元支出总和。
> 
> 3、算力锁定：高达数百亿美元的刚性承诺
> 
> 为了支持下一代前沿模型的研发与服务，Anthropic 与各大云厂商及芯片租赁商绑定了巨额长期开支：
> 
> · 云协议与芯片租赁：未来7至10年内，公司承担了约 4500 亿美元的云服务协议，且绝大部分为不可撤销条款（其中包含与 Google 签署的 1110 亿美元、与 AWS 签署的 1100 亿美元以及与微软签署的 310 亿美元协议）。
> · 总承诺或冲至 7500 亿美元：叠加与 Broadcom 的 1600 多亿美元芯片租赁等项目后，其未来的基础设施支出已超 6000 亿美元；若加上目前仍在谈判中的算力协议，未来承诺总额可能进一步攀升至 7500 亿美元。
> 
> 4、核心风险
> 
> 在招股书中，风险因素披露占据了约三分之一的篇幅：
> 
> · 模型失控与法律责任：文件提及 AI 模型可能出现“自我保护”行为甚至类似“勒索”的表现以规避关闭风险；若失控模型引发灾难性安全事故或大规模数据泄露，公司可能承担直接赔偿责任，甚至可能因损失规模过大而面临无法获得商业保险承保的困境。
> · 算力依赖与竞合矛盾：主流云服务商（如微软、亚马逊等）正将 Anthropic 视作竞争对手，能提供的算力配额逐渐触及上限。公司虽转向自建数据中心或与第三方小型算力运营商合作，但面临后者运营经验不足及稳定性不及头部厂商的挑战。
> · 数据中心落地的政治阻力：数据中心扩张在多地引发了愈发有组织、跨管辖区的社区与环保抗议，这对 Anthropic 的全球基础设施扩建构成阻碍。


♥ 11 · ↻ 0 · 💬 11 · [查看原帖](https://x.com/Gorden_Sun/status/2112717579395735990)

---

### 视频图像与音乐

![头像](https://pbs.twimg.com/profile_images/1826028197256822784/pfgqU218_normal.jpg) **Midjourney** (@midjourney) · 10-22 03:11

> Midjourney Weekly Office Hours - 10/21 https://t.co/G4PW2wJ5FH


♥ 11 · ↻ 2 · 💬 6 · [查看原帖](https://x.com/midjourney/status/2112985137193566330)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:55

> A little Kling magic on Magnific. ✨ #Kling4 #KlingAI https://t.co/y44wQ6GOaM


♥ 24 · ↻ 3 · 💬 3 · [查看原帖](https://x.com/Kling_ai/status/2112950925614530753)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:52

> Saddle up for #Kling4 🤠 #KlingAI https://t.co/96BlL8BECG


♥ 27 · ↻ 5 · 💬 1 · [查看原帖](https://x.com/Kling_ai/status/2112950065790603265)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:48

> Unlimited Kling 4.0? Say less 🙌 #Kling4 #KlingAI https://t.co/UdNV17Kymj


♥ 36 · ↻ 1 · 💬 2 · [查看原帖](https://x.com/Kling_ai/status/2112949237743018319)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:36

> KLING 4.0 API — Officially Rolling Out Now
> 
> Integrate Kling 4.0 into your products and workflows. Let’s build. 🚀 #Kling4 #KlingAI https://t.co/Eec6OKqNc1

![配图](https://pbs.twimg.com/media/HVKxZ72XUAA051O.jpg)

♥ 97 · ↻ 9 · 💬 16 · [查看原帖](https://x.com/Kling_ai/status/2112946255257084260)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:35

> KLING 4.0 API — Officially Rolling Out Now
> 
> Integrate Kling 4.0 into your products and workflows. Let’s build. 🚀 #Kling4 #KlingAI


♥ 0 · ↻ 0 · 💬 0 · [查看原帖](https://x.com/Kling_ai/status/2112945976470069358)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:19

> KLING 4.0 API Now Opening
> 
> Integrate Kling 4.0 into your products and workflows. Let’s build. 🚀 #Kling4 #KlingAI

![配图](https://pbs.twimg.com/media/HVKsMTxWcAAsxNT.jpg)

♥ 7 · ↻ 2 · 💬 0 · [查看原帖](https://x.com/Kling_ai/status/2112941918367678573)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 00:14

> KLING 4.0 API Now Open
> 
> Integrate Kling 4.0 into your products and workflows. Let’s build. 🚀 #Kling4 #KlingAI

![配图](https://pbs.twimg.com/media/HVKsMTxWcAAsxNT.jpg)

♥ 5 · ↻ 1 · 💬 1 · [查看原帖](https://x.com/Kling_ai/status/2112940577150955857)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-21 23:25

> Now live on Higgsfield. Ready to roll. #KlingAI #Kling4 https://t.co/BRf0Srfhl9


♥ 54 · ↻ 4 · 💬 5 · [查看原帖](https://x.com/Kling_ai/status/2112928202880401556)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-21 23:25

> Bring your next video idea to life with Kling 4.0, now available on fal. #Kling4 #KlingAI https://t.co/5xN6S4jIm3


♥ 49 · ↻ 1 · 💬 4 · [查看原帖](https://x.com/Kling_ai/status/2112928160312643931)

---

![头像](https://pbs.twimg.com/profile_images/1999115192232292353/zOq5-uwB_normal.jpg) **Runway** (@runwayml) · 10-21 23:15

> Unlimited Kling 4 is now live on Runway.
> 
> Sign up for a new Max or Team plan to get 3 days of unlimited access. Plus 25% off Kling 4 on all plans. Get started at the link below. https://t.co/AthV6pDo0c

![配图](https://pbs.twimg.com/amplify_video_thumb/2112925258445418496/img/71p1fmAGEEqkhLBE.jpg)

♥ 94 · ↻ 11 · 💬 21 · [查看原帖](https://x.com/runwayml/status/2112925874144030784)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-21 19:00

> On October 14, Kling AI joined Oxen AI and Obsidian Studio at LA Tech Week 2026 to explore how AI video is becoming part of enterprise content production.
> 
> Drawing on commercial production experience, the panel discussed how creative capabilities become repeatable workflows and support advertising and film projects, from shot creation and revision through final delivery.
> 
> As production needs grow more complex, Kling 4.0 improves stability across complex motion and camera movement. Kling AI will keep working with partners worldwide to bring AI video into more enterprise production workflows and help more ideas reach the screen.

![配图](https://pbs.twimg.com/media/HVJXx78aYAAGVRy.jpg)
![配图](https://pbs.twimg.com/media/HVJXx8AbQAA0kcq.jpg)
![配图](https://pbs.twimg.com/media/HVJXx8CaEAAyw3F.jpg)
![配图](https://pbs.twimg.com/media/HVJXx7waUAAzvtI.jpg)

♥ 33 · ↻ 2 · 💬 11 · [查看原帖](https://x.com/Kling_ai/status/2112861465833312488)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-21 12:52

> A packed subway car. Passengers collide with a giant worm. It’s the Kafka-inspired scene Korean director Sung-soo Kim had wanted to bring to life for years.
> 
> Watch Kim share his first experience with AI filmmaking and explain how Kling 4.0 made the “impossible” shot possible. https://t.co/GRFm7TZM9u

![配图](https://pbs.twimg.com/media/HVIQA3qbgAALhQt.jpg)

♥ 80 · ↻ 7 · 💬 22 · [查看原帖](https://x.com/Kling_ai/status/2112769091383836746)

---
