# AI 会员报错速查表：ChatGPT / Claude / Claude Code / Codex 付款、开通、额度、封号常见报错怎么处理

> 本页是《国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集》的一章（[合集首页](../README.md)）。把原来分散在 4 个仓库里的报错整理到一页：先查速查表，再看对应产品的详细条目。每条按"现象 → 原因 → 怎么处理"写，处理办法来自官方帮助中心并附官方链接；官方没写到的地方注明"以官方说明为准"。

> **立场说明：** 整理：瑶瑶ai训练师，作者自营代充商城（kw.yaoyao.chat），非官方；链接到 kw.yaoyao.chat/guide/ 的是作者自己写的教程页，标"官方"的是厂商文档。

## 目录

- [一页速查](#一页速查)
- [ChatGPT：12 个报错](#chatgpt12-个报错)
- [Claude：12 个报错](#claude12-个报错)
- [Claude Code 报错](#claude-code-报错)
- [Codex CLI 报错](#codex-cli-报错)
- [Grok 开通前先确认](#grok-开通前先确认)
- [合集里的其他章节](#合集里的其他章节)

## 一页速查

下面的链接指向作者整理的教程页，每页有更新日期；标了"官方"的是厂商文档。

| 你看到的 | 多半是 | 看这篇 |
|---|---|---|
| 付款提示"请核对账单信息后重试" / Your card was declined | 卡不在支持地区，或账单地址和发卡行登记的不一致 | [账单信息无效怎么办](https://kw.yaoyao.chat/guide/chatgpt-billing-invalid.html)、[账单地址怎么填](https://kw.yaoyao.chat/guide/zhangdan-dizhi.html) |
| 国内银行卡付不了 | 发卡地区不受支持 | [银行卡不能用怎么办](https://kw.yaoyao.chat/guide/yinhangka.html)、[可以用支付宝吗](https://kw.yaoyao.chat/guide/chatgpt-zhifubao.html) |
| 显示"已有订阅 / 无法升级" | 账号上已有一份订阅，Plus 升 Pro 要补差价 | [已有订阅怎么办](https://kw.yaoyao.chat/guide/plus-sheng-pro.html) |
| 代充提交失败 | 登录信息过期、复制不完整、通道风控等 6 种情况 | [Plus 充值失败 6 种情况](https://kw.yaoyao.chat/guide/plus-shibai.html)、[卡密怎么用](https://kw.yaoyao.chat/guide/plus-kami.html) |
| 用手机号验证码登录的账号怎么开 Plus | 登录方式不同，开通流程不同 | [手机验证码登录怎么开 Plus](https://kw.yaoyao.chat/guide/plus-yanzhengma.html) |
| Plus / Codex 提示额度用完 | 5 小时窗口或每周上限 | [Plus 每天能用多少](https://kw.yaoyao.chat/guide/plus-edu.html)、[Codex 额度用完了怎么办](https://kw.yaoyao.chat/guide/codex-edu-yongwan.html) |
| Claude 充了还是 Free Plan | 登录了别的邮箱；钱充到了 API 平台；付款失败被降级 | [Claude 显示 Free Plan 怎么办](https://kw.yaoyao.chat/guide/claude-free-plan.html)、官方 [Paid plan billing FAQs](https://support.claude.com/en/articles/8325618-paid-plan-billing-faqs) |
| Claude Code 提示去充 API / Credit balance is too low | 登录成了 Console 账号，或环境变量里有旧的 ANTHROPIC_API_KEY | [Claude Code 怎么收费](https://kw.yaoyao.chat/guide/claude-code.html)、官方 [Claude Code 错误参考](https://code.claude.com/docs/en/errors) |
| Claude 提示 session limit / weekly limit | 5 小时窗口或每周额度用完 | [Claude Pro 有多少额度](https://kw.yaoyao.chat/guide/claude-pro-edu.html)、官方 [How do usage and length limits work?](https://support.claude.com/en/articles/11647753-how-do-usage-and-length-limits-work) |
| 账号被停用 | 共享、频繁切换地区、付款被撤销、违规内容 | [ChatGPT 封号原因](https://kw.yaoyao.chat/guide/chatgpt-fenghao.html)、[Claude 封号了怎么办](https://kw.yaoyao.chat/guide/claude-fenghao.html) |
| 想取消自动续费 | 自己绑卡的在设置里取消；App 内订阅在手机订阅设置里取消 | [自动续费怎么取消](https://kw.yaoyao.chat/guide/cancel-renew.html) |
| 想退款 | 官方条款下订阅费一般不退；代充的不能向官方申请 | [ChatGPT 订阅能退款吗](https://kw.yaoyao.chat/guide/chatgpt-tuikuan.html) |
| 代充突然停了 | 通道补额度、风控或卖家自身原因 | [代充为啥突然停了](https://kw.yaoyao.chat/guide/daichong-tingle.html) |
| Codex 想切换多个账号 | 官方本身支持 | [Codex 怎么切换多个账号](https://kw.yaoyao.chat/guide/codex-duozhanghao.html) |

更多：[教程目录（45 篇）](https://kw.yaoyao.chat/guide/)。

## ChatGPT：12 个报错

每条按"现象 → 原因 → 怎么处理"写，处理办法来自 OpenAI 官方帮助中心，并附官方链接；官方没写到的地方注明"以官方说明为准"。

### 1. 付款时提示"请核对账单信息后重试"（英文界面类似 Your card was declined）

- **现象：** 在 chatgpt.com 升级 Plus / Pro，填完卡点付款，页面提示"请核对账单信息后重试"，或者英文提示卡被拒。
- **原因：** 这是付款被拒后的统一提示。官方列出的常见原因：卡号、有效期、账单地址填错或和发卡行登记的不一致；银行出于安全原因拦截，或余额不足；你本人或发卡行所在地不在 OpenAI 支持地区（官方原话：如果任一方在支持地区之外，付款可能被拒）。官方页面没有逐字解释这条中文提示，以官方说明为准。
- **怎么处理：** 按官方建议：①核对卡号、有效期、账单地址，账单地址填发卡行登记的真实地址（见 [ChatGPT 订阅账单地址怎么填](https://kw.yaoyao.chat/guide/zhangdan-dizhi.html?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=chatgpt-plus)）；②清除浏览器缓存和 Cookie 后再试一次；③联系银行，确认是否被拦截、余额是否足够；④确认你和发卡行都在支持地区；⑤都不行，用帮助中心右下角的聊天窗口联系 OpenAI 支持。不要短时间内反复点付款，连续被拒会更难通过。
- **官方出处：** [Why did my ChatGPT Plus or ChatGPT Pro renewal transaction fail?](https://help.openai.com/en/articles/7242622-why-did-my-chatgpt-plus-or-chatgpt-pro-renewal-transaction-fail)、[Supported countries and territories](https://platform.openai.com/docs/supported-countries)

### 2. 卡被拒（card declined）、国内银行卡 / 支付宝付不了

- **现象：** 国内发行的信用卡、借记卡、双币卡被拒；付款页没有支付宝等国内付款选项。
- **原因：** 官方定价页写明 Go / Plus / Pro / Business 接受主流信用卡；结算以支持地区为前提，国内发行的银联卡、支付宝不在范围内，双币卡也经常因为发卡行所在地被拒。
- **怎么处理：** 换支持地区发行的卡，或者改用代充（由卖家付款，会员开到你自己的账号）。更多情况见 [ChatGPT 充值银行卡不能用怎么办](https://kw.yaoyao.chat/guide/yinhangka.html?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=chatgpt-plus) 和 [ChatGPT 可以用支付宝吗](https://kw.yaoyao.chat/guide/chatgpt-zhifubao.html?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=chatgpt-plus)。
- **官方出处：** [OpenAI 定价页 FAQ](https://openai.com/chatgpt/pricing/)、[续费失败说明](https://help.openai.com/en/articles/7242622-why-did-my-chatgpt-plus-or-chatgpt-pro-renewal-transaction-fail)

### 3. 已有订阅，想升级到 Pro 或换档位，找不到入口 / 提示账号已有订阅

- **现象：** 账号已经是 Plus，想换成 Pro，或者 Pro 100 想换 Pro 200，页面没有想要的选项；在代充平台提交时提示"该账号已有订阅或近期付款记录"。
- **原因：** ChatGPT 的订阅由购买渠道管理：网页（chatgpt.com）、Apple App Store、Google Play 各自独立。官方说明：换方案要用现有账号，在 **Settings → My Plan** 查看当前订阅和可以切换的方案；在 App Store / Google Play 订阅的，网页上管不了，要先在对应商店处理。同一个账号在两个渠道各订一份，会重复扣费。代充平台的"已有订阅"类提示，一般是因为账号当前已有生效订阅或刚付过款，通道不会重复开通。
- **怎么处理：** 网页订阅：Settings → My Plan 看可用的升级 / 切换；App 内订阅：先在 App Store / Google Play 管理。降级或取消在当前账期结束时生效，期间可以撤回。
- **官方出处：** [About ChatGPT Pro tiers](https://help.openai.com/en/articles/9793128-about-chatgpt-pro-tiers)、[How do I avoid being charged twice](https://help.openai.com/en/articles/20001043-how-do-i-avoid-being-charged-twice-if-i-subscribe-to-chatgpt-on-ios-android-and-the-web)

### 4. Plus 到期了 / 续费扣款失败，账号变回免费版

- **现象：** 到了续费日没扣成功，收到付款失败邮件，账号变回 Free。
- **原因：** 官方说明续费偶尔会因为安全措施或支付方式本身的问题失败，常见是银行拦截、卡过期或余额不足、浏览器缓存干扰、你或发卡行不在支持地区。取消订阅或续费失败后，付费功能用到当前账期结束，之后回到免费版。
- **怎么处理：** 自己绑卡的：按官方建议清缓存、核对卡信息和账单地址、联系银行，然后在 Settings → Billing 重新订阅；代充开通的：不走你的银行卡，到期前重新下单一次即可。
- **官方出处：** [续费失败说明](https://help.openai.com/en/articles/7242622-why-did-my-chatgpt-plus-or-chatgpt-pro-renewal-transaction-fail)、[Canceling your ChatGPT subscription](https://help.openai.com/en/articles/7232927-how-do-i-cancel-my-chatgpt-plus-subscription)

### 5. 付了钱（或代充显示成功）但账号还是 Free

- **现象：** 扣款成功、收到收据，登录后还是免费版；或者代充页面显示成功，ChatGPT 里看不到 Plus。
- **原因：** 官方列出的原因：现在登录的邮箱或登录方式（Google / Apple / 邮箱密码）和付款时的账号不一致；手机 App 内购买没同步到账号；页面没刷新。
- **怎么处理：** 官方建议：①确认登录的就是付款时的账号和登录方式；②手机 App 里点"Restore purchases（恢复购买）"；③退出再重新登录；④仍不行，带收据或卡号后 4 位联系 OpenAI 支持。代充开通的找卖家处理，因为付款不是你本人完成的，官方查不到你的付款记录。
- **官方出处：** [What is ChatGPT Plus?](https://help.openai.com/en/articles/6950777-what-is-chatgpt-plus)

### 6. 被扣了两次钱

- **现象：** 信用卡和 App Store（或 Google Play）同时出现 ChatGPT 的扣款。
- **原因：** 网页和应用商店各自独立计费，在一边订了、另一边没取消就会双份。官方特别提醒：Apple 续费失败不会自动取消，Apple 会持续重试，你更新 Apple 付款方式后可能又把它续上。
- **怎么处理：** 按官方步骤查三处：iPhone 设置 → 你的姓名 → 订阅；Google Play → 订阅；chatgpt.com Settings → Account / Billing。留一份，其余在对应渠道取消。Apple 购买的退款找 Apple；Google Play 购买的通过 OpenAI 支持申请；两份订阅不自动退款，重复扣费的错误可以申请复核。
- **官方出处：** [How do I avoid being charged twice](https://help.openai.com/en/articles/20001043-how-do-i-avoid-being-charged-twice-if-i-subscribe-to-chatgpt-on-ios-android-and-the-web)

### 7. 想取消自动续费 / 想退款

- **现象：** 不想下个月继续扣钱，或者刚付完想退。
- **原因 / 规则：** 取消只是停止以后的续费，不会自动退已付的费用；付费功能保留到当前账期结束。退款资格按购买情况和所在地规定另行评估，获批后通常 5–10 个工作日到账。
- **怎么处理：** 网页：Settings → Billing → Cancel plan；iPhone：设置 → 姓名 → 订阅 → ChatGPT → 取消订阅；安卓：Play 商店 → 订阅 → ChatGPT → 取消。官方建议在下次扣款日前至少 24 小时取消。代充开的会员不走你的卡，不会自动续费，不用取消。
- **官方出处：** [Canceling your ChatGPT subscription](https://help.openai.com/en/articles/7232927-how-do-i-cancel-my-chatgpt-plus-subscription)、[What is ChatGPT Plus?](https://help.openai.com/en/articles/6950777-what-is-chatgpt-plus)

### 8. Pro 100 / 200 / 500 美金档位有什么区别？Pro 200 为什么额度变了？

- **现象：** 升级页只写 Pro"From 100 美元"和"3 档用量"，看不懂差别；有人说 Pro 200 额度被砍了。
- **说明（官方）：** 三档都包含 Pro 模型、Codex、深度研究、图像生成、记忆、文件上传，差别在"包含的用量"高低和 Ultrafast：只有 Pro 500 有 Ultrafast（GPT-6 Astra、GPT-6.1 Sol，按标准速率的 8 倍扣用量）；Pro 100 / 200 买 credits 也不能解锁 Ultrafast。Pro 200 的新订阅自 2026 年 9 月底起用量比以前低，价格不变；老用户过渡期到 2026-10-29。额度用完后对应模型要等重置，官方支持不能帮你重置。
- **怎么处理：** 按用量选档；不确定先买低一档用一周。三档只能月付。
- **官方出处：** [About ChatGPT Pro tiers](https://help.openai.com/en/articles/9793128-about-chatgpt-pro-tiers)

### 9. 用着提示达到用量上限、某个模型暂时不可用

- **现象：** 对话中提示已达上限，某个模型在重置时间前用不了。
- **原因：** Plus / Pro 没有固定的每日条数，额度按模型、上下文长度、推理和工具使用等折算，按滚动时间窗口计算；到上限后该模型在重置前不可用。
- **怎么处理：** 等提示里的重置时间；换轻量模型继续；经常碰上限就升一档。Codex 用量到顶后 Plus / Pro 可以购买 credits 继续。
- **官方出处：** [About ChatGPT Pro tiers](https://help.openai.com/en/articles/9793128-about-chatgpt-pro-tiers)、[Codex 定价页](https://developers.openai.com/codex/pricing)

### 10. 开了 Plus，API 还是没额度 / Codex 提示要升级

- **现象：** platform.openai.com 显示余额为 0；Codex 登录后提示升级套餐。
- **原因：** 会员和 API 分开计费（Plus 帮助文章原文：API 用量单独计费）。Codex 要用 **Sign in with ChatGPT** 登录开了会员的账号才算在会员里，用 API Key 登录按 API 价扣钱；登录了没会员的另一个邮箱也会提示升级。
- **怎么处理：** 需要 API 的到 platform.openai.com 另充；Codex 里 `codex logout` 后重新选 Sign in with ChatGPT，用开了会员的账号登录。详见 [OpenAI Codex CLI 国内使用指南](codex-cli.md)。
- **官方出处：** [What is ChatGPT Plus?](https://help.openai.com/en/articles/6950777-what-is-chatgpt-plus)、[Codex 定价页](https://developers.openai.com/codex/pricing)

### 11. 账号被停用（Deactivated）

- **现象：** 登录提示账号已停用，收到 OpenAI 的通知邮件。
- **原因：** 官方会在邮件里说明原因；OpenAI 支持地区页面写明在不支持的地区访问可能导致账号被封禁或停用，其他常见原因是违反使用政策（多人共用、脚本批量调用等）。
- **怎么处理：** 先看邮箱里的通知，按邮件里的指引申诉；能否恢复、订阅费是否退以官方处理结果为准。代充开通的订单找卖家确认质保范围。更多见 [ChatGPT 封号原因有哪些](https://kw.yaoyao.chat/guide/chatgpt-fenghao.html?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=chatgpt-plus)。
- **官方出处：** [Supported countries and territories](https://platform.openai.com/docs/supported-countries)、[OpenAI 使用政策](https://openai.com/policies/usage-policies/)

### 12. 自助开通（卡密方式）常见提示

下面这些提示来自自助充值页的实际使用经验，不是 OpenAI 官方报错，完整版见 [ChatGPT Plus 充值失败怎么办](https://kw.yaoyao.chat/guide/plus-shibai.html?utm_source=github&utm_medium=org&utm_campaign=yaoyao-ai-trainer&utm_content=chatgpt-plus)：

| 提示或情况 | 原因 | 怎么办 |
|---|---|---|
| accessToken 已过期 | 复制的登录信息放久了 | 用无痕窗口重新登录 ChatGPT，打开 chatgpt.com/api/auth/session，复制后 1 分钟内提交 |
| 登录凭证无效 / 格式不对 | 没有复制完整 | 在那个页面全选再复制，内容应以 { 开头、} 结尾 |
| 识别到的邮箱不是要充的账号 | 无痕窗口里登录错了账号 | 退出，换成要开通的账号重新登录再复制 |
| 银行卡支付未获通过 | 充值通道付款时被支付风控拦下 | 卡密自动退回，隔一段时间再试，连续重提容易触发暂停 |
| 充值通道暂时不可用 | 通道正在补充额度 | 卡密不会被扣，稍后再试 |
| 一直转圈 | 上游还在处理 | 不要重复提交，等 3 分钟再刷新 ChatGPT |
| 显示成功但看不到 Plus | 页面没刷新 | 退出重新登录，App 里下拉刷新 |

手机上操作失败，多半是：用了 ChatGPT App（要用手机浏览器）、在 App 内置浏览器里打开（要换系统浏览器）、没用无痕模式、长按只选中了一部分文字。能用电脑浏览器就用电脑。

安全提醒：登录信息相当于临时登录凭证，只粘贴到你信任的充值页，不要发到群里；开通后在 ChatGPT「设置 → 安全」里退出所有设备，它就失效了。

## Claude：12 个报错

每条按"现象 → 原因 → 怎么处理"写，处理办法来自 Anthropic 官方帮助中心和 Claude Code 官方文档，并附链接；官方没写到的地方注明"以官方说明为准"。

### 1. 升级（或代充）之后还是显示 Free Plan

- **现象：** 付款成功或代充显示成功，claude.ai 右上角还是 Free，升级入口还在。
- **原因：** 官方账单 FAQ 列了两条：登录的邮箱和开通会员的邮箱不是同一个；付款方式失败导致账号被降级。实际还常见：当前在团队（Team）空间里、手机订阅后电脑没登录同一个账号、页面没刷新。
- **怎么处理：** ①退出再重新登录，手机 App 也一样；②用你可能注册过的其他邮箱、其他登录方式（Google / 邮箱）各试一次；③Settings → Billing 看最近一次付款状态，失败的话更新付款方式；④切换回个人账户；⑤手机上订阅的，电脑上登录同一个账号。代充的订单找卖家处理。
- **官方出处：** [Paid plan billing FAQs](https://support.claude.com/en/articles/8325618-paid-plan-billing-faqs)。完整排查见 [Claude 充值了还是显示 Free Plan 怎么办](https://kw.yaoyao.chat/guide/claude-free-plan.html)。

### 2. 钱充到了 console.anthropic.com（API 平台），会员没变

- **现象：** 在 console.anthropic.com / platform.claude.com 充了钱，余额有了，但 claude.ai 还是 Free。
- **原因：** 那是 API 平台，充的是 API 额度，和会员订阅是两套分开计费的账户，不会变成 Pro。
- **怎么处理：** 会员要在 claude.ai 的设置里升级；API 余额按 API 用量消耗，官方说明 API 用量从不计入会员账单。
- **官方出处：** [Paid plan billing FAQs](https://support.claude.com/en/articles/8325618-paid-plan-billing-faqs)、[What is the Pro plan?](https://support.claude.com/en/articles/8325606-what-is-the-pro-plan)

### 3. 提示 "5-hour limit reached" / "You've reached your weekly limit"，额度怎么算

- **现象：** 对话中出现 `5-hour limit reached - resets [时间]` 或 `You've reached your weekly limit. It resets [星期] at [时间]`；Claude Code 里是 `You've hit your session limit · resets 3:45pm` 或 `You've hit your weekly limit`。
- **原因：** 每个套餐都有按滚动 5 小时窗口重置的会话额度，付费套餐另有每周上限（每周在账号固定的时间重置）。消耗多少取决于对话长短、复杂度、模型、用的功能和推理强度；网页、桌面、手机、Claude Code 共用同一份。官方没有公布具体条数。
- **怎么处理：** 等提示里的重置时间；Settings → Usage 看两条进度条；开长对话前新建会话、减少附件、关掉不需要的工具能省额度；经常碰上限就升一档（官方说明升级后新额度立刻生效）；或者开启用量额度（见第 6 条）。
- **官方出处：** [How do usage and length limits work?](https://support.claude.com/en/articles/11647753-how-do-usage-and-length-limits-work)、[Troubleshoot Claude error messages](https://support.claude.com/en/articles/12466728-troubleshoot-claude-error-messages)、[Claude Code 错误参考](https://code.claude.com/docs/en/errors)

### 4. Pro、Max 5x、Max 20x 到底差在哪？升级怎么算钱？

- **现象：** 不知道买哪档；从 Pro 升 Max 怕被重复扣一个月。
- **说明（官方）：** Max 5x 是 Pro 每 5 小时额度的 5 倍，Max 20x 是 20 倍，三档都含 Claude Code；Max 另有新模型和新功能的优先体验、每月 API credits（只能在 API 平台用）。从低档升高档按剩余账期比例补差价，立刻生效。年付 Pro 升 Max 时，剩余年费多于 Max 价格的部分会变成账户余额；账单地址变了要先取消 Pro、等到期再订 Max。
- **怎么处理：** 按上面"Pro 和 Max 怎么选"选档；在 claude.ai Settings → Billing 里升级。
- **官方出处：** [What is the Max plan?](https://support.claude.com/en/articles/11049741-what-is-the-max-plan)、[Anthropic 定价页](https://claude.com/pricing)

### 5. Claude Code 登录后提示要充 API，或出现 "Credit balance is too low"

- **现象：** 明明有 Pro / Max，Claude Code 却提示余额不足、让去 Console 充值，或者显示按 API 计费。
- **原因：** 两种情况：登录时选了 Anthropic Console 账号（API 计费）而不是 Claude 订阅账号；或者电脑环境变量里有 `ANTHROPIC_API_KEY`，官方说明这个变量优先于订阅，即使有 Pro / Max 也会按 API 扣费。
- **怎么处理：** 在 Claude Code 里输入 `/login`，选择用 Claude 账号（订阅）登录；有 API Key 变量的，先 `unset ANTHROPIC_API_KEY`（Windows PowerShell 用 `Remove-Item Env:ANTHROPIC_API_KEY`），把 `~/.zshrc`、`~/.bashrc` 里的 `export` 行删掉，重开终端后 `/status` 确认当前用的是订阅。官方还建议：不想碰 API 账单就 `claude logout` 再 `claude login`，只用 Pro / Max 账号登录，不要添加 Console 凭据。
- **官方出处：** [Use Claude Code with your Pro or Max plan](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan)、[Claude Code 错误参考：Credit balance is too low](https://code.claude.com/docs/en/errors)

### 6. 额度用完还想继续：用量额度（usage credits）是什么

- **现象：** 到上限不想等，又不想马上升档。
- **说明（官方）：** Pro、Max 5x、Max 20x 都可以在 claude.ai 的 Settings → Usage 开启"Usage credits"：到上限后请求自动转成按量付费（按标准 API 价），可以设每月花费上限、预充金额、自动充值和提醒；这些费用和订阅费分开出现在账单上。Claude Code 里对应命令是 `/usage-credits`。在手机 App 订阅的，只能在网页版开启并先绑卡。Max 自带的每月 API credits 不能抵用量额度。
- **怎么处理：** 不想多花钱就不要开；开了记得设每月上限。
- **官方出处：** [Manage usage credits for paid Claude plans](https://support.claude.com/en/articles/12429409-manage-usage-credits-for-paid-claude-plans)

### 7. Claude Code 的登录选项里没有"订阅账号"

- **现象：** 运行 `claude` 登录时只看到 Console / API 的选项，看不到用 Claude 订阅登录。
- **原因：** 版本太旧，或者之前的登录状态没清干净。
- **怎么处理：** 官方步骤：`/logout` → 运行 `claude update` → 完全关掉终端再打开 → 运行 `claude`，选正确的账号登录。
- **官方出处：** [Use Claude Code with your Pro or Max plan](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan)

### 8. 网页登录报错 "There was an error logging you in"

- **现象：** claude.ai 登录时提示登录出错。
- **原因：** 官方列的常见原因：VPN、浏览器扩展、浏览器缓存和 Cookie 干扰；也可能是服务端故障。
- **怎么处理：** 官方建议：关掉 VPN、禁用浏览器扩展、清除缓存和 Cookie 再试；还不行看 [status.claude.com](https://status.claude.com) 有没有故障公告。
- **官方出处：** [Troubleshoot Claude error messages](https://support.claude.com/en/articles/12466728-troubleshoot-claude-error-messages)

### 9. 提示 "Due to unexpected capacity constraints, Claude is unable to respond..."

- **现象：** 发消息后提示容量不足、暂时无法回复。
- **原因：** 官方说明这是全体用户同时请求过多导致的临时情况，不是你的额度问题，也不算故障，不会出现在状态页上。
- **怎么处理：** 等几分钟再试。Claude Code 里对应的是 `529 Overloaded`，可以用 `/model` 换个模型继续，不扣你的额度。
- **官方出处：** [Troubleshoot Claude error messages](https://support.claude.com/en/articles/12466728-troubleshoot-claude-error-messages)、[Claude Code 错误参考](https://code.claude.com/docs/en/errors)

### 10. 付款方式、发票和取消订阅

- **现象：** 想换卡、要发票、想取消。
- **说明（官方）：** 网页订阅只接受信用卡和借记卡；App 内订阅的付款、收据和取消都由 App Store / Google Play 管理。换卡在 Settings → Billing 点 Update，新卡在下次续费时扣；发票在 Settings → Billing → Invoices 查看，也会发到账单邮箱（主题 "Your receipt from Anthropic"），已出的发票不能改。账单日不能直接改，只能取消后在想要的日期重新订。取消和退款规则见帮助中心"Cancel your Pro or Max subscription"文章，以官方为准。代充开的会员不走你的卡，不会自动续费。
- **官方出处：** [Paid plan billing FAQs](https://support.claude.com/en/articles/8325618-paid-plan-billing-faqs)

### 11. 账号被停用（Account disabled）

- **现象：** 登录后提示账号已停用，收到 Anthropic 邮件。
- **原因：** 官方会在邮件里说明；支持地区页面写明未列出的地区不受支持，其他常见原因是违反使用政策（多人共用、频繁换地区、付款被撤销等）。
- **怎么处理：** 先看邮箱通知，通过 Anthropic 官方帮助中心申诉：登录 claude.ai，点左下角头像 → Get help。能否恢复、是否退款以官方处理结果为准。代充订单找卖家确认质保范围。更多见 [Claude 封号了怎么办](https://kw.yaoyao.chat/guide/claude-fenghao.html)。
- **官方出处：** [How to get support](https://support.claude.com/en/articles/9015913-how-to-get-support)、[支持的国家和地区](https://www.anthropic.com/supported-countries)

### 12. 消息太长："Your message will exceed the length limit for this chat"

- **现象：** 粘贴长文或大文件后发不出去。
- **原因：** 单次输入超过了这个对话的上下文长度。官方说明一部分上下文始终留给 Claude 的回复；付费套餐开了代码执行后一般会自动压缩旧消息，所以这个提示不常见。
- **怎么处理：** 缩短、分段发，或新开对话。
- **官方出处：** [Troubleshoot Claude error messages](https://support.claude.com/en/articles/12466728-troubleshoot-claude-error-messages)、[How do usage and length limits work?](https://support.claude.com/en/articles/11647753-how-do-usage-and-length-limits-work)

## Claude Code 报错

下面每条按"你看到的 → 原因 → 怎么办"写，报错文字和处理办法来自官方文档，最后一列是出处，以官方最新说明为准。

| 你看到的 | 原因 | 怎么办 | 官方出处 |
|---|---|---|---|
| `command not found: claude` / `'claude' is not recognized` | 安装目录不在 PATH 里（macOS / Linux 是 `~/.local/bin`，Windows 是 `%USERPROFILE%\.local\bin`） | 先新开一个终端；还不行，macOS / Linux 运行 `echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc` 然后 `source ~/.zshrc`（bash 用 `~/.bashrc`）；Windows PowerShell 把 `%USERPROFILE%\.local\bin` 加进用户 PATH 后重开终端 | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `syntax error near unexpected token '<'`、`< was unexpected at this time` 或 `curl: (22) ... 403` | 安装地址返回的是网页而不是安装脚本：临时故障、代理或网络过滤拦截，或者所在国家不受支持（输出里会有 `App unavailable in region`） | 等几分钟重试；改用 Homebrew、WinGet 安装；`App unavailable in region` 说明当前所在国家不受支持，见 [支持的国家和地区](https://www.anthropic.com/supported-countries) | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `irm is not recognized` / `The token '&&' is not a valid statement separator` / `'bash' is not recognized` | 在 CMD 里跑了 PowerShell 命令，或反过来 | 看提示符：`PS C:\` 用 `irm ... | iex`，`C:\` 用 CMD 那条命令 | [安装说明](https://code.claude.com/docs/en/setup) |
| `Failed to fetch version from downloads.claude.ai` | 网络无法访问下载服务器 | 运行 `curl -sI https://downloads.claude.ai/claude-code-releases/latest` 测试，返回 200 才正常；403 多是代理或网络过滤，或地区不受支持；检查 `HTTPS_PROXY` 设置，见下文"网络与代理" | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `TLS connect error`、`unable to get local issuer certificate` 等 TLS 报错 | 系统根证书过旧，或公司代理做 TLS 检查 | 更新系统 CA 证书；公司代理用 `export NODE_EXTRA_CA_CERTS=/path/to/ca-cert.pem` 让它信任代理证书 | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `EACCES: permission denied`（npm 安装时） | npm 全局目录没有写权限 | 不要用 `sudo npm install -g`；官方建议改用原生安装脚本，或按排错页修复 npm 目录权限 | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `Unable to connect to Anthropic services`（后面跟 `ECONNREFUSED` 或 `timed out after 10 seconds`） | 首次启动时连不上 `api.anthropic.com` 或 `platform.claude.com` | 运行 `curl -I https://api.anthropic.com` 测试；检查提示里点名的代理变量是否正确、防火墙是否放行；官方提示网络正常仍失败时，可能是当前国家不可用 | [错误参考](https://code.claude.com/docs/en/errors) |
| `OAuth error: Invalid code. Please make sure the full code was copied` | 登录码过期或复制不完整；SSH 远程时浏览器开在了另一台机器上 | 回车重试，浏览器打开后尽快完成；按 `c` 复制完整链接；远程机器把终端里的链接复制到本地浏览器打开 | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| 浏览器登录后显示一串登录码，不跳回终端（WSL2、SSH、容器） | 浏览器连不上 Claude Code 本机的回调端口 | 把登录码粘贴到 `Paste code here if prompted` 处；粘贴没反应就运行 `claude auth login`；WSL2 浏览器打不开时设置 `export BROWSER="/mnt/c/Program Files/Google/Chrome/Application/chrome.exe"` 后再运行 `claude` | [登录与认证](https://code.claude.com/docs/en/authentication)、[安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `API Error: 403 Request not allowed` | 订阅未生效，或 Console 账号没有 "Claude Code" / "Developer" 角色；公司代理干扰 | Pro / Max 用户在 claude.ai/settings 确认订阅有效；Console 用户让管理员在 Members 页分配角色；代理环境见"网络与代理" | [安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `This organization has been disabled` 或 `Your ANTHROPIC_API_KEY belongs to a disabled organization`（但订阅有效） | 环境变量里有旧的 `ANTHROPIC_API_KEY`（常见是以前公司或项目留下的），它优先于订阅 | `unset ANTHROPIC_API_KEY`（PowerShell：`Remove-Item Env:ANTHROPIC_API_KEY`），删掉 `~/.zshrc`、`~/.bashrc` 或 `$PROFILE` 里的对应行，重新运行 `claude`，`/status` 确认 | [错误参考](https://code.claude.com/docs/en/errors) |
| `Credit balance is too low` | 用的是 Console 账号而 API 预付余额用完了；或者 `ANTHROPIC_API_KEY` 把请求导到了 API 账户 | 有 Pro / Max 的：`/status` 看当前凭据，有 API Key 就按上一条 unset 掉，必要时 `/login` 用订阅账号登录；确实要用 API 的到 platform.claude.com/settings/billing 充值 | [错误参考](https://code.claude.com/docs/en/errors)、[用 Pro / Max 使用 Claude Code](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan) |
| 登录选项里没有"订阅账号"，只能选 Console | 版本旧，或旧登录状态没清掉 | `/logout` → `claude update` → 完全关掉终端再打开 → `claude` 重新选账号 | [用 Pro / Max 使用 Claude Code](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan) |
| `Login expired · Please run /login`（脚本模式是 `Failed to authenticate: OAuth session expired and could not be refreshed`） | 保存的登录过期且无法刷新，Claude Code 已清掉凭据；系统时间不准也会导致 | 运行 `/login` 重新登录；经常出现就校准系统时钟；自动化脚本改用 `claude setup-token` 生成的长期令牌或 API Key | [错误参考](https://code.claude.com/docs/en/errors)、[安装与登录排错](https://code.claude.com/docs/en/troubleshoot-install) |
| `You've hit your session limit · resets 3:45pm` / `You've hit your weekly limit` / `Opus limit` / `Sonnet limit` | 5 小时窗口或每周额度用完；Opus / Sonnet 上限只针对该模型家族 | 等提示里的重置时间；`/usage` 看各窗口用量；Opus / Sonnet 上限时用 `/model` 换另一家族的模型；长期不够升级套餐，或 `/usage-credits` 开启用量额度 | [错误参考](https://code.claude.com/docs/en/errors) |
| `You've hit your monthly spend limit · raise it at ...` | 套餐额度和你设的用量额度每月上限都用完了 | Pro / Max 在 claude.ai Settings → Usage 调高上限，或运行 `/usage-credits`；有重置时间就等；Team / Enterprise 找管理员 | [错误参考](https://code.claude.com/docs/en/errors) |
| `Usage credits required for 1M context` | 选的是带 `[1m]` 后缀的 100 万上下文模型，你的套餐只能通过用量额度使用它 | `/model` 选不带 `[1m]` 的版本；或开启 `/usage-credits` 后重启 | [错误参考](https://code.claude.com/docs/en/errors) |
| `API Error: Server is temporarily limiting requests (not your usage limit)` | 服务端短时限流，和你的额度无关 | 稍等再试；持续出现看 status.claude.com | [错误参考](https://code.claude.com/docs/en/errors) |
| `API Error: Request rejected (429)` | 你的 API Key（或 Bedrock / Vertex 项目）的速率上限 | `/status` 确认当前凭据，有多余的 `ANTHROPIC_API_KEY` 先去掉；到服务商后台申请更高档；减少并行子任务或用 `/model` 换小模型 | [错误参考](https://code.claude.com/docs/en/errors) |
| `API Error: Repeated 529 Overloaded errors` | 服务端繁忙，官方说明不占你的额度 | 几分钟后重试，或用 `/model` 换一个模型（容量按模型分别统计）；看 status.claude.com | [错误参考](https://code.claude.com/docs/en/errors) |
| `API Error: 500 Internal server error` | 服务端内部故障，和你的提示、设置、账号无关 | 等一分钟重发（长提示直接输入 `try again`）；看 status.claude.com；持续出现用 `/feedback` 反馈 | [错误参考](https://code.claude.com/docs/en/errors) |
| `Request timed out` / `API Error: No response from API` | 网络慢、代理拖慢，或模型正在生成很长的回复（默认超时 10 分钟） | 重试；网络或代理慢的调大超时：`export API_TIMEOUT_MS=900000` | [错误参考](https://code.claude.com/docs/en/errors) |
| 充了会员还显示 Free Plan，或 Claude Code 让去充 API | 登录了别的邮箱；钱充到了 API 平台（Console）；付款失败被降级 | 退出重新登录、核对邮箱和登录方式；Settings → Billing 看付款状态；API 余额不会变成 Pro；Claude Code 里 `/login` 选订阅账号 | [账单 FAQ](https://support.claude.com/en/articles/8325618-paid-plan-billing-faqs)、[用 Pro / Max 使用 Claude Code](https://support.claude.com/en/articles/11145838-use-claude-code-with-your-pro-or-max-plan) |
| `Autocompact is thrashing: the context refilled to the limit...` | 自动压缩后某个大文件或工具输出立刻又把上下文填满 | 让它分段读大文件；`/compact` 时说明保留什么；大文件任务交给子代理；不需要旧对话就 `/clear` | [运行排错](https://code.claude.com/docs/en/troubleshooting) |
| 卡住不动、占用内存很高、搜索找不到文件 | 上下文太大；内置 ripgrep 在你的系统上跑不起来；WSL 跨文件系统慢 | `/compact` 压缩、重启后 `claude --continue` 接着聊；`claude --safe-mode` 排查插件；装系统 ripgrep 并设 `USE_BUILTIN_RIPGREP=0`；WSL 把项目放到 `/home/` 下 | [运行排错](https://code.claude.com/docs/en/troubleshooting) |

拿不准是哪条：在 Claude Code 里运行 `/doctor` 做自动检查；`claude` 根本起不来就在终端运行 `claude doctor`。账号、账单、订阅类的问题（登录循环、订阅不被识别、组织被停用）官方让联系支持：登录 claude.ai，点左下角头像 → Get help（Console 用户在 platform.claude.com）。

更多（安装、登录、网络与代理）见 [Claude Code 国内使用指南](claude-code.md)。

## Codex CLI 报错

| 情况 | 多半是什么原因 | 怎么办 |
|---|---|---|
| 浏览器授权页打不开或一直转圈 | 网络连不上 OpenAI 的登录服务 | 先确认 chatgpt.com 能正常打开，网络稳定后重试；远程机器用 `codex login --device-auth` |
| 登录后提示要升级套餐 | 登录的账号没有会员，或登录了另一个邮箱 | `codex login status` 查看，`codex logout` 后重新用开了会员的账号登录 |
| 写到一半提示额度用完 | Plus 的 5 小时额度用完了 | 等窗口恢复；用 `/model` 换轻量模型；长期不够考虑购买 credits 或升级 Pro |
| 发现被扣了 API 费用 | 登录时选成了 API Key | `codex logout`，重新选 Sign in with ChatGPT，额度才算进会员 |
| 安装脚本下载失败 | 默认下载地址当前不可用 | 设置 `CODEX_INSTALLER_USE_RELEASES_OPENAI_COM=false` 改从 GitHub Releases 下载，或用 npm、Homebrew 安装 |
| WSL 里编辑器找不到 Codex | WSL 里没装或不在 PATH 里 | 在 WSL 里运行 `which codex`，没有就在 WSL 里重装 |
| WSL 里大仓库很慢 | 仓库放在 `/mnt/c/...` 下 | 把仓库移到 Linux 家目录；再运行 `wsl --update` 和 `wsl --shutdown` |
| 命令行和桌面应用版本不一致 | 两边版本不同 | 分别运行 `codex --version` 对比后升级 |
| 一直在等，没有输出 | 可能在等你确认权限 | 看终端是否停在审批提示上，`/permissions` 查看当前设置 |

更多（安装、登录、多账号切换、credits）见 [Codex CLI 国内使用指南](codex-cli.md)。

## Grok 开通前先确认

Grok 代充最常见的"失败"不是报错，而是账号条件不符：账号已经是付费会员的充不了，要等到期变回免费版再充；提交的是 grok.com Cookie 里的 sso 值，粘贴整段 JSON 或过期的值会被拒。详见 [Grok 代充：什么账号能充、怎么开通](grok-daichong.md)。

## 合集里的其他章节

本文是 [国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集](https://github.com/yaoyao-ai-trainer/yaoyao-ai-trainer.github.io) 的一章，其他章节：

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
- [报错速查表：ChatGPT / Claude / Claude Code / Codex 常见报错](baocuo-sucha.md)
- [全部复测记录（按日期）](fuce-jilu.md)
- [回到合集首页](../README.md)
