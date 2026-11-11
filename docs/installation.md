# 获取与安装：Codex、Claude Code、WorkBuddy

三种客户端的安装入口不同。此页依据官方文档整理；本技能现有真实实测仍为本机 Windows/Codex 只读协作，尚未在 Claude Code、WorkBuddy 或另一台电脑实际安装运行。

## 获取单个技能

[下载 project-manager 1.2.0 单技能 ZIP](https://github.com/xmonk888-art/project-manager/releases/download/project-manager-v1.2.0/project-manager-1.2.0.zip) · [版本说明与附件](https://github.com/xmonk888-art/project-manager/releases/tag/project-manager-v1.2.0)

单技能附件只包含 project-manager 及其说明，不必安装整个总库。也可从仓库 `skills/project-manager/` 取得三个运行文件与 LICENSE。GitHub 的“Download ZIP”取得整个总库，WorkBuddy 请使用这里的单技能附件。

## 从单技能 ZIP 安装

把提供的单技能 ZIP 交给支持文件访问的客户端，再发送：

```text
请从我提供的本地 project-manager 单技能 ZIP 安装此技能。先识别当前客户端的官方安装方式：Codex/Claude Code 按实际发现目录处理；WorkBuddy 使用“添加技能 → 上传技能”，无法代操作时告诉我选择哪个包。保留三个运行文件和 LICENSE，检查同名安装，不覆盖自定义内容。完成后报告实际安装位置或导入结果、版本和识别状态；本轮只安装，不执行项目任务。
```

WorkBuddy 自定义包的官方入口是“技能 → 添加技能 → 上传技能”；其对话安装主要面向技能市场。若界面导入必须由用户完成，选择本地单技能 ZIP，随后确认启用。不要仅上传附件就认为已经完成导入。

## 从 GitHub 安装：复制一段话

### Codex

```text
请从 https://github.com/xmonk888-art/project-manager 的 skills/project-manager 目录，只安装 project-manager 到本机 Codex 可发现的个人技能目录。先核对当前版本的路径和已有同名安装；保留 SKILL.md、agents/openai.yaml、references/records-and-handoff.md 和 LICENSE，不覆盖已有自定义内容，不安装其他技能或依赖。完成后报告实际路径、版本和识别结果；需要新会话时说明。本轮只安装，不执行项目任务。
```

当前官方文档列出的个人目录为 `~/.agents/skills/`，项目内为 `.agents/skills/`。已有配置或旧版路径先核对，不自动迁移或增加同名副本。可用 `$project-manager` 明确选择；宿主实际发现结果需要在目标机确认。

### Claude Code

```text
请从 https://github.com/xmonk888-art/project-manager 的 skills/project-manager 目录，只安装 project-manager 到本机 Claude Code 的个人技能目录 ~/.claude/skills/project-manager/。先检查已有同名版本；保留 SKILL.md、agents/openai.yaml、references/records-and-handoff.md 和 LICENSE，不覆盖已有自定义内容，不安装其他技能或依赖。完成后报告路径、版本及 /project-manager 是否可发现；需要新会话时说明。本轮只安装，不执行项目任务。
```

个人技能使用 `~/.claude/skills/`，项目内使用 `.claude/skills/`。在实际 Claude Code 本地会话中确认 `/project-manager`；这不等同于 Cowork 或云会话的安装方式。

### WorkBuddy

下载单技能 ZIP，通过“添加技能 → 上传技能”导入，再发送：

```text
我已通过“添加技能 → 上传技能”导入 project-manager。请确认技能是否已安装并启用，能否读取 SKILL.md 及 references/records-and-handoff.md；报告实际识别结果。若尚未导入，请明确告知，不把附件可读取写成已安装。本轮只检查安装状态，不执行项目任务。
```

没有确认自定义 GitHub 技能可由一句话自动导入的端到端能力，因此当前不承诺同一段话在三个客户端都能全自动安装。也不编造 `.workbuddy/skills/` 路径。

## 最小文件与已有安装

```text
project-manager/
├── SKILL.md
├── agents/openai.yaml
├── references/records-and-handoff.md
└── LICENSE
```

前三项是运行指令与资源；LICENSE 随复制和分发保留。`agents/openai.yaml` 保持中文简短说明，其他宿主未使用该界面文件时也可随包保留。图、案例与 README 供阅读，不是运行依赖。

已有同名目录时先比对内容和版本，保留备份，在暂存目录准备完整新版本后再替换，避免把旧文件残留合并进去。当前没有必要的外部依赖安装脚本；专业制作软件和账号按后续任务另行核对。

## 安装完成后

先核对实际识别，再选择[只读检查](../skills/project-manager/README.zh-CN.md#check)或[执行已授权任务](../skills/project-manager/README.zh-CN.md#execute)。确认安装不等于专业软件齐全或真实派工已通过。

## 官方依据（2026-11-06 核对）

- [Codex：本地技能与发现目录](https://learn.chatgpt.com/docs/build-skills)
- [Claude Code：Skills 与加载位置](https://code.claude.com/docs/en/skills)
- [WorkBuddy：技能、对话安装与上传技能](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market)

[返回总库](../README.zh-CN.md) · [技能说明](../skills/project-manager/README.zh-CN.md) · [使用排查](troubleshooting.md)

## 更新已有安装

升级前保留同名技能的自定义内容，再同步新版运行文件。已打开的对话请重新读取新版 SKILL.md；不能仅凭文件替换推断当前对话已加载新规则。
