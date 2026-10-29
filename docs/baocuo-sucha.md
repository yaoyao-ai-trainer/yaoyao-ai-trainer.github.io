# AI 会员报错速查表：ChatGPT / Claude / Claude Code / Codex / Grok 常见报错一页索引

> 本页是《国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集》的一章（[合集首页](../README.md)）。每条报错的详细处理（现象 → 原因 → 怎么处理，附官方链接）在对应的原仓库里，这里只放一句话判断和去哪看。

> **立场说明：** 整理：瑶瑶ai训练师。作者自己经营一家 AI 会员代充商城（kw.yaoyao.chat），所以本文不是第三方评测；作者商城的价格、开通流程和售后统一放在 [作者商城商品说明](shangcheng.md)。与 OpenAI、Anthropic、Google、xAI 没有隶属关系，也没有授权，品牌名仅用于说明。

常见报错分 ChatGPT、Claude、Claude Code、Codex CLI、Grok 五类。这一页只放一句话判断和该去哪看；每一条的详细处理（现象 → 原因 → 怎么处理，并附官方链接）都在对应的仓库里，点"详细处理"一列直接跳到那一节。

| 你看到的 | 多半是 | 详细处理 |
|---|---|---|
| ChatGPT 付款提示"请核对账单信息后重试"或 Your card was declined | 卡号、有效期、账单地址和发卡行登记的对不上，被银行拦下，或者你 / 发卡行不在支持地区 | [gpt-chongzhi 第 1 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#1-付款时提示请核对账单信息后重试英文界面类似-your-card-was-declined) |
| 国内银行卡、双币卡被拒，付款页没有支付宝 | 官网只收主要信用卡，结算以支持地区为前提 | [gpt-chongzhi 第 2 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#2-卡被拒card-declined国内银行卡--支付宝付不了) |
| 已是 Plus，想换 Pro 找不到入口，或提示账号已有订阅 | 订阅按购买渠道（网页、App Store、Google Play）分开管理，或账号上已有生效的订阅 | [gpt-chongzhi 第 3 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#3-已有订阅想升级到-pro-或换档位找不到入口--提示账号已有订阅) |
| 付了钱或代充显示成功，ChatGPT 还是 Free | 现在登录的邮箱或登录方式和付款时不是同一个，App 购买没同步，或页面没刷新 | [gpt-chongzhi 第 5 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#5-付了钱或代充显示成功但账号还是-free) |
| 提示达到用量上限，某个模型暂时用不了 | 按滚动时间窗口计算的额度用完了，要等重置 | [gpt-chongzhi 第 9 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#9-用着提示达到用量上限某个模型暂时不可用) |
| 开了 Plus，API 余额还是 0，或 Codex 让升级套餐 | 会员和 API 分开计费；Codex 登录时没选 Sign in with ChatGPT，或登的不是有会员的那个号 | [gpt-chongzhi 第 10 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#10-开了-plusapi-还是没额度--codex-提示要升级) |
| ChatGPT 账号被停用（Deactivated） | 在不支持的地区访问，或违反使用政策，具体原因看官方邮件 | [gpt-chongzhi 第 11 条](https://github.com/haiwaihuyonghui-rgb/gpt-chongzhi#11-账号被停用deactivated) |
| Claude 升级或代充后还是 Free Plan | 登录的邮箱不是开通的那个，付款失败被降级，或停在了团队空间 | [claude-chongzhi 第 1 条](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#1-升级或代充之后还是显示-free-plan) |
| 在 console.anthropic.com 充了钱，会员没变 | 那是 API 平台，和 claude.ai 会员是两套账 | [claude-chongzhi 第 2 条](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#2-钱充到了-consoleanthropiccomapi-平台会员没变) |
| "5-hour limit reached" 或 "You've reached your weekly limit" | 5 小时会话额度或每周上限用完，网页、手机和 Claude Code 共用一份 | [claude-chongzhi 第 3 条](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#3-提示-5-hour-limit-reached--youve-reached-your-weekly-limit额度怎么算) |
| "Due to unexpected capacity constraints…" | 同时请求的人太多，临时容量不足，不占你的额度 | [claude-chongzhi 第 9 条](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#9-提示-due-to-unexpected-capacity-constraints-claude-is-unable-to-respond) |
| Claude 账号被停用（Account disabled） | 在不支持的地区使用、多人共用、付款被撤销等，以官方邮件为准 | [claude-chongzhi 第 11 条](https://github.com/haiwaihuyonghui-rgb/claude-chongzhi#11-账号被停用account-disabled) |
| Claude Code 提示 `Credit balance is too low` 或让去充 API | 登录成了 Console 账号，或环境变量里的 `ANTHROPIC_API_KEY` 优先于订阅 | [claude-code-guide-cn 报错一节](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#报错--常见问题大全) |
| `command not found: claude` | 安装目录没加进 PATH，或者装完没新开终端 | [claude-code-guide-cn 报错一节](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#报错--常见问题大全) |
| 安装时出现 `syntax error near unexpected token '<'`、403 或 `App unavailable in region` | 安装地址返回的是网页：被网络拦截，或所在国家不受支持 | [claude-code-guide-cn 报错一节](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#报错--常见问题大全) |
| Codex 登录后提示要升级套餐 | 登录的账号没开会员，或登成了另一个邮箱 | [codex-cli-guide-cn 报错一节](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#常见报错与解决) |
| Codex 被扣了 API 费用 | 登录时选成了 API Key，没走会员额度 | [codex-cli-guide-cn 报错一节](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#常见报错与解决) |
| Codex 安装脚本下载失败 | 默认下载地址暂时不通，可改从 GitHub Releases 下载或换 npm、Homebrew | [codex-cli-guide-cn 报错一节](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#常见报错与解决) |
| 已是 SuperGrok / Premium 会员，Grok 代充充不了 | 正本所写的代充只限免费版账号，付费会员要等到期 | [grok-daichong 账号条件](https://github.com/haiwaihuyonghui-rgb/grok-premium/blob/main/grok-daichong.md#下单前先确认你的账号能不能充) |
| Grok 开通后看不到会员，或手机上找不到 sso | 登录方式和平时不同；sso 要在电脑浏览器的 Cookie 里复制 | [grok-daichong 开通 4 步](https://github.com/haiwaihuyonghui-rgb/grok-premium/blob/main/grok-daichong.md#怎么开通4-步) |

处理办法以 OpenAI、Anthropic、xAI 官方帮助中心的最新说明为准，上面各仓库里每条都附了官方出处。通过代充开通的订单出了问题（开通失败、本期内掉会员等），先找卖家处理：钱是卖家付的，官方那边没有你的付款记录，也就无从处理。

## 合集里的其他章节

谷歌站版攻略（同一作者整理，手机上看更方便；[全部 15 页入口](../README.md#谷歌站版攻略)）：

- [ChatGPT 订阅提示"银行卡被拒绝"怎么办：原因排查和三种正规解决方案](https://sites.google.com/view/yaoyao-ai/yinhangka-jujue)
- [ChatGPT Plus 续费扣款失败怎么办：先排查这 4 个原因](https://sites.google.com/view/yaoyao-ai/xufei-shibai)
- [ChatGPT 注册教程：国内怎么注册账号、App 下载和常见问题](https://sites.google.com/view/yaoyao-ai/chatgpt-zhuce)

本文是 [国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集](https://github.com/yaoyao-chat/yaoyao-chat.github.io) 的一章，其他章节（每章是摘要，完整正文在各自的原仓库）：

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
