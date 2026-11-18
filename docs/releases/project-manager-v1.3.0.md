# project-manager v1.3.0 · 围绕最终目标推进 / Coordinate around the final goal

**正式版本：v1.3.0 · 2026-11-18。**

[下载 1.3.0 单技能 ZIP](https://github.com/xmonk888-art/project-manager/releases/download/project-manager-v1.3.0/project-manager-1.3.0.zip) · [中文首页](../../README.zh-CN.md) · [English home](../../README.md)

## 本版变化

接手一个标记“完成”的原型时，先核实这个结论对应哪个目标、产物和验收依据；如果最终目标需要可交付的完整结果，原型完成不能代替项目完成。

- **先判断进度。** 区分已完成且有证据、已制作待验收、未开始和阻塞。没有依据的旧结论标为待核实，不按聊天长度或文件数猜百分比。
- **确认最终目标。** 分清最终目标、阶段目标和当前任务，记录用户可用结果、最终交付、必要通过条件、授权阶段、目标版本和确认依据。有效既有确认直接沿用。
- **每阶段对照最终验收。** 派工和阶段交接注明对应的最终交付与验收项；继续依赖已满足的已授权必要工作，避免只交中间结果就结束。
- **目标稳定，方法可调整。** 在授权内调整顺序、工具和修复路线。问进度后继续；明确改目标、暂停或取消按新指令处理，并保留变更依据。
- **补全续作记录。** 同一权威状态保留目标版本、确认依据、本次范围和阶段映射，供下一次接手核对。

1.2.0 已有的必要验收清单、失败修复、修复后复验、真实阻塞与恢复条件继续保留。新项目及实质变更仍先提交计划确认。Skill 不提供后台常驻执行器；“持续”限定于宿主实际能执行的会话与授权。

## 附件与安装

附件：`project-manager-1.3.0.zip`，供安装单个技能；可阅读资料随包提供。运行资源为 `SKILL.md`、`agents/openai.yaml`、`references/records-and-handoff.md`，分发保留 MIT `LICENSE`。

从固定版本 GitHub 地址安装，或使用本版 ZIP。按[安装说明](../installation.md)核对包内版本、已有自定义内容、实际安装目录和宿主识别。本次发布未修改日常安装环境。Claude Code、WorkBuddy 及跨电脑说明不代表本版已在这些环境实测。

## 验证与边界

2026-11-17，本机 Windows/Codex 运行了一个合成离线 CSV 报告小项目。测试方模拟使用者确认目标，一个执行助手串行完成制作和交接，没有再派生员工。

确认前 7 文件哈希不变、新增 0；固定 8 项验收首次 7 失败、1 报错，修复后 8/8 通过，绑定不同源码哈希；ZIP 解压后实际运行通过。主助手另用 21 条 BOM CSV 复核，随后检查两份报告的 1440 / 390 宽度，共 4 浏览器场景通过。原始要求及验收脚本保持不变。技能格式、YAML、引用和无关配置完整性检查通过；桌面列表刷新及重启显示尚未验证。

[案例与脱敏证据](../../cases/goal-driven-trial-20261117/README.md) · [完整能力边界](../validation.md)

这是维护者提供的有限实测摘要；确认由测试方模拟，无旧版或不用技能的对照，不量化效率，不保证长期持续运行。未验证真实客户生产项目、1.3.0 多员工并行、其他宿主、跨电脑或会话关闭后的自动恢复。公开摘要未包含完整可重放实验包。历史 VI 案例仍归属 2026-11-05 的 task-orchestrator 1.0.0，不为本版新增行为背书。

## 发布地址

- [Release：project-manager-v1.3.0](https://github.com/xmonk888-art/project-manager/releases/tag/project-manager-v1.3.0)
- [单技能 ZIP](https://github.com/xmonk888-art/project-manager/releases/download/project-manager-v1.3.0/project-manager-1.3.0.zip)
- [与 v1.2.0 的完整差异](https://github.com/xmonk888-art/project-manager/compare/project-manager-v1.2.0...project-manager-v1.3.0)

## English release notes

**Version 1.3.0 · Released 2026-11-18.** [Download the standalone ZIP](https://github.com/xmonk888-art/project-manager/releases/download/project-manager-v1.3.0/project-manager-1.3.0.zip).

When taking over a prototype marked complete, first check which goal, outputs, and acceptance evidence that status describes. A completed prototype does not establish completion of a larger delivery goal.

- Assess actual progress: distinguish evidence-backed completion, pending acceptance, unstarted work, and blockers. Mark unsupported old claims as unverified; do not guess percentages.
- Separate the final goal, stage goals, and current tasks. Record the user-usable outcome, deliverables, required pass conditions, authorized stages, goal version, and approval evidence. Reuse valid approval.
- Map every assignment and stage handoff to final delivery and acceptance. Continue ready, authorized necessary work instead of stopping at an intermediate output.
- Adjust methods within scope while retaining the confirmed goal. Answer progress questions and resume; follow explicit goal changes, pause, or cancellation.
- Retain goal version, confirmation evidence, scope, and stage mappings in the existing authoritative state for continuation.

The required-check, repair, recheck, and genuine-blocker handling introduced earlier remains in place. New work and material changes still need plan confirmation. No background runner is included.

The standalone `project-manager-1.3.0.zip` supplies one skill. Preserve its three runtime files and MIT LICENSE. Install from the pinned version on GitHub or use this release ZIP. See [installation guidance](../installation.md). The daily installation was not changed during publication; other-client and cross-computer installation remains untested.

In a synthetic offline CSV report project on local Windows/Codex, one real assistant worked serially after tester-simulated user approval. All 7 initial files remained unchanged before approval. The fixed 8-check suite first had 7 failures and 1 error, then passed 8/8 after repair, with different source hashes. The extracted delivery ZIP ran. A subsequent coordinator review used 21 new BOM CSV rows; both reports passed browser checks at 1440 and 390 widths, totaling 4 scenarios. Protected requirements and the test script were unchanged. Skill format, YAML, references, and unrelated configuration were checked; desktop refresh/restart display was not.

[Case and evidence](../../cases/goal-driven-trial-20261117/README.md) · [Validation scope](../validation.md). This maintainer summary does not supply a complete replayable experiment. There was no skill-version or no-skill control, so it does not quantify efficiency or guarantee long-running execution. Real customer production projects, multi-worker execution in 1.3.0, other hosts/computers, and automatic recovery after session closure remain untested. The historical VI case remains attributed to task-orchestrator 1.0.0 on 2026-11-05.

The GitHub links above identify this release, its standalone ZIP, and the complete changes from v1.2.0.
