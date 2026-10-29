# Claude Code 国内使用指南：安装、登录、Pro / Max 额度怎么选、常见报错（摘要）

> 本页是《国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集》里的一章摘要（[合集首页](../README.md) · [全部章节](../README.md#目录)）。**完整正文在原仓库：[haiwaihuyonghui-rgb/claude-code-guide-cn](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn)**，内容、价格和复测记录都以原仓库为准。

> **立场说明：** 整理：瑶瑶ai训练师。作者自己经营一家 AI 会员代充商城（kw.yaoyao.chat），所以本文不是第三方评测；作者商城的价格、开通流程和售后统一放在 [作者商城商品说明](shangcheng.md)。与 OpenAI、Anthropic、Google、xAI 没有隶属关系，也没有授权，品牌名仅用于说明。

正本是 Claude Code 的中文使用说明，按 Anthropic 官方文档整理安装、登录、Pro / Max 额度怎么选和常见报错，每条附官方链接。它是 Anthropic 出的、在终端里读写代码的编程工具，本身不另收费：Pro、Max、Team、Enterprise 订阅都包含，也可以用 Console 的 API Key 按量计费；免费版 claude.ai 不含。

[安装](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#安装)：官方推荐原生安装脚本（macOS / Linux / WSL 用 curl，Windows 用 PowerShell 的 irm，装好会在后台自动更新），另有 Homebrew、WinGet 和 npm 三种方式，npm 要 Node.js 22 以上、不要加 sudo。装完新开一个终端，用 `claude --version` 和 `claude doctor` 检查。[登录](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#登录)时首次运行 `claude` 会打开浏览器，WSL、SSH 这类环境可以把浏览器给出的登录码粘回终端。要特别注意：环境变量里如果有 `ANTHROPIC_API_KEY`，它会优先按 API 计费，可以用 `/status` 确认当前走的是订阅还是 API。

[额度](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#pro-和-max-额度怎么选)（2026-10-17 核对）：Pro 每月 20 美元（年付折合 17），Max 5x、Max 20x 每月 100、200 美元，额度分别是 Pro 的 5 倍和 20 倍。额度按滚动 5 小时窗口加每周上限计算，网页、手机、编辑器插件和 Claude Code 共用一份；`/usage` 可以看用量和重置时间，用完可以等重置、升档，或开启按 API 价计费的用量额度。Max 附带的每月 API credits 不能在 Claude Code 里当额度用。

正本的[报错表](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn#报错--常见问题大全)有二十多条，覆盖 `command not found`、安装脚本返回网页（含 `App unavailable in region`）、TLS 证书、登录码无效、403、旧 API Key 导致"组织已停用"、`Credit balance is too low`、各种 limit 提示、529 / 500 / 超时等，并给出官方出处；拿不准是哪条时，先在 Claude Code 里运行 `/doctor` 自动检查。上手部分给了三个习惯：项目先交给 git 管理，出错可以回滚；开工前跑一次 `/init` 生成项目说明；每个任务单开一个对话，结束就 `/clear`，因为对话拉得越长越费额度。另有网络与代理设置（只支持标准代理变量、不支持 SOCKS）、多账号用 `CLAUDE_CONFIG_DIR` 分开配置目录的方法，以及和 Codex 怎么取舍。

**看完整版：** [haiwaihuyonghui-rgb/claude-code-guide-cn](https://github.com/haiwaihuyonghui-rgb/claude-code-guide-cn)

## 合集里的其他章节

谷歌站版攻略（同一作者整理，手机上看更方便；[全部 15 页入口](../README.md#谷歌站版攻略)）：

- [Claude 充值订阅教程：Pro / Max 5x / Max 20x 国内代充怎么开](https://sites.google.com/view/yaoyao-ai/claude)
- [Claude 注册教程：国内怎么注册账号、收不到验证码怎么办](https://sites.google.com/view/yaoyao-ai/claude-zhuce)

本文是 [国内 ChatGPT / Claude / Grok / Gemini 充值代充教程合集](https://github.com/yaoyao-chat/yaoyao-chat.github.io) 的一章，其他章节（每章是摘要，完整正文在各自的原仓库）：

- [ChatGPT Plus 国内怎么开通：官方订阅、应用内购、礼品卡、代充四种方法怎么选](chatgpt-plus.md)
- [没有信用卡怎么开通 ChatGPT Plus：支付宝 / 微信能不能付、礼品卡、应用内购、代充](chatgpt-plus-wu-xinyongka.md)
- [ChatGPT Pro 100 美金档位国内怎么买：Pro 100 / 200 / 500 三档区别、和 Plus 差在哪](chatgpt-pro-100.md)
- [ChatGPT / Claude / Gemini / Grok 会员价格对比：四家官方价、约合人民币、代充价怎么算账](jiage-duibi.md)
- [Claude Pro / Max 国内怎么开通：官方订阅、应用内购、赠送订阅、代充四种方法怎么选](claude-daichong.md)
- [Claude 充值平台怎么选：Pro / Max 怎么选、充值后显示 Free Plan 排查、防封习惯](claude-chongzhi.md)
- [Claude 代充靠谱吗：代充原理、要交出什么信息、风险在哪](claude-kaopu-yuanli.md)
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
