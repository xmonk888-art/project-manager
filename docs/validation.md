# 验证记录与能力边界 / Validation scope

当前资料对应 **project-manager 1.3.0**。不同版本的证据分别保留；不把文档场景、历史只读复核和本版合成实测混为一项。

## 1.3.0：2026-11-17 合成离线小项目

环境：本机 Windows/Codex；执行项目使用 Python 3.10.22 标准库。一个不继承主对话历史的真实执行助手读取新版技能，接手 CSV 报告工具原型。测试方模拟使用者确认目标，执行助手串行制作、修复和交付，未继续派生员工。

| 核验 | 记录结论 |
| --- | --- |
| 接手位置 | 识别旧完成状态只覆盖 v1 原型，v2 缺交付与验收 |
| 确认前只读 | 7 个初始文件哈希不变，新增文件 0 |
| 固定验收 | 首次 8 项中 7 失败、1 报错；修复后 8/8 通过；两轮绑定不同源码哈希 |
| 保留标准 | 原始要求、说明、对话材料、输入和验收脚本哈希不变 |
| 交付包 | ZIP 解压后的真实运行通过，包与源码一致 |
| 主助手后续独立复核 | 使用新增 21 条 BOM CSV，检查混合状态、重复编号、顺序、转义和晚出现的非法行保护 |
| 浏览器 | 两份报告 × 1440 / 390 宽度，共 4 场景通过；无横向溢出、脚本错误或外部资源请求 |
| 技能静态检查 | 格式、YAML、中文界面说明、引用路径及许可与无关配置完整性通过 |

执行助手交接时未做浏览器视觉检查；上表浏览器结果来自主助手之后的检查，不追写成该执行助手当时已做。一次进度询问后的继续执行可由后续代码、包、复验和交接佐证。

[新案例与脱敏摘要](../cases/goal-driven-trial-20261117/README.md)。这是维护者根据本地记录整理的有限实践证据。公开材料未提供完整可重放实验包，不是第三方认证，也不是效率基准。源码前后比较反映该测试项目修复，不是技能 1.2.0 与 1.3.0 的对照。

## 历史记录

| 时间 / 版本 | 实际工作与边界 |
| --- | --- |
| 2026-11-04 创建前与初版 | 真实资料设计核验、格式、配置和运行文件检查；当时尚未证明协作实跑 |
| 2026-11-05 task-orchestrator 1.0.0 | 真实只读 VI 协作：3 名子助手、13 页 PDF、81 份原文件不变，一次报告哈希补证回查 |
| project-manager 1.2.0 | 格式、配置及失败修复、暂停、阻塞等文档场景；当时尚无本版开发项目执行实测 |

[VI 原案例](../cases/vi-readonly-20261105/README.md)保留更名前名称与版本。只读报告通过不等于设计缺陷已修复，更不证明本版新功能。

## 未验证

真实客户生产项目、1.3.0 多员工并行、另一台电脑、其他宿主或操作系统、真实跨会话中断恢复、长期运行、会话关闭后的自行执行、专业源稿编辑保存重开、印刷及实物打样均未由本次测试覆盖。桌面技能列表刷新、重启后的显示未实测。没有旧版或不用技能的对照，不报告效率提升或总体成功率。

## English

This documentation covers **project-manager 1.3.0**. On 2026-11-17, one real assistant in local Windows/Codex read the new skill and worked on a synthetic offline CSV report project using Python 3.10.22. The tester simulated user approval. The assistant executed serially, without delegating further.

Before approval, all 7 initial file hashes were unchanged and no new files appeared. The fixed 8-check suite initially recorded 7 failures and 1 error; after repair, all 8 passed, bound to a different source hash. Protected requirements and the acceptance script were unchanged. The extracted ZIP ran successfully. The coordinator subsequently reviewed 21 new BOM CSV rows and both reports at widths 1440 and 390: all 4 browser scenarios passed, without overflow, script errors, or external requests. Browser checks occurred after the execution assistant's handoff. Skill format, YAML, references, and unrelated configuration integrity were also checked.

The [public case](../cases/goal-driven-trial-20261117/README.md) is a sanitized maintainer-reported summary, not a replayable benchmark or independent certification. It is not a comparison of skill versions. The [historical VI case](../cases/vi-readonly-20261105/README.md) remains attributed to task-orchestrator 1.0.0 on 2026-11-05; its 3 workers, 13 PDF pages, and 81 unchanged originals do not validate new 1.3.0 behavior.

Real customer production work, multi-worker execution in 1.3.0, other hosts/computers, long runs, actual interruption recovery, automatic work after session closure, and native production-file workflows remain untested. Desktop list refresh/restart was not verified. No controlled efficiency or overall-success-rate claim is supported.
