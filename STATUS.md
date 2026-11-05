# STATUS

仓库当前快照，供 Agent 与协作者快速了解各 scope 的现状。快照有时效，以最新提交为准。

> 快照日期：2026-10-29
> 最新主仓 commit：f7ba3e3

## 仓库形态

适配轴的飞书适配仓：把 `domains/` 的领域知识转换成飞书可消费的形态，不生产领域事实，只做接通。共 14 个子模块（apps 3、data 5、docs 4、examples 1、packages 1），明细见 [README.md](./README.md)。

## apps/ — 应用

### qtcloud-feishu（飞书适配 CLI，正本）

- Rust CLI（crate `qtcloud-feishu-cli`，命令 `qtcloud-feishu`）；`main.rs` 是骨架，**命令面尚未定义**。
- 骨架已成形：六个资源、十四个动作，登记即契约。基础单元按资源分文件（`src/resources/`），串联器读定义（`engine.rs`），执行器读流程推格（`flow.rs`），落盘按加工后的缓存加游标（`store.rs`，原始响应禁止落盘），路径按 XDG 规范（`paths.rs`）。
- 测试集中在 `tests/`（含假 lark-cli 与夹具），`src/` 只放实现。
- 下一步：按迁入指南接入 qtcloud-connect 的五项飞书能力（聊天记录搜索、群通知、邮件投递统计、邮件发送通道、聊天知识提取），迁入后为七资源十九动作。方案在 `src/cli/docs/dev-guide/`。

### qtcloud-connect（共识连接器）

- 飞书能力退出中：v0.1.x 冻结并标记废弃，v0.2.0 起分批删除；只删本仓重复实现的平台层，共识、Provider、Studio 保留。计划见其 `docs/dev-guide/feishu-removal.md`。

### qtadmin（管理后台）

- 独立演进；ROADMAP 已降级为 `docs/dev-guide/roadmap.md`（2026-10-21）。

## data/ — 陈述性记忆

| 仓 | 负责 | 现状 |
|----|------|------|
| `intention` | 为什么做、做成什么形态 | 已整理为结构化文档，含分层定义（2026-10-15） |
| `context` | 语境：素材与未定稿 | 增补成员职务与任职信息接口说明（2026-10-16） |
| `roadmap` | 阶段目标与演进路径 | 首条主线：通过飞书连接器打通招聘流程 |
| `insight` | 洞察：判断与结论 | 刚起步（2026-10-12 initial） |
| `report` | 报告与复盘 | 刚起步（2026-10-14 初始化） |

## docs/ — 程序性记忆

| 仓 | 负责 | 现状 |
|----|------|------|
| `bylaw` | 飞书平台章程 | 三章六条，未定范围移入 TODO（2026-10-16） |
| `gallery` | 案例集 | 已发布 v0.1.1（2026-10-19） |
| `handbook` | 手册：操作规范与做法 | 待办入口已清理，统一收敛（2026-10-19） |
| `tutorial` | 教程 | 自然淘汰一节并入总章程（2026-10-16） |

## examples/ — 实验室

- `quanttide-feishu-lab`：已收为骨架，与平台仓重复的功能已删除，正本在 `apps/qtcloud-feishu`（2026-10-14）。

## packages/ — 标准库

- `quanttide-feishu-toolkit`：共享工具包；表述已统一为「标准库」（2026-10-23）。
