# 安装项目管家 v1.3.0 / Install project-manager v1.3.0

[下载单技能 ZIP](https://github.com/xmonk888-art/project-manager/releases/download/project-manager-v1.3.0/project-manager-1.3.0.zip) · [完整更新说明](https://github.com/xmonk888-art/project-manager/releases/tag/project-manager-v1.3.0) · [固定版本源码](https://github.com/xmonk888-art/project-manager/tree/project-manager-v1.3.0/skills/project-manager)

## Codex：复制一段话安装

```text
请从 https://github.com/xmonk888-art/project-manager/tree/project-manager-v1.3.0/skills/project-manager 安装项目管家 project-manager v1.3.0。Codex 请使用 skill-installer；其他客户端先核对实际支持的安装方式。只安装此技能，先检查并备份已有同名技能，保留自定义内容。核对 SKILL.md 版本为 1.3.0，保留运行资源和 MIT LICENSE，保持 agents/openai.yaml 的准确中文说明。安装后报告实际路径、版本、技能识别结果和刷新要求；只做只读调用检查，不启动实际项目，不安装其他依赖。
```

可用的 skill-installer 支持 GitHub URL，固定到 `project-manager-v1.3.0` 标签，目录为 `skills/project-manager`。按目标机实际配置确认技能目录；已有同名目录先备份并保留自定义内容，完整替换后核对版本。不要创建多个同名副本。安装后使用 `$project-manager`，并核对实际识别结果；当前会话必要时重新读取技能，刷新或重启是否必要以目标客户端为准。

## Claude Code

复制上面的 GitHub 安装指令，要求使用当前客户端支持的个人技能目录，检查已有安装并核对版本。安装后确认 `/project-manager` 可发现。也可以把下载的 ZIP 交给支持文件访问的本地助手安装；具体目录和加载方式以当前客户端的官方规则为准。

## WorkBuddy

下载上方 ZIP，沿用此前核对的“技能 → 添加技能 → 上传技能”方式导入并确认启用。上传附件不等于完成技能导入；目前没有本版一句话从自定义 GitHub URL 自动安装的实测证据。不要推测安装目录。

## 从 ZIP 安装与检查

解压后顶层目录为 `project-manager/`。保留 `SKILL.md`、`agents/openai.yaml`、`references/records-and-handoff.md` 及 MIT `LICENSE`。包内中文 `README.md`、英文 `README.en.md`、配图和案例均可独立阅读。只有运行指令与必要引用是运行资源；图与案例供阅读。

安装后先检查版本 **1.3.0**、文件完整性、中文界面说明以及客户端真实发现结果，再进行只读调用检查。确认安装不代表专业软件、账号和真实派工已配置齐全。

## 验证范围与依据

v1.3.0 有本机 Windows/Codex 合成小项目执行记录。其他客户端、第二台电脑和桌面技能列表刷新/重启显示尚未实测。安装目标机应重新检查当前环境。

Codex GitHub URL 安装语法已与本机 `skill-installer` 说明核对（2026-11-18）；其他客户端沿用 2026-11-06 的官方依据，本轮未重新验证。

- [Codex 技能说明](https://learn.chatgpt.com/docs/build-skills)
- [Claude Code Skills](https://code.claude.com/docs/en/skills)
- [WorkBuddy 技能](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Skills-Market)

[返回中文首页](../README.zh-CN.md) · [技能说明](../skills/project-manager/README.zh-CN.md) · [安装排查](troubleshooting.md)

## English: copy into Codex or a supported local client

```text
Install only project-manager v1.3.0 from https://github.com/xmonk888-art/project-manager/tree/project-manager-v1.3.0/skills/project-manager. In Codex, use skill-installer; in other clients, verify the supported installation method first. Inspect and back up any existing installation and preserve customizations. Verify SKILL.md declares 1.3.0, retain runtime resources and MIT LICENSE, and keep the accurate Chinese interface description. Report the actual path, version, discovery result, and refresh requirements. Perform only a read-only invocation check; do not start a project or install other dependencies.
```

The pinned GitHub URL identifies tag `project-manager-v1.3.0` and path `skills/project-manager`. Codex skill-installer supports this URL syntax; confirm the target machine's actual configuration. In Claude Code, use its supported skill directory and confirm discovery. WorkBuddy uses its existing Skills → Add skill → Upload skill guidance with the ZIP; automatic custom-URL installation has not been tested.

Preserve all runtime resources and MIT LICENSE. Back up an existing installation, retain customizations, verify version 1.3.0 and discovery, and perform a read-only invocation check. Runtime behavior in other clients/computers and desktop refresh/restart remain untested. The Codex installer syntax was checked against the local installer instructions on 2026-11-18; the other-client guidance retains official sources checked on 2026-11-06.
