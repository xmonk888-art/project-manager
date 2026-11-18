# 可复制的任务指令

先把技能安装到目标宿主能发现的位置。下列“当前项目”指 Codex 当前打开的实际项目；有多个项目时，换成明确的项目路径。方括号内容由使用者替换，不代表可自动访问任何历史。

调用方式：以下模板以 Codex 的 `$project-manager` 为例。Claude Code 请将开头换成 `/project-manager`；WorkBuddy 请先导入并启用技能，再用“使用项目管家（project-manager）”明确选择。安装方式和实际识别需按各客户端核对，不能把名称写进消息视为已成功加载。

## 1. 只读启动检查

```text
使用 $project-manager，以当前项目为对象，结合当前可读取的对话和项目资料，
判断实际进度及权威版本，区分最终目标、阶段目标、当前任务，列出完成证据、待验收、未开始与阻塞；
提出员工分工、技能调用、能力缺口和验收方案，
输出项目启动单。本轮不修改源文件、不实际派工、不创建或安装技能。
```

预期收到状态恢复、能力核对和分工建议，不应出现“员工已完成”或项目文件被修改的结果。

## 2. 提交计划与执行

新项目可复制这段启动指令。计划确认后再进入执行。

```text
使用 $project-manager，先跟我梳理最终目标、最终交付物、必要通过条件、本次授权阶段与限制，
核对实际进度，并记录目标版本和确认依据，
提出分工、交付物、执行步骤和验收标准。
先给我审阅计划，等我确认后再执行。
```

已有确认计划时，使用以下续作指令。

```text
使用 $project-manager，按已确认的计划完成【具体交付物】。
已确认要求：【要求和完成条件】。
允许操作：【可修改文件或新建成果的范围】。
保留限制：【必须保留的源文件、禁止动作及外部发布限制】。
根据已知对话恢复状态，读取适用的已有专业技能。
有必要且宿主能力和权限允许时委派子助手；否则串行推进并说明。
恢复已确认的最终目标版本和确认依据，把最终交付列为必要验收清单。
每个阶段注明支撑哪项最终验收，阶段结束后继续下一项已授权且依赖已满足的工作。
进度询问先回答再继续；明确改目标、暂停或取消遵从最新指令。
检查失败自动安排范围内修复，并复验原问题和受影响功能。
必要项全部通过后交付；真实阻塞时保留进度、证据和恢复入口，不降低标准。
遇到超出授权的必要动作，先完成可独立推进的工作，再说明具体影响。
```

员工数和技能选择由交付需要决定。使用“团队”这个说法，并不保证宿主提供真实并行执行。

## 3. 继续已有工作

```text
使用 $project-manager，继续当前项目。
先读取项目入口、状态与最新成果，核对最终目标版本、确认依据、阶段与最终验收的对应关系。
旧“完成”只按对应目标与有效证据判断；已有确认有效且未变更时直接沿用。
沿用已确认的计划与仍然有效的授权，从尚未完成的任务继续；不因旧日志写着待办而盲目重跑。
授权或权威输入无法确认时，标明缺口并继续可独立完成的部分。
完成后汇报本次新增成果、复用的检查及仍待处理项。
```

这是一条续作指令，不表示真实中断恢复机制已经经过验证。新聊天必须能读取对应项目记录。

## 4. 换一台电脑接手

```text
使用 $project-manager，接手当前项目交接包。
先核对最终目标版本、确认依据、当前阶段、权威源稿、授权及已有检查，再把项目内相对路径映射到本机。
分别检查调度技能、专业技能、软件工具、字体和账号连接。
按“已可做、需要替代、待补条件”列出结果，在已有授权范围内继续可完成的部分。
缺失能力先评估通用方法能否可靠满足验收，不擅自安装技能、修改软件配置或登录账号。
不要把旧电脑验证通过写成本机验证通过；完成后说明本机实际执行和未验证的范围。
```

需要一并携带项目资料和状态；复制这段话或一个技能文件夹不会带来另一台电脑的全部上下文。

## 5. 遇到缺技能或工具

```text
使用 $project-manager，先评估当前缺少的能力是否影响交付。
已有项目规范和通用工具足够时，继续完成能验证的部分。
不足时调研替代方案，提供原始来源、GitHub Stars 与查询日期、所属仓库和中文对比。
明确替代方法对可编辑性、交付格式和质量的影响。本轮只调研，不安装、不改配置。
```

有 `skill-research` 时可调用它；没有时仍可依据来源核实候选，不把“找到”写成“已安装或实测”。

[返回技能说明](../skills/project-manager/README.zh-CN.md)

## 6. 最小任务示例：从“有原型”到“同事能使用”

以一个 CSV 报告工具为例，目标不只写“修复脚本”，而是“同事能解压离线运行，得到准确 JSON 和可读 HTML；错误输入不得覆盖已有报告”。当前阶段可依次为核对原型、实现修复、打包说明、交付验收；每阶段注明对应的必要条件。此例展示用法，不授权读者环境中的实际制作。

在确认目标前，只读核对原型与旧状态，提交目标确认单。确认后在允许范围内制作和检查。HTML 成功不代表 ZIP 已能运行；只有本次必要项齐全并通过才报告范围内验收通过。若本次只授权调研，就交付调研，不自动进入制作。

本版一次合成离线实测见[案例](../cases/goal-driven-trial-20261117/README.md)。没有跨电脑、长期运行或关闭会话后自行恢复的验证。

## English: goal-led start and continuation

For a new project, assess actual progress and submit a goal record and plan first. Include the user-usable result, final deliverables, required pass conditions, authorized stages, exclusions, goal version, and confirmation evidence. Existing valid approval should be reused without repeated confirmation.

```text
Use $project-manager to recover this project's confirmed final goal and scope.
Compare actual outputs with the goal version and acceptance evidence; do not
inherit an old completion claim without checking what it covered.
Map each stage and current task to required final acceptance checks.
Continue authorized work whose dependencies are ready. Answer progress questions,
then resume. Repair and recheck failures without lowering the criteria.
Follow explicit goal changes, pause, or cancellation. Record real blockers and
recovery conditions; report completion only for the verified authorized scope.
```

A minimal example is a CSV report tool: the final result is a ZIP a colleague can extract and run offline to obtain accurate JSON and readable HTML, with invalid input preserving existing reports. Implementing the script alone does not establish final delivery. If only assessment is authorized, stop at its agreed deliverable.

Codex uses `$project-manager`; Claude Code uses `/project-manager`; WorkBuddy requires import and activation first, followed by an explicit request to use project-manager. These invocation notes do not establish cross-client test coverage. [Trial evidence](../cases/goal-driven-trial-20261117/README.md) · [Validation boundaries](validation.md)
