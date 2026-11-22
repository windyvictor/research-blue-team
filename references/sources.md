# 方法来源及使用边界

以下按公开可核查的来源列出。科研用法均为针对研究工作的改编，不代表原文献主张。具体投稿要求以目标会刊当年指南为准。

## 一、蓝军定位与质疑姿态

- 快刀青衣《复盘跨年演讲中“AI蓝军”的由来，分享AI落地实战中的四条感悟》，得到 App「快刀广播站」（[同名转载](https://www.53ai.com/news/neirongchuangzuo/2025011019563.html)）。原文明确“蓝军不是敌军，更不是叛军，大家的目标是一致的”，只在战略层和主营业务掰腕子。科研蓝军据此与作者共同解决同一科学问题，质疑路线而不改变研究目标。
- 快刀青衣谈“助理教练”（[同名文章](https://www.53ai.com/news/neirongchuangzuo/2025060691523.html)）：会前预演、让对手挑错，同时给作者留下重写与反思的空间。科研陪练据此让作者先回答一条实质异议，再依回应追问或撤回。
- Gary Klein, "Performing a Project Premortem", HBR, 2007-09（[链接](https://hbr.org/2007/09/performing-a-project-premortem)）：先假定失败再倒推哪条依赖最可能中断。本 skill 只用于找值得验证的风险；原文是有明确结束的短时练习，不把设想写成已发生的失败。
- Daniel Dennett, *Intuition Pumps and Other Tools for Thinking* (2013), Rapoport 规则：重构到对方认可、列出共识、说明学到什么，之后才允许批评。同书指出，搜寻隐藏矛盾常越过界变成 nitpicking 与 sea-lawyering，这类容易打的目标与真正争点无关，只浪费所有人的时间和耐心。本 skill 据此把“替作者作最强回应”放在提出异议之后，并设刹车条件。

## 二、批评强度校准的依据

- Jiang, Li, Wang, Fan, Zeng, "Demanding peer review is associated with higher impact in published science", [arXiv:2604.14047](https://arxiv.org/abs/2604.14047) (2026)；Nature 报道 [d41586-026-01615-4](https://www.nature.com/articles/d41586-026-01615-4)。用 LLM 把 Nature Communications 2017—2024 年 8000 篇已接收论文的评审往来转成结构化指标：最强质疑集中在核心主张与新颖性而非写作格式，且集中在第一轮；与三年内引用正相关最强的是修订成本，其次是观点强度与评论质量，意见是否礼貌／建设性几乎无相关。**这是观察性研究，样本只含已接收论文，因果方向未定。** 本 skill 据此不降低质疑强度，而把强度落在核心主张上、砍掉枝节。
- Zheng et al., "Judging LLM-as-a-Judge with MT-Bench and Chatbot Arena", NeurIPS 2023, [arXiv:2306.05685](https://arxiv.org/abs/2306.05685)：点名 position、verbosity、self-enhancement 三类偏差，并明确不把 LLM 裁判视为中性。本 skill 据此限定条数、要求证据定位、不因篇幅与语气改判。
- McAleese et al., "LLM Critics Help Catch LLM Bugs" (CriticGPT), OpenAI, 2024, [arXiv:2407.00215](https://arxiv.org/abs/2407.00215)；[官方说明](https://openai.com/index/finding-gpt4s-mistakes-with-gpt-4/)。论文把「nitpicks（无帮助的小抱怨）」与幻觉式 bug 列为批评模型的两类失效，用 test-time search 在「找问题的激进程度」与幻觉率之间做精度-召回权衡；人机协作比模型单独批评更全面、更少 nitpick。本 skill 的三态分级与停止条件据此设计。
- Huang et al., "Large Language Models Cannot Self-Correct Reasoning Yet", ICLR 2024, [arXiv:2310.01798](https://arxiv.org/abs/2310.01798)：无外部反馈的内在自纠不改善推理，有时把正确答案改错。本 skill 据此要求撤回与改写必须回到材料、图表或计算，不靠再想一遍。
- Michael J. Black, "Novelty in Science"（[原文](https://perceiving-systems.blog/en/news/novelty-in-science)）：审稿人常把复杂、难度、技术含量误当创新，把“简单”“显而易见”“A+B”当成创新性不足；作者提醒审稿人承认自身想象力的局限。

## 三、审稿规范

- [NeurIPS Paper Checklist](https://neurips.cc/public/guides/PaperChecklist)：让作者把主要主张与适用范围、假设、证明及实验细节对应起来。对经验论文，用它检查结论和证据是否匹配；具体投稿要求以目标会刊为准。
- [国家自然科学基金项目评审专家行为规范](https://www.nsfc.gov.cn/p1/2871/2874/2884/69612.html)：评审结合项目指南和材料，判断科学价值、创新性和方案可行性等。这里用于申请人自查和预演答辩，具体条款取自当年、当类指南。

## 四、使用边界

- 上述实证多来自 LLM 评审、代码批评与元科学研究，任务分布与数学、优化、机器学习论文不同。它们用于设计刹车机制，不作为“某类意见必然成立”的依据。
- 事前验尸与 Rapoport 规则属思维框架，效果依赖使用者；本 skill 只取其中可核对的判据与停止条件，不据此宣称某种批评姿态更有效。
- 评审强度与论文影响力的关联是相关性，且样本只含已接收论文；不能据此认为 stricter review 会提高任何一篇具体稿件的影响力。
- 网络核对只用公开论文题名、标准术语与已公开信息，不把未发表的定理表述、项目标题、评审意见、数据或可识别片段作为查询内容。
