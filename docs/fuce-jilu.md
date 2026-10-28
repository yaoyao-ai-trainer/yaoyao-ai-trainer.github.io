# 全部复测记录（按日期倒序）：官方价格、官方政策、作者商城价格每次核对了什么、结果如何

> 本页是《国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集》的一章（[合集首页](../README.md)）。把各原仓库文末的复测记录汇总到一页，去掉重复行；每一行的出处链接到原仓库。只记真实做过的核对；官方出新模型、改价格、改政策，或作者商城改价时补一行。

共 38 条（统计到 2026-10-28）。

| 日期 | 核对了什么 | 结果 | 出处（原仓库） |
|---|---|---|---|
| 2026-10-28 | **价格：** 按作者商城事实卡 yy-facts.json（每 15 分钟从商城数据库生成）核对全部商品 | 与本页"快速购买"和价格表一致，无变动；开通时间统一写"平均 2 分钟" | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-28 | **商城调价：** ChatGPT Plus 三个月 ¥381 → ¥387、六个月 ¥750 → ¥774、十二个月 ¥1488 → ¥1548，统一按一个月 ¥129 × 月数计价 | 快速购买、价格表已同步；其余商品价格不变 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-28 | **商城调价：** ChatGPT Plus 十二个月改为 ¥1488，并入一个月的下单页（item/5 选「1 年」，旧 item/7 链接自动跳转）；三个月 ¥381、六个月 ¥750 | 快速购买、价格表已同步；其余商品价格不变 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-28 | **价格：** 按作者商城事实卡 yy-facts.json（每 15 分钟从商城数据库生成）核对全部商品 | 与本页"快速购买"一致，无变动；开通时间统一写"平均 2 分钟" | [OpenAI Codex CLI 国内使用指南](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#复测记录) |
| 2026-10-28 | **下单页：** curl 作者商城 item/10 和 item/10?d=premium | 价格仍是 Plus ¥70 / Premium ¥239 / Super ¥749 / Ultra ¥1499；直接打开 item/10 默认选中 Plus（不再是 Premium），?d=premium 会预选 Premium；快速购买链接改为 ?d=premium，本页说明已同步 | [Grok Premium（原 SuperGrok）国内怎么买](https://github.com/haiwaihuyonghui-rgb/grok-premium#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/10（含 ?d=plus / super / ultra）和 llms.txt | Grok 改为四档：Plus ¥70、Premium ¥239（原 ¥159）、Super ¥749、Ultra ¥1499，同一个下单页选档位；商品页开通条件改为"账号不是会员（免费版）就能充"，不再要求半价优惠；本页价格表已同步 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-27 | **商城调价：** ChatGPT Plus 十二个月 ¥1548 → ¥1439 | 快速购买、价格表已同步；其余商品价格不变 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus 一个月 ¥129、十二个月 ¥1548，其余商品见价格表），十个商品均无变动 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页价格表一致（Plus 一个月 ¥129、十二个月 ¥1548、Pro 100 美金档位 ¥699 等），无变动 | [没有信用卡怎么开通 ChatGPT Plus](https://github.com/haiwaihuyonghui-rgb/chatgpt-plus-wu-xinyongka#复测记录) |
| 2026-10-27 | **官方规则：** 浏览器打开 What is ChatGPT Plus、ChatGPT 定价页付款 FAQ（中文版）、OpenAI 礼品卡文章 | Plus 20 美元/月、只能月付；付款写"任何主要信用卡"；礼品卡只限美国、15～250 美元、只能网页兑换、不能用于 App 内购 | [没有信用卡怎么开通 ChatGPT Plus](https://github.com/haiwaihuyonghui-rgb/chatgpt-plus-wu-xinyongka#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页价格表一致（Pro 100 美金档位 ¥699、200 美金档位 ¥1399、500 美金档位 ¥3499、Plus ¥129），无变动 | [ChatGPT Pro 100 美金档位国内怎么买](https://github.com/haiwaihuyonghui-rgb/chatgpt-pro-100#复测记录) |
| 2026-10-27 | **官方价格与规则：** 浏览器打开 About ChatGPT Pro tiers、What is ChatGPT Plus | Pro 100 / 200 / 500 美元、只能月付；只有 Pro 500 含 Ultrafast；Fast 2.5 倍、Ultrafast 8 倍消耗额度；Pro 200 老用户旧额度保留到 10-29；Plus 20 美元/月、只能月付 | [ChatGPT Pro 100 美金档位国内怎么买](https://github.com/haiwaihuyonghui-rgb/chatgpt-pro-100#复测记录) |
| 2026-10-27 | **官方政策：** ChatGPT 定价页付款 FAQ、OpenAI 礼品卡文章 | 付款写"任何主要信用卡"；礼品卡只限美国、只能网页兑换、不能用于 App 内购 | [ChatGPT Pro 100 美金档位国内怎么买](https://github.com/haiwaihuyonghui-rgb/chatgpt-pro-100#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页价格表一致（Plus ¥129、Pro 100 美金档位 ¥699、Claude Pro ¥159、Grok ¥159、Gemini 18 个月 ¥99 等），无变动 | [ChatGPT / Claude / Gemini / Grok 会员价格对比](https://github.com/haiwaihuyonghui-rgb/chatgpt-jiage-duibi#复测记录) |
| 2026-10-27 | **官方价格：** 浏览器打开 OpenAI Plus、Pro 三档帮助文章；curl Claude 定价页；浏览器打开 gemini.google/subscriptions（地区切到 United States）和 x.ai/pricing | ChatGPT Plus 20、Pro 100 / 200 / 500；Claude Pro 20（年付 200）、Max 100 / 200；Google AI Plus 4.99、Pro 19.99、Ultra 99.99 / 199.99；xAI 8 / 30 / 100 / 200 美元。ChatGPT 定价页用中国大陆网络打开不显示价格，Go 沿用 10-17 核对结果 | [ChatGPT / Claude / Gemini / Grok 会员价格对比](https://github.com/haiwaihuyonghui-rgb/chatgpt-jiage-duibi#复测记录) |
| 2026-10-27 | **官方政策：** ChatGPT 定价页付款 FAQ、OpenAI 礼品卡文章、x.ai/pricing FAQ、Gemini 网页版地区列表 | ChatGPT 付款写"任何主要信用卡"；礼品卡只限美国、只能网页兑换；xAI 不授权第三方卖家；Gemini 网页版列表含香港、澳门、台湾，中国大陆只写 Workspace only | [ChatGPT / Claude / Gemini / Grok 会员价格对比](https://github.com/haiwaihuyonghui-rgb/chatgpt-jiage-duibi#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus ¥129、Claude Pro ¥159、Max 5X ¥900、Max 20X ¥1800），十个商品均无变动 | [Claude Pro / Max 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/claude-daichong#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus ¥129、Claude Pro ¥159、Max 5X ¥900），十个商品均无变动 | [Claude 充值平台怎么选](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus ¥129、Pro 200 美金档位 ¥1399），十个商品均无变动 | [OpenAI Codex CLI 国内使用指南](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus ¥129、Grok Premium ¥159（商品页仍写只限免费版 + 半价 50%）），十个商品均无变动 | [Grok Premium（原 SuperGrok）国内怎么买](https://github.com/haiwaihuyonghui-rgb/grok-premium#复测记录) |
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus ¥129、Claude Pro ¥159、Grok ¥159、Gemini 18 个月 ¥99），十个商品均无变动 | [AI 会员订阅国内指南](https://github.com/haiwaihuyonghui-rgb/ai-subscription-guide-cn#复测记录) |
| 2026-10-26 | **价格：** 逐个 curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19，和 llms.txt 对照 | 与本页价格表一致（Plus 一个月 ¥129 … Gemini 18 个月 ¥99），无变动 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-26 | **官方价格：** 打开 OpenAI 帮助中心 Plus、Pro 三档文章 | Plus 20 美元/月、只能月付；Pro 100 / 200 / 500 美元三档，只有 Pro 500 含 Ultrafast；Pro 200 老用户旧额度保留到 10-29。用中国大陆网络打开定价页不显示价格，Go 的 8 美元沿用 10-17 核对结果 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-26 | **官方政策：** 定价页付款 FAQ、礼品卡文章、重复扣费文章、支持地区列表 | 官网付款写"任何主要信用卡"；官方礼品卡只限美国、不能用于 App 内购；App 内订阅由苹果 / 谷歌管理；大陆、香港、澳门不在支持列表，台湾在 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-26 | **开通流程：** 对照作者商城 llms.txt 和售后页 | Plus 一个月卡密自助开通、其他商品订单页填信息人工开通；售后三条与售后页一致 | [ChatGPT Plus 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#复测记录) |
| 2026-10-26 | **价格：** curl 作者商城商品页 item/12、14、13 和 llms.txt | Claude Pro ¥159、Max 5X ¥900、Max 20X ¥1800，无变动 | [Claude Pro / Max 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/claude-daichong#复测记录) |
| 2026-10-26 | **官方价格：** Claude 定价页、帮助中心 What is the Max plan | Pro 月付 20 美元 / 年付折合 17 美元；Max 5x 100、20x 200 美元；新看到：Max 含每月 100～200 美元 API 额度；手机端价格可能不同 | [Claude Pro / Max 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/claude-daichong#复测记录) |
| 2026-10-26 | **官方政策：** 赠送订阅文章、账单 FAQ、支持地区列表 | 赠送订阅暂停购买；App 内订阅由苹果 / 谷歌管理；大陆、香港、澳门不在列表，台湾在 | [Claude Pro / Max 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/claude-daichong#复测记录) |
| 2026-10-26 | **开通流程：** 对照商城售后页和 llms.txt | 订单页只填组织 ID、人工开通；售后三条与售后页一致 | [Claude Pro / Max 国内怎么开通](https://github.com/haiwaihuyonghui-rgb/claude-daichong#复测记录) |
| 2026-10-26 | **官方价格：** Claude 定价页、帮助中心 What is the Max plan | Pro 月付 20 美元 / 年付折合 17 美元（一次 200 美元）；Max 5x 100、Max 20x 200 美元；Max 含每月 API 额度；官方注明手机端价格可能不同——与本页价格表一致 | [Claude 充值平台怎么选](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#复测记录) |
| 2026-10-26 | **官方政策：** Anthropic 支持地区列表、账单 FAQ、赠送订阅文章 | 大陆、香港、澳门不在支持列表，台湾在；App 内订阅由苹果 / 谷歌管理；赠送订阅暂停购买 | [Claude 充值平台怎么选](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#复测记录) |
| 2026-10-26 | **官方价格：** OpenAI 帮助中心 What is ChatGPT Plus、About ChatGPT Pro tiers | Plus 20 美元/月、只能月付；Pro 100 / 200 / 500 美元三档，只有 Pro 500 含 Ultrafast；Pro 200 老用户旧额度到 10-29——与本页一致 | [OpenAI Codex CLI 国内使用指南](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#复测记录) |
| 2026-10-26 | **官方政策：** 支持地区列表、定价页付款 FAQ | 大陆、香港、澳门不在支持列表，台湾在；官网付款写"任何主要信用卡" | [OpenAI Codex CLI 国内使用指南](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#复测记录) |
| 2026-10-26 | **价格：** curl 作者商城商品页 item/10 和 llms.txt | Grok Premium 一个月 ¥159，商品页仍写"只限免费版 + 半价 50%"，无变动 | [Grok Premium（原 SuperGrok）国内怎么买](https://github.com/haiwaihuyonghui-rgb/grok-premium#复测记录) |
| 2026-10-26 | **官方价格：** 打开 x.ai/pricing | Plus 8 / Premium 30 / Super 100 / Ultra 200 美元每月，不含税，和 10-22 核对一致 | [Grok Premium（原 SuperGrok）国内怎么买](https://github.com/haiwaihuyonghui-rgb/grok-premium#复测记录) |
| 2026-10-26 | 官方政策： x.ai/pricing FAQ | 自助订阅支持主流信用卡和借记卡；用量池 Grok 与 Cursor 共用、每周刷新；官方不授权任何第三方卖家，未授权来源的订阅可能被暂停或终止（本次新写入正文）；续费前 24 小时取消 | [Grok Premium（原 SuperGrok）国内怎么买](https://github.com/haiwaihuyonghui-rgb/grok-premium#复测记录) |
| 2026-10-26 | **开通流程：** 对照商城售后页和 llms.txt | 订单页填 sso 代码、人工开通；售后三条一致 | [Grok Premium（原 SuperGrok）国内怎么买](https://github.com/haiwaihuyonghui-rgb/grok-premium#复测记录) |
| 2026-10-26 | **xAI 官方价格与政策：** x.ai/pricing | 三合一四档 8 / 30 / 100 / 200 美元每月；原表"SuperGrok / SuperGrok Heavy 30 / 300 美元"已过时，本次更正；官方 FAQ 写明不授权任何经销商或第三方卖家 | [AI 会员订阅国内指南](https://github.com/haiwaihuyonghui-rgb/ai-subscription-guide-cn#复测记录) |

## 合集里的其他章节

谷歌站版攻略（同一作者整理，手机上看更方便；[全部 15 页入口](../README.md#谷歌站版攻略)）：

- [ChatGPT Plus 多少钱一个月：官方价、人民币真实成本和国内购买方式](https://sites.google.com/view/yaoyao-ai/plus-jiage)
- [国内代充 AI 会员常见问题：售后、退款、掉会员、封号、发票、客服时间](https://sites.google.com/view/yaoyao-ai/faq)

本文是 [国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集](https://github.com/yaoyao-ai-trainer/yaoyao-ai-trainer.github.io) 的一章，其他章节（每章是摘要，完整正文在各自的原仓库）：

- [ChatGPT Plus 国内怎么开通：官方订阅、应用内购、礼品卡、代充四种方法怎么选](chatgpt-plus.md)
- [没有信用卡怎么开通 ChatGPT Plus：支付宝 / 微信能不能付、礼品卡、应用内购、代充](chatgpt-plus-wu-xinyongka.md)
- [ChatGPT Pro 100 美金档位国内怎么买：Pro 100 / 200 / 500 三档区别、和 Plus 差在哪](chatgpt-pro-100.md)
- [ChatGPT / Claude / Gemini / Grok 会员价格对比：四家官方价、约合人民币、代充价怎么算账](jiage-duibi.md)
- [Claude Pro / Max 国内怎么开通：官方订阅、应用内购、赠送订阅、代充四种方法怎么选](claude-daichong.md)
- [Claude 充值平台怎么选：Pro / Max 怎么选、充值后显示 Free Plan 排查、防封习惯](claude-chongzhi.md)
- [Claude 代充靠谱吗：代充原理、要交出什么信息、风险在哪](claude-kaopu-yuanli.md)
- [Claude Code 国内使用指南：安装、登录、Pro / Max 额度怎么选、常见报错](claude-code.md)
- [OpenAI Codex CLI 国内使用指南：安装、ChatGPT 账号登录、多账号切换、Plus / Pro 额度、常见报错](codex-cli.md)
- [Grok Premium（原 SuperGrok）国内怎么买：官方四档价格、三合一说明、四种开通方法](grok-premium.md)
- [Grok 代充：什么账号能充、怎么开通、靠谱吗](grok-daichong.md)
- [Gemini Pro（Google AI Pro）国内代充：怎么开通、开通后怎么确认生效、常见问题](gemini-pro.md)
- [AI 会员订阅国内指南：ChatGPT / Claude / Gemini / Grok 开通路线对比、代充判断 8 条](ai-subscription.md)
- [常见问题详细版：能不能用、代充、档位](faq-xiangxi.md)
- [作者商城商品说明：全部商品价格、开通流程、售后](shangcheng.md)
- [报错速查表：ChatGPT / Claude / Claude Code / Codex 常见报错去哪看](baocuo-sucha.md)
- [全部复测记录（按日期）](fuce-jilu.md)
- [回到合集首页](../README.md)
