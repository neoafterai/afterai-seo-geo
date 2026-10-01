# Execution log

复制到当前客户 `seo-geo/progress.md`。每批追加运行小节，维护最新摘要；不覆盖历史。多人同时修改时先交接，Markdown 不提供自动锁。

## Current checkpoint

记录按需创建，不为单纯查看进度创建新运行或空报告。ID 规则：每次产生新证据／修改时读取已有运行，选择未占用的日期加序号 run-id。同一客户的 T-ID、K-ID、Approval ID 分别递增且不重用；已有任务跨轮沿用。E-ID／R-ID 在运行内唯一，跨文件引用必须带 run-id，例如 `2026-09-22-01:E001`。P-ID 引用同时带问题组版本，例如 `panel-1:P01`；问题变更建立新版本。报告同时给证据相对路径，不能仅写可能重复的 E001。

- Project ID / domain / customer folder:
- Actual private record root / deployment exclusion evidence:
- Skill / rubric / plan / GEO panel versions:
- Last run ID / time / timezone:
- Current stage / active operator or task:
- Stage goal / entry prerequisites / completion criteria:
- Current task-card step / completed evidence / next user action:
- Current live / preview identity:
- Release phase / actual release date and version / included T-IDs / approval / live verification / restore reference:
- Approved scope and approval IDs:
- Next concrete action:
- Blocked items / required user action:

## Run record

为每轮复制此节，标题改为实际 run-id。

| T-ID | State before → after | Actual file / URL / object / field | Before value / diff reference | Approval ID | Verification performed / result | E-ID | Published? / environment | Restore reference |
|---|---|---|---|---|---|---|---|---|

任务完成状态与线上事实分别记录。计划内发布需要验收与批准；共享 Shopify 数据写入成功可能已经影响线上。此时若验收失败，任务状态保持“受阻／已改未验证”，Published? 字段如实写“共享数据已写入线上，验收失败”，不能把它算成完成或一律写“待主题发布”。恢复后另记“原值已恢复，复验结果”，保留初次写入和失败记录。

## Evidence manifest

| E-ID | Kind | Location / source URL | Collected at / method | Actual observation | Limitations | Related task / check |
|---|---|---|---|---|---|---|

证据内容保存在 `evidence/<run-id>/observations.md`；原始截图、导出可另保存在该私有目录。证据位置写可追踪的相对路径。缺文件不能标已核验。

## Resume reconciliation

- 档案身份与实际目标一致吗？
- 进行中的任务是否另有执行者？若有，先交接。
- 文件／后台原值与日志一致吗？若不一致，先检查来源和差异。
- 变更已部署还是仅在预览？是否已经部分写入共享数据？
- 批准覆盖下一动作吗？条件变化需要呈现具体差异。
- 本轮会新增哪些证据和报告？保留旧版。

## Schedule record

| Mode | Scheduler / task ID | Frequency / timezone / first date | Scope | Last actual run / result |
|---|---|---|---|---|

未创建实际任务时 Mode 写“手动”；不填虚构的 scheduler ID。
