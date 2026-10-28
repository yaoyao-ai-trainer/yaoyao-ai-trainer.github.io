# OpenAI Codex CLI 国内使用指南：安装、ChatGPT 账号登录、多账号切换、Plus / Pro 额度、常见报错（摘要）

> 本页是《国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集》里的一章摘要（[合集首页](../README.md) · [全部章节](../README.md#目录)）。**完整正文在原仓库：[haiwaihuyonghui-rgb/codex-cli-guide-cn](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn)**，内容、价格和复测记录都以原仓库为准。

> **立场说明：** 整理：瑶瑶ai训练师。作者自己经营一家 AI 会员代充商城（kw.yaoyao.chat），所以本文不是第三方评测；作者商城的价格、开通流程和售后统一放在 [作者商城商品说明](shangcheng.md)。与 OpenAI、Anthropic、Google、xAI 没有隶属关系，也没有授权，品牌名仅用于说明。

正本整理 OpenAI Codex CLI 的安装、登录、多账号切换、额度和报错。Codex CLI 是 OpenAI 官方开源、在终端里运行的编程助手，资料来自 openai/codex 仓库 README 和 OpenAI 官方的认证、环境变量、定价文档（2026-10-13～10-16 核对）。Codex 不单卖，额度随 ChatGPT 订阅附带：Plus、Pro、Business、Edu、Enterprise 都包含，命令行、编辑器插件、桌面应用和网页版共用同一份额度。

[安装](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#安装)有官方脚本（macOS / Linux、Windows PowerShell 各一条）、npm、Homebrew 和 GitHub Releases 压缩包几种；默认下载地址不通时，官方给了一个改从 GitHub Releases 下载的环境变量。Windows 可以原生运行，也可以装在 WSL2 里（WSL1 已不再支持），仓库建议放在 Linux 家目录下。[登录](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#用-chatgpt-账号登录)时选 Sign in with ChatGPT，用量才算进会员；用 API Key 登录则按标准 API 价另计。

[额度](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#plus-和-pro-的额度差别)：Plus 每月 20 美元，按每 5 小时估算——官方给的是按模型划分的消息条数区间，不是固定上限，另外可能还有每周限制；Pro 100 / 200 / 500 美元目前没有 5 小时限制。用到上限可以另买 credits，官方说明先扣套餐自带额度、再扣 credits，当前价格以 ChatGPT 里显示的为准；如果每周都要额外买，正本建议算一算是不是直接升 Pro 更划算。

[多账号](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#多账号切换官方方法)方面，官方没有切换按钮：偶尔换号用 `codex logout` 再 `codex login`，经常换号用 `CODEX_HOME` 给每个账号一个独立目录。`auth.json` 里存着访问令牌，要像密码一样保管；网上的第三方"账号切换器"不是官方软件，专门注册多个账号轮流躲额度也可能违反条款。正本最后有 [9 条常见报错](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn#常见报错与解决)（登录后提示升级、被扣了 API 费、安装脚本下载失败、WSL 里很慢等）和与 Claude Code 怎么选。

**看完整版：** [haiwaihuyonghui-rgb/codex-cli-guide-cn](https://github.com/haiwaihuyonghui-rgb/codex-cli-guide-cn)

## 合集里的其他章节

谷歌站版攻略（同一作者整理，手机上看更方便；[全部 15 页入口](../README.md#谷歌站版攻略)）：

- [ChatGPT 注册教程：国内怎么注册账号、App 下载和常见问题](https://sites.google.com/view/yaoyao-ai/chatgpt-zhuce)
- [ChatGPT Plus 购买指南：没有账号怎么买、成品号和代充的区别、Plus 与 Pro 怎么选](https://sites.google.com/view/yaoyao-ai/chatgpt)

本文是 [国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集](https://github.com/yaoyao-ai-trainer/yaoyao-ai-trainer.github.io) 的一章，其他章节（每章是摘要，完整正文在各自的原仓库）：

- [ChatGPT Plus 国内怎么开通：官方订阅、应用内购、礼品卡、代充四种方法怎么选](chatgpt-plus.md)
- [没有信用卡怎么开通 ChatGPT Plus：支付宝 / 微信能不能付、礼品卡、应用内购、代充](chatgpt-plus-wu-xinyongka.md)
- [ChatGPT Pro 100 美金档位国内怎么买：Pro 100 / 200 / 500 三档区别、和 Plus 差在哪](chatgpt-pro-100.md)
- [ChatGPT / Claude / Gemini / Grok 会员价格对比：四家官方价、约合人民币、代充价怎么算账](jiage-duibi.md)
- [Claude Pro / Max 国内怎么开通：官方订阅、应用内购、赠送订阅、代充四种方法怎么选](claude-daichong.md)
- [Claude 充值平台怎么选：Pro / Max 怎么选、充值后显示 Free Plan 排查、防封习惯](claude-chongzhi.md)
- [Claude 代充靠谱吗：代充原理、要交出什么信息、风险在哪](claude-kaopu-yuanli.md)
- [Claude Code 国内使用指南：安装、登录、Pro / Max 额度怎么选、常见报错](claude-code.md)
- [Grok Premium（原 SuperGrok）国内怎么买：官方四档价格、三合一说明、四种开通方法](grok-premium.md)
- [Grok 代充：什么账号能充、怎么开通、靠谱吗](grok-daichong.md)
- [Gemini Pro（Google AI Pro）国内代充：怎么开通、开通后怎么确认生效、常见问题](gemini-pro.md)
- [AI 会员订阅国内指南：ChatGPT / Claude / Gemini / Grok 开通路线对比、代充判断 8 条](ai-subscription.md)
- [常见问题详细版：能不能用、代充、档位](faq-xiangxi.md)
- [作者商城商品说明：全部商品价格、开通流程、售后](shangcheng.md)
- [报错速查表：ChatGPT / Claude / Claude Code / Codex 常见报错去哪看](baocuo-sucha.md)
- [全部复测记录（按日期）](fuce-jilu.md)
- [回到合集首页](../README.md)
