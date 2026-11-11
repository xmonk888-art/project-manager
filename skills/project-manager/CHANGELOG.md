# project-manager 版本记录

## 1.2.0 · 验收驱动的持续执行 / Acceptance-driven execution

- 将已确认目标转成必要验收清单；可选改进单列，不自行降低标准。
- 阶段汇报后继续推进，检查失败自动安排修复，修复后复验受影响范围。
- 必要项通过、交付齐全才报告范围内完成；真实阻塞或暂停时保留恢复入口。
- 同步中英文介绍、首屏版本摘要、流程配图、使用指令和单技能 ZIP。
- 验证限于格式、配置、文件与文档场景；真实开发项目持续执行和桌面刷新尚未实测。

Required acceptance checks now drive execution, repair assignments, and verification. Progress reports do not end approved work. Deliver when required checks pass; retain recovery state for genuine blockers. Bilingual docs, diagrams, and the standalone package are synchronized. Real development-project execution remains untested.

## 1.1.0 · 先确认计划，再执行

- 新项目先沟通需求并提交计划。用户确认后开始派工、制作与验收。
- 续作沿用已获批计划。范围、交付物或验收标准有实质变化时，重新确认受影响部分。
- 启动简报与交接模板记录计划版本、确认状态和确认依据。
- 同步中英文介绍、桌面及手机配图、安装入口与单技能 ZIP。首发前 VI 只读实测仍按原案例记录。

## 1.0.1 · 文档与配图

- 中英文说明在安装前展示工作看板，实测区使用新版复核摘要。
- 单技能 ZIP 携带说明引用的桌面图、手机图和 SVG 源稿。
- 本次版本更新覆盖文档、配图和版本标识。已有实测仍对应首发前的只读协作记录。

## 1.0.0 · 首发内容

### 已具备

- 从可读取的对话和项目资料恢复目标、阶段、决定与权威版本。
- 按需安排真实子助手或串行职责，选择已有专业技能与工具。
- 管理任务依赖、单一写入负责人、成果交接、证据验收和范围内修复。
- 为续作与跨电脑交接保留状态、版本、依赖和能力缺口。
- 区分讨论、只读与执行，继承当前有效授权及宿主能力限制。

### 验证依据

本地初版创建于 2026-11-04；2026-11-05 完成一次真实 Windows/Codex 只读协作。3 名子助手、13 页 PDF 复核、报告补证回查及 81 份原文件不变的结果见[案例](../../cases/vi-readonly-20261105/README.md)。

### 已知限制

尚未实测第二台电脑、其他宿主、原生制作修订和长期运行；不包含专业制作能力或独立后台服务。许可为 MIT。


## 2026-11-06 · 首次公开发布前更名

`task-orchestrator` 更名为 `project-manager`，中文显示名为“项目管家”；调用、目录、界面说明、文档和分发包同步更新。版本保持 1.0.0，业务规则与交接参考未变。已有实测在旧名下完成，见案例的更名说明。
