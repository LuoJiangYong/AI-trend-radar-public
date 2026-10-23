# AI 资讯日报 · 第 005 期

2026-10-23（周五）· 覆盖 10-22 08:00 – 10-23 08:00（北京时间）· 收录 60 条，14/30 个 P1 账号有更新

## 01 今日趋势

过去 24 小时，安全仍是时间线的主线，但话题从「AI 找到漏洞」转向「怎么守住」：Anthropic 在 Frontier Red Team 博客上介绍用 Claude 大规模做软件形式化验证，拿到约 2300 赞，是今天互动最高的一条；OpenAI 公布今夏邀请 METR 和 Redwood Research 深入评估其内部监控系统。与此同时，Node.js 三条版本线修补高危漏洞，Gorden Sun 一口气列出 PHP、Node.js、GitLab、LiteLLM、eMudhra、Railway 六处漏洞，Ethan Mollick 形容这是攻防都在以「非人速度」加速。评测方面，Artificial Analysis 继续放出 AA-PersonalityBench 结果，并上线 CritPt v2 物理题评测和 DeepSeek Search 的搜索榜成绩。资本与开源侧，宝玉转述彭博社报道称 DeepSeek 新一轮融资约 1000 亿元（公司尚未确认），多款小参数开源模型密集发布。创作工具上，可灵 4.0 接入 Adobe Firefly 等平台，Codex 与 Claude Code 的玩法和额度成了中文圈的日常话题。

### 一、从找漏洞到防漏洞：Claude 做大规模形式化验证，OpenAI 请外部机构审监控系统

Anthropic 在 Frontier Red Team 博客发文，介绍用 Claude 对软件做大规模形式化验证：形式化验证能证明代码不含某类 bug，但过去只适用于小代码库或需要大量专家时间，帖子称 AI 模型正在改变这一点。OpenAI 则披露，今年夏天邀请 METR 和 Redwood Research 对其内部监控系统做为期三周的嵌入式评估，给予了深入的基础设施访问权限，称他们的发现帮助加强了扩展系统时的防护措施。两家头部实验室同一天把重点放在「验证与监督」上。

[@AnthropicAI](https://x.com/AnthropicAI/status/2113390212911083894) · [@OpenAI](https://x.com/OpenAI/status/2113298833392496746)

### 二、漏洞潮持续：Node.js 三线高危修复，攻防在「非人速度」上加速

宝玉整理了 Node.js 10 月 21 日的安全更新：22.x、24.x、26.x 三条维护线都修了高危漏洞，最严重的 Brotli 解压组件越界写入可能导致远程代码执行，另有三处 HTTPS 证书核对可被不规范 IP 写法绕过，已停止维护的 20.x 和 25.x 没有补丁；同时拉黑 eMudhra 的 8 枚问题证书。Gorden Sun 感叹两天里冒出 PHP RCE、Node.js、GitLab、LiteLLM、eMudhra CA、Railway 一串漏洞，并转发了 PHP RCE 的科普视频；宝玉还转述卡普空确认 CAPCOM ID 遭攻击，影响 11,774,247 个账户。Ethan Mollick 的评论获约 1900 赞：这是 AI 圈自 Mythos 发布以来一直警告的情况，攻击和防御都以非人的速度加速，而需要响应的却是人类系统。

[@dotey](https://x.com/dotey/status/2113067412979433847) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113085000254165124) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113222561849119064) · [@dotey](https://x.com/dotey/status/2113312593821794320) · [@emollick](https://x.com/emollick/status/2113063313810792916) · [@dotey](https://x.com/dotey/status/2113120595651297771)

### 三、评测密集更新：模型「性格」、物理研究题、搜索 API 与医疗问答

Artificial Analysis 继续发布 AA-PersonalityBench 结果：Anthropic 模型整体信息密度最高、文字最有素养（Claude Fable 5.1 信息密度 100 分）；能力越弱的模型通常「Slop」越多，但前沿模型之间差异仍大，GPT-6 Sol 与 Muse Spark 1.3 智能指数同为 48，在 Slop 榜上却分列第 1 和第 80。它还上线 CritPt v2（70 道研究级物理题经作者复核，模型可用代码执行工具作答），给 DeepSeek Search 打出 69 分（27 款搜索产品中第 17，且是榜上最便宜的付费搜索 API），并比较了医疗长上下文推理与 HealthBench Professional：Anthropic 模型回答最完整，OpenAI 模型更准确简洁。蚂蚁的 0.5B 参数 TTS 模型 Ming-3.0-tts 进入其语音合成榜前三。

[@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2113247130122944963) · [@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2113402182292648369) · [@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2113332770940629284) · [@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2113124084410425362) · [@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2113089188161782208) · [@ArtificialAnlys](https://x.com/ArtificialAnlys/status/2113380805552857591)

### 四、DeepSeek 传出千亿元融资，小参数开源模型扎堆发布

宝玉转述彭博社 10 月 21 日的独家报道：DeepSeek 新一轮融资约 1000 亿元人民币（约 150 亿美元），宁德时代和腾讯出资最多，公司尚未官方确认。开源侧，Gorden Sun 当天连发多条：RecursiveSI 开源编程模型 flint（40B 总参数、2.5B 激活、262K 上下文），韩国魁匠团开源 MoE 模型 Raon-1-mini-preview（29B 总参数、4.3B 激活），英伟达开源 Nemotron 3.5 Parse、Embed、Rerank 检索系列，以及仅 163 MB 的语音转文字模型 Underdog Bark 3.0；Hugging Face 也发帖称连监管最严的行业都在转向开源。

[@dotey](https://x.com/dotey/status/2113124395321360646) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113210097442984185) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113115220310913198) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113114045591285817) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113141081026224479) · [@huggingface](https://x.com/huggingface/status/2113289455121342950)

### 五、创作者工具：可灵 4.0 接入 Firefly，Codex 与 Claude Code 成日常话题

可灵连发多条，宣布 Kling 4.0 已接入 Adobe Firefly、OnSolo、OiiOii，并在 LA Tech Week 上和 Oxen AI、Obsidian Studio 讨论 AI 视频进入企业内容生产。编程助手方面，歸藏把 Codex 连上了电视直接对话，Ethan Mollick 分享了一条 Codex 配合电脑操作的实用提示词，Gorden Sun 演示用 Opus 5.5 生成素材替代整套生成加剪辑工作台；宝玉介绍了 Claude Code 任务卡片可转到云端执行，也吐槽 Codex 订阅额度和 28 天重置。Ethan Mollick 还给出一组对比：他的上一本书出版时 AI 能以 50% 成功率完成约 4 分钟的人类工作，新书交稿时是 17 小时，出版时已到 17 周。

[@Kling_ai](https://x.com/Kling_ai/status/2113135088091476358) · [@Kling_ai](https://x.com/Kling_ai/status/2113072850802196961) · [@op7418](https://x.com/op7418/status/2113101644334551095) · [@emollick](https://x.com/emollick/status/2113361252173091114) · [@Gorden_Sun](https://x.com/Gorden_Sun/status/2113325149978337318) · [@dotey](https://x.com/dotey/status/2113067847429632059) · [@dotey](https://x.com/dotey/status/2113299677785542772) · [@emollick](https://x.com/emollick/status/2113323645284344215)

## 02 原始汇总

### 实验室与官方

![头像](https://pbs.twimg.com/profile_images/1798110641414443008/XP8gyBaY_normal.jpg) **Anthropic** (@AnthropicAI) · 10-23 06:01

> New on our Frontier Red Team blog: using Claude to formally verify software at large scale.
> 
> Formal verification can prove that code is free of certain bugs, but historically it has only been feasible for small codebases (or required a lot of expert time).
> 
> With AI models,


♥ 2.3k · ↻ 204 · 💬 204 · [查看原帖](https://x.com/AnthropicAI/status/2113390212911083894)

---

![头像](https://pbs.twimg.com/profile_images/1885410181409820672/ztsaR0JW_normal.jpg) **OpenAI** (@OpenAI) · 10-22 23:57

> This summer, we invited METR and Redwood Research to pilot an embedded evaluation of our internal monitoring system, providing deep access to our infrastructure over three weeks. 
> 
> Their findings helped strengthen safeguards as we expanded the system and will help shape future https://t.co/F9DSyjEOr1


♥ 1.9k · ↻ 122 · 💬 273 · [查看原帖](https://x.com/OpenAI/status/2113298833392496746)

---

![头像](https://pbs.twimg.com/profile_images/1991559933473497089/mbrRS49P_normal.jpg) **Hugging Face** (@huggingface) · 10-22 23:20

> Even the most regulated industries are going open-source 🤗 https://t.co/BfLlVdQZo6


♥ 112 · ↻ 14 · 💬 42 · [查看原帖](https://x.com/huggingface/status/2113289455121342950)

---

![头像](https://pbs.twimg.com/profile_images/1695024885070737408/-M-HSH5P_normal.jpg) **Google DeepMind** (@GoogleDeepMind) · 10-22 22:38

> Not all forests are equal, and now we can map the difference. 🌳
> 
> Meet Forest Typology (ForTy): a 10m map of natural, planted, and farmed forests to help identify deforestation and protect the forests that matter most. 🧵 https://t.co/JoIOTkiZcT

![配图](https://pbs.twimg.com/tweet_video_thumb/HVPfO3QXkAAphKe.jpg)

♥ 505 · ↻ 56 · 💬 94 · [查看原帖](https://x.com/GoogleDeepMind/status/2113278710795153785)

---

### 研究者与领袖

![头像](https://pbs.twimg.com/profile_images/1990472620614053888/xrAu0wQL_normal.jpg) **Demis Hassabis** (@demishassabis) · 10-23 03:30

> Honoured to be featured in the @WSJ Innovators Issue. I’ve always believed in the power of human ingenuity to solve our hardest problems. I’m confident we can collectively navigate the potential challenges of frontier models and usher in a new golden age of scientific discovery! https://t.co/44e74aJppd


♥ 1.3k · ↻ 84 · 💬 86 · [查看原帖](https://x.com/demishassabis/status/2113352276026990972)

---

### 资讯与分析

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-23 06:48

> In AA-PersonalityBench, less intelligent models generally produce more Slop, but Slop still varies widely among frontier models
> 
> ➤ Same intelligence level but opposing Slop rankings: GPT-6 Sol and Muse Spark 1.3 both score 48 on the Intelligence Index, yet rank 1 and 80 on Slop https://t.co/snkFBpGlnn

![配图](https://pbs.twimg.com/media/HVRQD6xWQAAfH-x.jpg)

♥ 63 · ↻ 6 · 💬 14 · [查看原帖](https://x.com/ArtificialAnlys/status/2113402182292648369)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-23 05:23

> Ant Group's Ming-3.0-tts fits top-tier Text to Speech quality into just 0.5B parameters, and it is MIT licensed and punches well above its weights
> 
> It is the only model under 1B parameters in the top 3 of any of our Text to Speech leaderboards. Every other open weights TTS model https://t.co/K611aEN5KJ

![配图](https://pbs.twimg.com/tweet_video_thumb/HVQ8jGnasAAzEh2.jpg)

♥ 127 · ↻ 8 · 💬 13 · [查看原帖](https://x.com/ArtificialAnlys/status/2113380805552857591)

---

![头像](https://pbs.twimg.com/profile_images/1601382188712398850/3AAOlqrX_normal.jpg) **Ethan Mollick** (@emollick) · 10-23 04:06

> Very useful prompt for Codex with computer use. https://t.co/tOCwIo3JOy

![配图](https://pbs.twimg.com/media/HVQq25hW8AA1afL.jpg)

♥ 361 · ↻ 20 · 💬 36 · [查看原帖](https://x.com/emollick/status/2113361252173091114)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-23 04:02

> Subquadratic has released SubQ Snap 1.1, tying d1-ultra and Elephant 9B for first on the Artificial Analysis Decision Index v1.0, driven by a low hallucination rate
> 
> SubQ Snap 1.1 is the new decision model from @subquadratic. It is priced at $0.04 per 1M input tokens and supports https://t.co/azzQUhBSUL

![配图](https://pbs.twimg.com/media/HVQoyMIaQAAN_0r.jpg)

♥ 80 · ↻ 7 · 💬 13 · [查看原帖](https://x.com/ArtificialAnlys/status/2113360449156890662)

---

![头像](https://pbs.twimg.com/profile_images/378800000261649705/be9cc55e64014e6d7663c50d7cb9fc75_normal.jpeg) **Simon Willison** (@simonw) · 10-23 03:47

> Spotted a familiar creature at 00:45s in this new music video for FREEDOM by De Staad https://t.co/AEIsAkro77 https://t.co/voZuAsGX17

![配图](https://pbs.twimg.com/amplify_video_thumb/2113356400651046913/img/NVpKP3CPesN3gSM1.jpg)

♥ 122 · ↻ 1 · 💬 6 · [查看原帖](https://x.com/simonw/status/2113356466770121166)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-23 02:12

> CritPt v2 has launched on Artificial Analysis: the CritPt authors have reviewed all 70 research-level physics challenges, and models now solve them with a code-execution tool
> 
> Following feedback from the research community, the CritPt team and physics expert collaborators https://t.co/CU8KBiEJ9N

![配图](https://pbs.twimg.com/media/HVQQykjbUAAFDJ_.jpg)

♥ 183 · ↻ 8 · 💬 15 · [查看原帖](https://x.com/ArtificialAnlys/status/2113332770940629284)

---

![头像](https://pbs.twimg.com/profile_images/1601382188712398850/3AAOlqrX_normal.jpg) **Ethan Mollick** (@emollick) · 10-23 01:36

> When my first AI book was published in 2024, the best AI could do 4 minutes of human work with a 50% chance of success
> 
> When I turned in the draft of Co-Existence earlier this year, it was 17 hours
> 
> When it was published two days ago, AI could do 17 weeks https://t.co/ON0qKpJ6LD https://t.co/d97kFWQ3B4

![配图](https://pbs.twimg.com/media/HVQIpyrXAAAuH48.jpg)

♥ 497 · ↻ 51 · 💬 112 · [查看原帖](https://x.com/emollick/status/2113323645284344215)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-23 01:26

> Build your own custom personality suite using AA-PersonalityBench evaluated Personality Traits https://t.co/sfHVuVrgto

![配图](https://pbs.twimg.com/amplify_video_thumb/2113320891996049408/img/TAK28v3Q1cHtg1Oo.jpg)

♥ 43 · ↻ 2 · 💬 5 · [查看原帖](https://x.com/ArtificialAnlys/status/2113321019209392243)

---

![头像](https://pbs.twimg.com/profile_images/1451191636810092553/kpM5Fe12_normal.jpg) **AK** (@_akhaliq) · 10-22 22:44

> Looking Ahead
> 
> Modeling Future Evolution in Autoregressive Video Generation
> 
> paper: https://t.co/DRdK9bigNZ https://t.co/jQRbx7m2et

![配图](https://pbs.twimg.com/amplify_video_thumb/2113280245507751936/img/qmKb55r7NpV96hwj.jpg)

♥ 44 · ↻ 11 · 💬 12 · [查看原帖](https://x.com/_akhaliq/status/2113280305301971067)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 20:32

> In AA-PersonalityBench, Anthropic models are generally the most Information Dense and Literate of all models measured
> 
> ➤ Most Information Dense: Claude Fable 5.1 (100), Claude Opus 5.5 (97), Claude Sonnet 5.5 (95) and Claude Haiku 5.5 (92)
>  ➤ Most Literate: Claude Haiku 5.5 https://t.co/W9KoYp51IH

![配图](https://pbs.twimg.com/media/HVPCdoxXYAATL8q.jpg)

♥ 455 · ↻ 23 · 💬 60 · [查看原帖](https://x.com/ArtificialAnlys/status/2113247130122944963)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 12:23

> DeepSeek Search debuts on the Artificial Analysis Search Index at 69, 17th of 27 search products, at the lowest price of any paid Search API on the board
> 
> @deepseek_ai launched its Search API on 17 October. We benchmarked it in our Stirrup agent harness, where GPT-5.6 Luna https://t.co/5OEwFx1PQt

![配图](https://pbs.twimg.com/media/HVNS1FpaIAAsGtx.jpg)

♥ 439 · ↻ 21 · 💬 35 · [查看原帖](https://x.com/ArtificialAnlys/status/2113124084410425362)

---

![头像](https://pbs.twimg.com/profile_images/2042402069320290304/A8C1lP07_normal.jpg) **Artificial Analysis** (@ArtificialAnlys) · 10-22 10:04

> On MLCR-AA and HealthBench Professional, Anthropic models give the most complete answers but OpenAI models are more accurate and concise
> 
> We compared 14 models with results on both MLCR-AA, our leaderboard for @wisedocsai's Medical Long Context Reasoning benchmark, and @OpenAI's HealthBench Professional. MLCR-AA grades answers about long medical records on completeness (covering every key point of the expert's answer) and accuracy (no claim contradicting the record), and its score requires both. HealthBench Professional grades replies to clinicians against physician-written rubrics: the raw score is the share of rubric points earned, while the length-adjusted score penalizes longer answers.
> 
> Key takeaways:
> 
> ➤ Anthropic models lead on completeness and raw score: Claude Sonnet 5.5, Opus 5.5 and Fable 5.1 (all max with fallback) from @AnthropicAI hold the top three MLCR-AA completeness scores, ~19-23 points ahead of the best OpenAI model, and Opus and Sonnet post the highest HealthBench Professional raw scores (71.4% and 70.8%), narrowly ahead of GPT-6 Astra (69.7%)
> 
> ➤ OpenAI models lead on accuracy and conciseness: OpenAI models hold the top MLCR-AA accuracy scores. Longer answers are less likely to be judged accurate, as each extra claim is another chance to contradict the record: Anthropic models write ~4-6x more per answer than OpenAI models, and score 19-61% on accuracy against 89-97%
> 
> ➤ The gap closes on scores that reward both: GPT-6 Astra (max) ties Claude Sonnet 5.5 for #1 on MLCR-AA and narrowly leads the HealthBench Professional length-adjusted score, while Claude Opus 5.5 falls from #1 on the raw score to #6 length-adjusted

![配图](https://pbs.twimg.com/media/HVMy0gFbsAAw1Sa.jpg)

♥ 71 · ↻ 4 · 💬 19 · [查看原帖](https://x.com/ArtificialAnlys/status/2113089188161782208)

---

![头像](https://pbs.twimg.com/profile_images/1601382188712398850/3AAOlqrX_normal.jpg) **Ethan Mollick** (@emollick) · 10-22 08:22

> A visible sign of what AI insiders have been warning about since at least the Mythos release. Acceleration of attack and defense, at inhuman speeds, interacting with the very human systems that need to react to them. https://t.co/jEI8WDjslo


♥ 1.9k · ↻ 180 · 💬 134 · [查看原帖](https://x.com/emollick/status/2113063313810792916)

---

### 中文创作者

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-23 04:13

> 旧金山聚变公司 Marathon Fusion 称用中子把水银变成了金子，金价不会受影响，他们真正要卖的是抗癌药原料
> 
> Marathon Fusion 是旧金山一家 28 人的创业公司。10 月 21 日，公司在 X 上发帖说，上个月他们用核聚变产生的中子，把水银（汞）变成了稳定的金子，速度是欧洲核子研究中心 CERN 2025 年纪录的 https://t.co/d7KYF6kugx


♥ 52 · ↻ 6 · 💬 9 · [查看原帖](https://x.com/dotey/status/2113363249194222032)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-23 02:02

> 我只希望 Claude Code 能支持读取 .agents/skills，别自己搞一套 .claude/skills https://t.co/rhiThAEz3y


♥ 19 · ↻ 0 · 💬 14 · [查看原帖](https://x.com/dotey/status/2113330196401303844)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-23 01:42

> 其实生成素材也可以交个Opus 5.5操作，能替代一整个AI生成+剪辑工作台
> 提示词见图片（可以说没有任何技巧） https://t.co/uK2ADFVWq1 https://t.co/kLUcahr4r6

![配图](https://pbs.twimg.com/amplify_video_thumb/2113324944960729088/img/0yaVAMC1UHVHN7Ts.jpg)
![配图](https://pbs.twimg.com/media/HVQJ9SMaQAAcBrv.jpg)

♥ 14 · ↻ 1 · 💬 1 · [查看原帖](https://x.com/Gorden_Sun/status/2113325149978337318)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-23 00:52

> 卡普空确认遭受针对其 CAPCOM ID 账户系统的网络攻击，影响全球 11,774,247 个账户。 https://t.co/lQ4q6gmvyw


♥ 10 · ↻ 0 · 💬 3 · [查看原帖](https://x.com/dotey/status/2113312593821794320)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-23 00:39

> Arc浏览器要停止使用了，曾经多么惊艳的浏览器。用户后续可以迁移到Dia上。
> 
> 这些浏览器我都试用过，但最终还是Chrome最好用，尤其是内置问问Gemini，是最符合日常使用的AI功能了（总结、写作等）。另外，现在的FireFox也非常漂亮。 https://t.co/WYCS92mmwC


♥ 4 · ↻ 0 · 💬 3 · [查看原帖](https://x.com/Gorden_Sun/status/2113309374999671131)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-23 00:33

> Ideogram发布能生成矢量图片的模型
> 矢量图片可以编辑、可以任意放大，也能由Agent通过代码编辑，尤其适合网页设计和海报等场景。模型同时支持图片转SVG。
> 
> 目前能生成矢量图片的模型有：Ideogram、Recraft、Arrow https://t.co/xZww4uet4G


♥ 3 · ↻ 0 · 💬 1 · [查看原帖](https://x.com/Gorden_Sun/status/2113307805767876779)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-23 00:01

> 我猜测 Tibo 搞这个 28 天不更新就重置活动，就是因为额度变少，需要每 3 天左右重置一次来维持以前一周的用量，否则你就会很快发现 Pro 订阅额度怎么这么少。
> 
> 可能他们正在加班加点解决模型不耐用问题，靠这 28 天续命呢。
> 
> https://t.co/ru39tAfGdJ https://t.co/mouRAuU1UD

![配图](https://pbs.twimg.com/amplify_video_thumb/2110557935726133248/img/lVj2zwqs1hUFwpFu.jpg)

♥ 109 · ↻ 3 · 💬 42 · [查看原帖](https://x.com/dotey/status/2113299677785542772)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 23:49

> 我一般是这样的：
> 我要外出没空搭理你，有问题你找 advisor 确认。
> 
> 当然前提是设置了 /advisor fable https://t.co/Y1v3ihYdB8


♥ 66 · ↻ 3 · 💬 8 · [查看原帖](https://x.com/dotey/status/2113296749737476142)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 23:27

> 吓我一跳，还以为 1Password 也出问题了，原来是要把密码共享给 Agent。有些网站我可以，但是主要的几个账号我还是不太放心的。 https://t.co/VZ5z34F6yZ


♥ 22 · ↻ 0 · 💬 18 · [查看原帖](https://x.com/dotey/status/2113291134265115101)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 18:54

> PHP RCE漏洞是什么？大肥鱼来介绍一下 https://t.co/jhLpYcpQxn

![配图](https://pbs.twimg.com/amplify_video_thumb/2113222014593081344/img/yWO89YQh1V8oLr2M.jpg)

♥ 79 · ↻ 8 · 💬 4 · [查看原帖](https://x.com/Gorden_Sun/status/2113222561849119064)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 18:05

> RecursiveSI开源flint模型
> 40B总参数，2.5B激活参数，针对编程任务设计，262K上下文，评分比Qwen3.6 35BA3B高。
> 
> 模型：https://t.co/tWcO0M1MRS https://t.co/zrvCjviPai https://t.co/VoZposgzsS

![配图](https://pbs.twimg.com/media/HVOhX2GakAEIoKp.jpg)

♥ 6 · ↻ 0 · 💬 10 · [查看原帖](https://x.com/Gorden_Sun/status/2113210097442984185)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 17:58

> 大肥鱼来介绍一下AI求职助手 https://t.co/c0SyDeZxqE

![配图](https://pbs.twimg.com/amplify_video_thumb/2113207765988687872/img/XK0z-Iu2mPMIlFlQ.jpg)

♥ 50 · ↻ 0 · 💬 6 · [查看原帖](https://x.com/Gorden_Sun/status/2113208446996881809)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-22 16:57

> 影视飓风都出海了。不过凭影视飓风这个视频质量，确实是吊打一众海外做数码测评的。
> 
> 但我觉着他们现在的视频没啥意思，看完以后只记得那些花里胡哨的转场和一些非常漂亮的样片
> 
> 就是把测评做的不像测评了，反倒是昨天看何同学的感觉不错 https://t.co/4X9oPqtJlK


♥ 33 · ↻ 0 · 💬 33 · [查看原帖](https://x.com/op7418/status/2113193055922921619)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-22 16:33

> Claude 里面还有一个存着的重置呢，没用的话大家可以用一下 https://t.co/4ukCnrVsSh


♥ 6 · ↻ 0 · 💬 9 · [查看原帖](https://x.com/op7418/status/2113186912076980242)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 15:04

> 又要重置了，还有10个小时？ https://t.co/3rRNpGkEYO


♥ 39 · ↻ 1 · 💬 52 · [查看原帖](https://x.com/dotey/status/2113164619078341049)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 13:31

> Underdog Bark 3.0：仅163 MB的语音转文字模型
> 
> 基于英伟达与 Moondream 开源的语音识别架构，模型体积被压缩到了 163 MB，转写速度极快，在苹果 M 系列芯片上转写 5 分钟音频仅需半秒。它不仅在英文会议场景下的错误率明显低于传统的 Whisper 等大模型，其特有的 Clean https://t.co/QLhELwXgHE

![配图](https://pbs.twimg.com/media/HVNim91aAAAjQGm.jpg)

♥ 22 · ↻ 0 · 💬 23 · [查看原帖](https://x.com/Gorden_Sun/status/2113141081026224479)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-22 13:03

> 这哥们儿做的宝可梦版本《吸血鬼幸存者》游戏是真的火
> 
>  叫 PokeBonk，我去，玩家非常多，各种自传播，国内也特别火。
> 
> 玩法就是你扮演其中一个宝可梦，在一个类似吸血鬼幸存者的地图里升级、自动打怪，宝可梦本身也能升级，打完 Boss 之后进下一个地图。 https://t.co/18AAOTWymd https://t.co/DPZE9fQohA

![配图](https://pbs.twimg.com/amplify_video_thumb/2113133807117430784/img/CdO8R6pTA-nag97W.jpg)

♥ 242 · ↻ 27 · 💬 36 · [查看原帖](https://x.com/op7418/status/2113134055680262324)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 12:26

> 紫微斗数：基于倪海厦《天纪》体系的紫微斗数开源排盘引擎与解读数据集。
> 
> 市面上传统的紫微斗数排盘算法多被商业软件封闭，普通人和研究者很难拿到透明可用的排盘规则与结构化解读数据。
> 
> 作者团队基于 Next.js、TypeScript、iztro 和 lunar-javascript https://t.co/Fm5sR8AWDp

![配图](https://pbs.twimg.com/media/HVNT4iBbkAAUkZa.jpg)

♥ 16 · ↻ 1 · 💬 5 · [查看原帖](https://x.com/Gorden_Sun/status/2113124936911065172)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 12:24

> DeepSeek 新一轮融资约 1000 亿元（约 150 亿美元），宁德时代和腾讯出钱最多，公司还没官方确认
> 
> 彭博社 10 月 21 日独家报道，DeepSeek 在最新一轮融资中筹到约 1000 亿元人民币，约合 150 https://t.co/qmj6gVx2Do


♥ 86 · ↻ 7 · 💬 85 · [查看原帖](https://x.com/dotey/status/2113124395321360646)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 12:09

> 为啥最近安全漏洞多
> 
> https://t.co/BucD9zkPjr https://t.co/dJcXasIRBw

![配图](https://pbs.twimg.com/amplify_video_thumb/2086627360548274177/img/A2dv52-gR2nKVfos.jpg)

♥ 84 · ↻ 3 · 💬 23 · [查看原帖](https://x.com/dotey/status/2113120595651297771)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 12:09

> 为啥最近安全漏洞多
> 
> https://t.co/zuygGhVP4q


♥ 0 · ↻ 0 · 💬 0 · [查看原帖](https://x.com/dotey/status/2113120523609604135)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 12:07

> Anthropic发布了一份年度公益报告，其中有一项是封号成果，封号上千万，维护了社会稳定。 https://t.co/sT49f78AMV


♥ 19 · ↻ 0 · 💬 7 · [查看原帖](https://x.com/Gorden_Sun/status/2113120088794841132)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 11:48

> Raon-1-mini-preview：韩国游戏公司魁匠团开源的MoE模型
> 
> 29B总参数，4.3B激活参数，整体评分比Qwen3.6 35BA3B高，对韩语和英语的支持比较好。
> 
> 模型：https://t.co/Buf8IVhioP https://t.co/O3ya97x0oN

![配图](https://pbs.twimg.com/media/HVNLEODaAAAiZDf.jpg)

♥ 7 · ↻ 0 · 💬 1 · [查看原帖](https://x.com/Gorden_Sun/status/2113115220310913198)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 11:43

> 英伟达开源检索系列模型
> 
> 包含负责看懂图文文档的Nemotron 3.5 Parse、负责在海量图文中精准搜索的Nemotron 3.5 Embed，以及负责对候选结果精细打分排序的Nemotron 3.5 Rerank。


♥ 31 · ↻ 6 · 💬 12 · [查看原帖](https://x.com/Gorden_Sun/status/2113114045591285817)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 11:34

> > TTS 读多音字、生僻字时经常读错，人工试听不可靠也不可规模化。这个方法把 TTS 音频交给 Kaldi 做语音识别，不看它识别出的汉字，而是读它解码路径上的音素（phoneme）序列，再与目标字的正确读音逐项比对，判定 TTS 到底读了什么音。 https://t.co/6i4evJN29Y


♥ 63 · ↻ 7 · 💬 43 · [查看原帖](https://x.com/dotey/status/2113111603650474251)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 10:55

> 马斯克的新订阅方案真他妈乱啊，我什么操作都没做，Cursor订阅和X订阅就自动合并到一起了，直接两边聊天记录都合并到一起，Grok Bot跑到了X的聊天里，给我看蒙了都。


♥ 15 · ↻ 0 · 💬 16 · [查看原帖](https://x.com/Gorden_Sun/status/2113101911138422916)

---

![头像](https://pbs.twimg.com/profile_images/1636981205504786434/xDl77JIw_normal.jpg) **歸藏(guizang.ai)** (@op7418) · 10-22 10:54

> 笑死！整了个大活儿！
> 
> 我把 Codex 连接到我电视上了，直接就可以跟它聊天 https://t.co/su52ko0Ihv https://t.co/XJs0Up1uy4

![配图](https://pbs.twimg.com/amplify_video_thumb/2113101522792009729/img/sOzR4BiKQOf9gN6S.jpg)

♥ 121 · ↻ 8 · 💬 66 · [查看原帖](https://x.com/op7418/status/2113101644334551095)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 10:04

> 晚点新闻 @latepostnews 你们的 X 账号被黑了 https://t.co/6n03bOxtYV

![配图](https://pbs.twimg.com/media/HVMzQEvXoAABx2A.jpg)

♥ 37 · ↻ 2 · 💬 20 · [查看原帖](https://x.com/dotey/status/2113089068225446022)

---

![头像](https://pbs.twimg.com/profile_images/1522159828231409664/GPpXyPT1_normal.jpg) **Gorden Sun** (@Gorden_Sun) · 10-22 09:48

> 这两天是有多少漏洞啊？
> PHP RCE
> Node.js
> GitLab
> LiteLLM
> eMudhra CA
> Railway


♥ 19 · ↻ 0 · 💬 14 · [查看原帖](https://x.com/Gorden_Sun/status/2113085000254165124)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 08:47

> 现在 AI 制作语音书效果还可以，但我觉得还不如专业的真人朗读的，另外还会有多音字错误，反而误导小朋友。所以有高质量真人的语音书还是选择真人的。
> 
> 如果真要自己用 AI 做语音书的话，最好先用大语言模型过一遍发音，让 Agent 去操作 TTS，多音字都标注上拼音、停顿位置、情感，然后再去生成会好很多。
> 
> 另外付费的比开源的普遍要好一些，但我没办法推荐哪家性价比高，我自己用 Gemini TTS 也不是因为它最好，只是用的顺手。


♥ 28 · ↻ 1 · 💬 33 · [查看原帖](https://x.com/dotey/status/2113069735260688703)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 08:40

> 再补充一个 Claude Code 任务卡片的细节，有些任务可以让它去云端执行，前提是你的项目是提交到 GitHub，然后通过 GitHub 的 connector 已经连接上了。
> 
> 走云端的好处是多任务并行起来会更容易，不过不如本地环境上工具丰富。 https://t.co/9YP9EycvH0 https://t.co/6OUyNjcG0F

![配图](https://pbs.twimg.com/media/HVL3k8FXcAAvFt5.jpg)

♥ 27 · ↻ 1 · 💬 41 · [查看原帖](https://x.com/dotey/status/2113067847429632059)

---

![头像](https://pbs.twimg.com/profile_images/561086911561736192/6_g58vEs_normal.jpeg) **宝玉** (@dotey) · 10-22 08:38

> 用 Node.js 的要升级了：三条版本线都有高危漏洞，最严重的可远程执行代码，eMudhra 那 8 枚坏证书也一并拉黑
> 
> 用 Node.js 跑服务、写工具的开发者，这周要换版本了。10 月 21 日，Node.js 给还在维护的三条版本线发了安全更新：22.x 升到 v22.23.4，24.x 升到 v24.22.1，26.x 升到 v26.12.1。三条线都修了高危漏洞，最严重的一个，官方说可能被用来远程执行代码。
> 
> 20.x 在 2026 年 4 月 30 日停止维护，25.x 在 6 月 1 日停止维护，这次都没有补丁。Node.js 在公告里提醒，每次发安全更新，停止维护的版本都会受影响，还在用的只能换到 22、24 或 26。
> 
> 【最需要注意的几个】
> 
> Node.js 自带一个解压 Brotli 格式的组件。Brotli 是网页传输常用的压缩格式，HTTP 里写作 br。这个组件有越界写入的问题，也就是把数据写到了不该写的内存位置，官方说这能导致远程执行代码。公告对它只有这一句描述，没说什么情况下会触发。修法是同步了 Google Brotli 项目的一处改动，让解压程序更早发现并拒绝格式不对的数据。
> 
> 另外三个漏洞出在 HTTPS 的证书核对上，两个高危、一个中危。Node 连 HTTPS 地址时，会核对证书上写的地址和你要连的地址是否一致，对不上就拒绝连接。这三个问题都和 IP 地址有关：IP 用全角数字写（输入法全角状态下打出的“１２７”这种），或者写法不规范、但能被宽松地认成 IP，核对就可能被绕过。修复后，Node 直接拒绝写法不规范的 IP 地址。全角数字那个只影响 24.x 和 26.x。
> 
> 还有一个高危出在 dns.resolve（查域名对应地址的函数）：域名中间如果夹着一个空字符（NUL），Node 会在那里把名字截断，实际查的只是前半截。
> 
> 中危里，用启动快照或者把程序打包成单个可执行文件（SEA）的要留意：crypto.randomUUID() 和 randomInt() 的随机数缓存会被一起存进包里，每次启动都生成同样的“随机”值。另有三个低危，涉及 26.x 读取 ZIP 文件，以及实验性的权限模型（--permission 开关）。
> 
> 这次还更新了 c-ares、OpenSSL、SQLite、undici 等内置组件，修的是这些组件已经公开的漏洞。
> 
> 【eMudhra 坏证书，Node 也拉黑了】
> 
> 三个新版本都加了一份内置黑名单，第一批放进去的就是 eMudhra 那 8 枚出问题的中间证书。
> 
> 这件事前几天刚曝出：印度发证机构 eMudhra 有 8 枚被各家系统认可的“网站公章”，盖章用的密码小到一秒就能算出来，谁拿到都能给任意网站做假证书。10 月 17 日被发现后，Chrome 和 Firefox 当天拉黑，eMudhra 18 日作废，Apple 19 日、Microsoft 20 日跟进，Node.js 21 日发版。
> 
> 当时 Cloudflare 提醒，浏览器之外的程序要一路更新到编程语言这一层，Node.js 就在这一层。Node 内置了 Mozilla 的可信发证机构名单，却没有浏览器那种随时拉黑坏证书的机制，所以用这 8 枚章签出的假证书，旧版 Node 照样放行。这份黑名单对 Node 建立的所有加密连接都生效。修复的提交说明里写道，它和 Go 语言、Electron 拉黑的是同一批。
> 
> 想测自己的程序还认不认这几枚章，可以用 Mozilla 工程师 Dennis Jackson 做的自查网站：https://t.co/iJDiH3dZ4O
> 
> 原文：https://t.co/0Ib8AIHPaX


♥ 256 · ↻ 48 · 💬 57 · [查看原帖](https://x.com/dotey/status/2113067412979433847)

---

### 视频图像与音乐

![头像](https://pbs.twimg.com/profile_images/1917978610683514880/JbHhI1yH_normal.jpg) **Suno** (@suno) · 10-23 05:10

> you’ve been using Suno. but have you used it like this? 🧵 https://t.co/5LLfQsrBwh

![配图](https://pbs.twimg.com/media/HVQ4k0NXMAAOQEy.jpg)

♥ 32 · ↻ 3 · 💬 11 · [查看原帖](https://x.com/suno/status/2113377372250788317)

---

![头像](https://pbs.twimg.com/profile_images/1917978610683514880/JbHhI1yH_normal.jpg) **Suno** (@suno) · 10-23 03:15

> Share a song you made this month 👇


♥ 209 · ↻ 28 · 💬 439 · [查看原帖](https://x.com/suno/status/2113348648629043464)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 16:31

> Things are getting surreal 👀 #Kling4 #KlingAI https://t.co/pXpVCEKj6Q


♥ 31 · ↻ 1 · 💬 6 · [查看原帖](https://x.com/Kling_ai/status/2113186439693586485)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 15:21

> One sweet prompt. 💜 #Kling4 https://t.co/P6yYLvl6P5


♥ 31 · ↻ 2 · 💬 6 · [查看原帖](https://x.com/Kling_ai/status/2113168909155315883)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 14:48

> Bring the drama! #Kling4 #KlingAI https://t.co/REyHSK1D7z


♥ 28 · ↻ 3 · 💬 2 · [查看原帖](https://x.com/Kling_ai/status/2113160491837313135)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 14:32

> Hold on to your hat. #KlingAI #Kling4 https://t.co/xkO3lwBZCo


♥ 21 · ↻ 3 · 💬 5 · [查看原帖](https://x.com/Kling_ai/status/2113156632134005040)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 14:06

> #Kling4 is now on OiiOii 🐈‍⬛ #KlingAI https://t.co/MfdTSqf4X1


♥ 25 · ↻ 1 · 💬 2 · [查看原帖](https://x.com/Kling_ai/status/2113150103750135859)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 13:36

> Kling 4.0 is now live on OnSolo. #Kling4 #KlingAI https://t.co/WUnjxWjEZT


♥ 16 · ↻ 0 · 💬 2 · [查看原帖](https://x.com/Kling_ai/status/2113142473145078041)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 13:07

> Meet your next creative spark: Kling 4.0, now in Firefly. #Kling4 #KlingAI https://t.co/AYlIxkV9MX


♥ 33 · ↻ 4 · 💬 6 · [查看原帖](https://x.com/Kling_ai/status/2113135088091476358)

---

![头像](https://pbs.twimg.com/profile_images/1905183334021697536/8agjzVoq_normal.jpg) **Kling AI** (@Kling_ai) · 10-22 09:00

> At LA Tech Week 2026, Kling joined Oxen AI and Obsidian Studio to explore how AI video is finding its place in enterprise content production, from shot creation to final delivery.
> 
> Watch the highlights to see how Kling 4.0 supports complex production needs. https://t.co/c95bA5k2uY

![配图](https://pbs.twimg.com/media/HVJ-cisWAAAs4Dw.jpg)

♥ 30 · ↻ 6 · 💬 12 · [查看原帖](https://x.com/Kling_ai/status/2113072850802196961)

---
