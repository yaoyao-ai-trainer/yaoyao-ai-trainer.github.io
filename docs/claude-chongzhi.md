# **📚 全部教程合集：[国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集 2026](https://github.com/yaoyao-ai-trainer/yaoyao-ai-trainer.github.io)**（本文已并入合集 [Claude 充值平台怎么选](https://github.com/yaoyao-ai-trainer/yaoyao-ai-trainer.github.io/blob/main/docs/claude-chongzhi.md)，16 章一个仓库，价格每周核对；网页版 [yaoyao-ai-trainer.github.io](https://yaoyao-ai-trainer.github.io/)）

> 本文是《国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集》的一章（[合集首页](../README.md) · [全部章节](../README.md#目录)）。原仓库 [claude-chongzhi](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi) 保留。 最后更新：2026-10-27 · 相关攻略加组织目录页链接（yaoyao-ai-trainer.github.io）

> **立场说明：** 整理：瑶瑶ai训练师。作者自己经营一家 AI 会员代充商城（kw.yaoyao.chat），所以本文不是第三方评测；代充只作为几种方法中的一种来写，作者商城的价格统一放在合集首页。与 OpenAI、Anthropic、Google、xAI 没有隶属关系，也没有授权，品牌名仅用于说明。

# Claude 充值平台怎么选？国内充值 Claude Pro / Max 指南（2026 年 10 月更新）

这是一份面向中文用户的 Claude 付费会员说明：Pro、Max 5x、Max 20x 的官方美元价和区别，国内为什么直接付不了款，充值平台（代充）怎么挑，以及"升级后还是显示 Free Plan"、额度用完、Claude Code 登录计费不对等问题的排查，报错部分按 Anthropic 官方帮助中心和 Claude Code 官方文档整理并附链接。作者：瑶瑶ai训练师；更新于 2026-10-17。本仓库是非官方整理，与 Anthropic 没有隶属关系，文中品牌名仅用于说明。

**直接回答：** Claude 官网只接受支持地区发行的信用卡 / 借记卡付款，国内银行卡、支付宝直接付不了。没有海外卡的人，常见做法是"代充"（订阅代付）：由卖家替你付款，把 Claude Pro 或 Max 订阅开到你自己的账号上。

**怎么选：** Pro 适合日常写作和偶尔写代码；每天用 Claude Code 写几个小时选 Max 5x；几乎全天在跑选 Max 20x。选充值平台看 6 点：价格正常、不要密码、开通方式说得清、失败怎么退、掉订阅管不管、售后找得到人。

**官方价格：** Pro $20/月（年付折合 $17/月）、Max 5x $100/月、Max 20x $200/月（2026-10-17 核对自 Anthropic 官方定价页和帮助中心，见下表）。

## 目录

- [使用前先读：关于地区](#使用前先读关于地区)
- [Claude 官方价格表（2026-10-17 核对）](#claude-官方价格表2026-10-17-核对)
- [Pro 和 Max 怎么选](#pro-和-max-怎么选)
- [为什么国内充值 Claude 很难](#为什么国内充值-claude-很难)
- [三种充值方式对比](#三种充值方式对比)
- [怎么选充值平台的 6 个判断点](#怎么选充值平台的-6-个判断点)
- [报错 / 常见问题大全](#报错--常见问题大全)
- [降低被封风险的习惯](#降低被封风险的习惯)
- [常见问题](#常见问题)
- [国内开通参考](#国内开通参考)
- [更多教程](#更多教程)
- [关于本仓库和作者](#关于本仓库和作者)
- [参考资料](#参考资料)
- [复测记录](#复测记录)
- [作者商城：代充方式中的一种（如实披露）](#作者商城代充方式中的一种如实披露)
- [合集里的其他章节](#合集里的其他章节)

## 使用前先读：关于地区

Anthropic（Claude 的公司）官方公布了支持的国家和地区列表（[anthropic.com/supported-countries](https://www.anthropic.com/supported-countries)），页面写明"未列出的国家和地区不受支持"。2026-10-17 查看：中国大陆、香港、澳门都不在列表中（台湾在列表中）。本仓库只整理官方的价格、订阅和报错说明，不提供绕过地区限制或支付限制的方法；请在符合 Anthropic 服务条款的前提下使用。

## Claude 官方价格表（2026-10-17 核对）

| 套餐 | 官方价（美元） | 用量和权益（官方说法） |
|---|---|---|
| Free | $0 | 用量少；不含 Claude Code |
| Pro | $20/月；年付一次交 $200，折合 $17/月 | 每 5 小时用量至少是 Free 的 5 倍；含 Claude Code；可开启用量额度（usage credits） |
| Max 5x | $100/月 | 每 5 小时用量是 Pro 的 5 倍；含 Claude Code；含每月 API credits（只能在 API 平台用） |
| Max 20x | $200/月 | 每 5 小时用量是 Pro 的 20 倍；其余同 Max 5x |
| Team | 标准席位 $20/人/月（年付）或 $25（月付）；高级席位 $100 / $125 | 2–150 人；含 Claude Code 和团队共享 API credits |
| Enterprise | 按席位加按 API 价计的用量，联系销售 | 大型组织 |

来源：[Anthropic 官方定价页](https://claude.com/pricing)（anthropic.com/pricing 会跳转到这里）、[What is the Pro plan?](https://support.claude.com/en/articles/8325606-what-is-the-pro-plan)、[What is the Max plan?](https://support.claude.com/en/articles/11049741-what-is-the-max-plan)。帮助中心注明这些是网页订阅价，手机 App 内订阅价格由应用商店决定，价格和套餐可能调整，以官方为准。

几点说明（都来自上面的官方页面）：

- 所有套餐的用量按滚动 5 小时窗口重置；付费套餐在此之外还有每周上限，官方也可能按容量加其他限制。网页、桌面端、手机 App 和 Claude Code 的使用都从同一份额度里扣。
- 会员和 API 分开计费：Pro 不含 API 额度；Max 附带的每月 API credits 只能在 API 平台（Console）用，不能用在 Claude 应用和 Claude Code 里。
- 额度用完后，Pro / Max 可以在 Settings → Usage 开启"用量额度（usage credits）"继续用，按标准 API 价计费，可以设每月上限；不开就等重置。
- 从 Pro 升 Max、Max 5x 升 20x，官方按剩余账期比例补差价，立即生效。

## Pro 和 Max 怎么选

- 首次开会员：先买 **Pro** 用一个月。
- Pro 一周里好几天提示额度用完，或者每天用 Claude Code 写几个小时代码：换 **Max 5x**。
- Max 5x 还是经常不够、几乎全天在用：换 **Max 20x**。
- 拿不准就先买低一档，用一周看看会不会经常碰到上限；同一个账号升级，聊天记录和项目都在。

额度用完时，Claude Code 里输入 `/usage` 可以看用量和重置时间。额度细节见 [Claude Pro 有多少额度](https://kw.yaoyao.chat/guide/claude-pro-edu.html)，Claude Code 的安装、登录和报错见技术教程仓库 [Claude Code 国内使用指南](claude-code.md)。

## 为什么国内充值 Claude 很难

- Anthropic 官方不面向中国大陆提供服务（见上面的地区说明）。
- 官网结算只接受信用卡或借记卡（官方账单 FAQ 原文：网页订阅只接受信用卡和借记卡），国内的银联卡、支付宝付不了，国内发行的双币卡也经常被拒（card declined）。
- 注册需要完成手机验证，且要求使用支持地区的号码，对使用地区的要求比 ChatGPT 更严格。

## 三种充值方式对比

| 方式 | 做法 | 优点 | 缺点 |
|---|---|---|---|
| 自己用海外卡订阅 | 在 claude.ai 设置里升级，绑海外卡 | 官方价，自己掌控 | 国内的卡基本付不了，被拒很常见 |
| 外区 Apple ID 应用内订阅 | 外区 Apple ID + 当地礼品卡，在 iPhone App 里订阅 | 不用信用卡 | 要外区账号、买礼品卡，步骤多，价格按当地商店；订阅由 App Store 管理 |
| 充值平台代充 | 卖家帮你付款，会员开在你自己的账号上 | 支付宝就能下单，省事 | 平台质量参差不齐，要会挑 |

## 怎么选充值平台的 6 个判断点

1. **价格是否正常。** 官方 Pro 是 $20/月，代充价是平台自己的定价，靠谱的代充一般比官方美元价折算后高一些（包含代付成本和售后）。价格低得离谱的要问清原因。
2. **要不要账号密码。** 不需要。要账号密码、要转发验证码的不要碰。
3. **开通方式和速度。** 问清是自助还是人工，晚上和节假日下单多久能处理。
4. **失败怎么退。** 付款前问清失败后钱怎么处理，让对方用文字回复。
5. **掉订阅管不管。** 问清有没有质保、覆盖多久、怎么补。
6. **售后找谁。** 有没有能联系到的真人，平台背后是谁，域名能不能在别处核实。

这 6 个问题对 ChatGPT 代充同样适用，逐项判断方法见 [GPT代充怎么选](https://kw.yaoyao.chat/guide/gpt-daichong.html?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=claude-chongzhi)。

## 报错 / 常见问题大全

这一节已整理进合集的 [报错速查表](baocuo-sucha.md#claude12-个报错)，按"现象 → 原因 → 怎么处理"写，附官方链接。

## 降低被封风险的习惯

- 网络保持稳定，一直用同一个地区，不要频繁切换国家。
- 一个账号只给自己用，不要多人共用。
- 不要短时间内反复注册、换邮箱。
- 重要的对话和代码自己另外备份。
- 被停用时先看邮箱里的通知，通过官方帮助中心申诉。能否恢复、是否退款以官方结果为准。

## 常见问题

**Q：Claude 会员能用 API 吗？**
A：不能。Pro 不包含 API 额度；会员和 API（console.anthropic.com，按用量付费）是两套分开计费的账户。Max 附带的每月 API credits 只能在 API 平台用。Claude Code 可以直接用会员账号登录，走会员额度。

**Q：Claude 会员能几个人共用吗？**
A：不建议。会互相抢额度，在不同地方同时登录更容易被风控。

**Q：代充会不会封号？**
A：代充开的是你自己账号上的正常订阅。账号被限制更多和使用习惯有关：频繁切换地区、多人共用、付款被撤销（低价单常见）。

**Q：国内用支付宝能买 Claude 会员吗？**
A：官网不能直接用支付宝。可以在充值平台用支付宝下单，由卖家开通到你自己的账号上。

**Q：Claude Code 要单独买吗？**
A：不用。Pro 和 Max 都包含 Claude Code，运行 `claude` 用订阅账号登录即可；免费版不含。见 [Claude Code 怎么收费](https://kw.yaoyao.chat/guide/claude-code.html)。

**Q：Pro 年付和月付怎么选？**
A：官方价年付 $200（折合 $17/月），月付 $20/月；年付一次付清、中途不退，确定长期用再选。代充一般按月。

**Q：Claude 和 ChatGPT 买哪个？**
A：两家入门价都是 $20/月。长文、写代码很多人偏 Claude；画图、搜索、语音偏 ChatGPT。见 [ChatGPT 和 Claude 买哪个](https://kw.yaoyao.chat/guide/chatgpt-vs-claude.html)。

## 国内开通参考

没有海外卡、想了解国内怎么开通 Claude Pro / Max 以及充值平台的流程和注意事项，看这一篇：[Claude 充值平台：国内怎么充值 Claude Pro / Max](https://kw.yaoyao.chat/guide/claude-daichong.html)。

## 更多教程

- [Claude 会员多少钱？Pro 和 Max 有什么区别](https://kw.yaoyao.chat/guide/claude-price.html)
- [Claude 充值了还是显示 Free Plan 怎么办](https://kw.yaoyao.chat/guide/claude-free-plan.html)
- [Claude Pro 有多少额度？5 小时和每周限制怎么算](https://kw.yaoyao.chat/guide/claude-pro-edu.html)
- [Claude Code 怎么收费？Pro 和 Max 怎么选](https://kw.yaoyao.chat/guide/claude-code.html)
- [Claude 封号了怎么办](https://kw.yaoyao.chat/guide/claude-fenghao.html)
- [AI 会员价格对比](https://kw.yaoyao.chat/guide/ai-huiyuan-jiage.html)
- 同一作者的其他仓库：[Claude Code 国内使用指南](claude-code.md)、[OpenAI Codex CLI 国内使用指南](codex-cli.md)、[GPT代充指南](chatgpt-plus.md)

## 关于本仓库和作者

本仓库由"瑶瑶ai训练师"整理，作者是做 AI 内容的自媒体博主，教程基于自己的使用和售后经验。与 Anthropic、OpenAI 没有隶属关系，文中品牌名仅用于说明。作者是谁、怎么交易、售后和退款规则，见 [瑶瑶ai训练师靠谱吗](https://kw.yaoyao.chat/guide/yaoyao-kaopu.html)。官方价格和权益以 Anthropic 官网为准。瑶瑶没有发布过任何桌面软件、手机 App、浏览器插件或"账号切换器"，本账号下只有文字教程仓库。

## 参考资料

- [Anthropic 官方定价页](https://claude.com/pricing)
- [支持的国家和地区](https://www.anthropic.com/supported-countries)
- [What is the Pro plan?](https://support.claude.com/en/articles/8325606-what-is-the-pro-plan)
- [What is the Max plan?](https://support.claude.com/en/articles/11049741-what-is-the-max-plan)
- [Paid plan billing FAQs](https://support.claude.com/en/articles/8325618-paid-plan-billing-faqs)
- [How do usage and length limits work?](https://support.claude.com/en/articles/11647753-how-do-usage-and-length-limits-work)
- [Manage usage credits for paid Claude plans](https://support.claude.com/en/articles/12429409-manage-usage-credits-for-paid-claude-plans)
- [Use Claude Code with your Pro or Max plan](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan)
- [Troubleshoot Claude error messages](https://support.claude.com/en/articles/12466728-troubleshoot-claude-error-messages)
- [How to get support](https://support.claude.com/en/articles/9015913-how-to-get-support)
- [Claude Code 错误参考](https://code.claude.com/docs/en/errors)
- [Claude Code 登录与认证](https://code.claude.com/docs/en/authentication)

## 复测记录

按日期倒序。每次只记真实做过的核对；官方出新模型、改价格时补一行。

| 日期 | 核对了什么 | 结果 |
|---|---|---|
| 2026-10-27 | **价格：** curl 作者商城商品页 item/5、7、10、11、12、13、14、17、18、19 和 llms.txt | 与本页"快速购买"一致（Pro 100 美金档位 ¥699、Plus ¥129、Claude Pro ¥159、Max 5X ¥900），十个商品均无变动 |
| 2026-10-26 | **官方价格：** Claude 定价页、帮助中心 What is the Max plan | Pro 月付 20 美元 / 年付折合 17 美元（一次 200 美元）；Max 5x 100、Max 20x 200 美元；Max 含每月 API 额度；官方注明手机端价格可能不同——与本页价格表一致 |
| 2026-10-26 | **官方政策：** Anthropic 支持地区列表、账单 FAQ、赠送订阅文章 | 大陆、香港、澳门不在支持列表，台湾在；App 内订阅由苹果 / 谷歌管理；赠送订阅暂停购买 |

## 作者商城：代充方式中的一种（如实披露）

上面讲的"代充"有很多家在做，本合集作者瑶瑶ai训练师自己经营的商城 [kw.yaoyao.chat](https://kw.yaoyao.chat/?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=claude-chongzhi) 是其中一家。为了不重复，全部商品的价格、开通流程、售后三条和客服方式统一放在两处：[合集首页的作者商城价格表](../README.md#作者商城价格表人民币) 和 [作者商城商品说明](shangcheng.md)。价格每周按商品页核对，实际以下单页为准；付款方式支付宝、微信；会员开到你自己的账号，不要密码。

## 合集里的其他章节

本文是 [国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集](https://github.com/yaoyao-ai-trainer/yaoyao-ai-trainer.github.io) 的一章，其他章节：

- [ChatGPT Plus 国内怎么开通：官方订阅、应用内购、礼品卡、代充四种方法怎么选](chatgpt-plus.md)
- [没有信用卡怎么开通 ChatGPT Plus：支付宝 / 微信能不能付、礼品卡、应用内购、代充](chatgpt-plus-wu-xinyongka.md)
- [ChatGPT Pro 100 美金档位国内怎么买：Pro 100 / 200 / 500 三档区别、和 Plus 差在哪](chatgpt-pro-100.md)
- [ChatGPT / Claude / Gemini / Grok 会员价格对比：四家官方价、约合人民币、代充价怎么算账](jiage-duibi.md)
- [Claude Pro / Max 国内怎么开通：官方订阅、应用内购、赠送订阅、代充四种方法怎么选](claude-daichong.md)
- [Claude 代充靠谱吗：代充原理、要交出什么信息、风险在哪](claude-kaopu-yuanli.md)
- [Claude Code 国内使用指南：安装、登录、Pro / Max 额度怎么选、常见报错](claude-code.md)
- [OpenAI Codex CLI 国内使用指南：安装、ChatGPT 账号登录、多账号切换、Plus / Pro 额度、常见报错](codex-cli.md)
- [Grok Premium（原 SuperGrok）国内怎么买：官方四档价格、三合一说明、四种开通方法](grok-premium.md)
- [Grok 代充：什么账号能充、怎么开通、靠谱吗](grok-daichong.md)
- [Gemini Pro（Google AI Pro）国内代充：怎么开通、开通后怎么确认生效、常见问题](gemini-pro.md)
- [AI 会员订阅国内指南：ChatGPT / Claude / Gemini / Grok 开通路线对比、代充判断 8 条](ai-subscription.md)
- [常见问题详细版：能不能用、代充、档位](faq-xiangxi.md)
- [作者商城商品说明：全部商品价格、开通流程、售后](shangcheng.md)
- [报错速查表：ChatGPT / Claude / Claude Code / Codex 常见报错](baocuo-sucha.md)
- [全部复测记录（按日期）](fuce-jilu.md)
- [回到合集首页](../README.md)
