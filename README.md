# 量潮飞书适配（quanttide-feishu）

量潮第二大脑适配轴（adapters/）的飞书适配仓库。

## 定位

把 `domains/` 的领域知识转换成飞书可消费的形态：负责协议转换、格式映射与接口包装，不生产领域事实，只做接通。

- 上游：`domains/` 领域知识
- 下游：飞书

## 结构

| 路径 | 仓库 | 说明 |
|:--|:--|:--|
| `apps/qtcloud-feishu` | [qtcloud-feishu](https://github.com/quanttide/qtcloud-feishu) | 飞书适配的可部署应用 |
| `apps/qtadmin` | [qtadmin](https://github.com/quanttide/qtadmin) | 量潮管理后台 |
| `data/context` | [quanttide-context-of-feishu-platform](https://github.com/quanttide/quanttide-context-of-feishu-platform) | 语境：素材与未定稿的整理内容 |
| `data/intention` | [quanttide-intention-of-feishu-platform](https://github.com/quanttide/quanttide-intention-of-feishu-platform) | 意图：为什么做、做成什么形态 |
| `data/roadmap` | [quanttide-roadmap-of-feishu-platform](https://github.com/quanttide/quanttide-roadmap-of-feishu-platform) | 路线图：阶段目标与演进路径 |
| `data/insight` | [quanttide-insight-of-feishu-platform](https://github.com/quanttide/quanttide-insight-of-feishu-platform) | 洞察：实践沉淀的判断与结论 |
| `data/report` | [quanttide-report-of-feishu-platform](https://github.com/quanttide/quanttide-report-of-feishu-platform) | 报告：工作与研究的报告与复盘 |
| `docs/bylaw` | [quanttide-bylaw-of-feishu-platform](https://github.com/quanttide/quanttide-bylaw-of-feishu-platform) | 飞书平台章程 |
| `docs/gallery` | [quanttide-gallery-of-feishu-platform](https://github.com/quanttide/quanttide-gallery-of-feishu-platform) | 案例集：实践案例与成果展示 |
| `docs/handbook` | [quanttide-handbook-of-feishu-platform](https://github.com/quanttide/quanttide-handbook-of-feishu-platform) | 手册：操作规范与做法 |
| `docs/tutorial` | [quanttide-tutorial-of-feishu-platform](https://github.com/quanttide/quanttide-tutorial-of-feishu-platform) | 飞书平台教程 |
| `examples/quanttide-feishu-lab` | [quanttide-feishu-lab](https://github.com/quanttide/quanttide-feishu-lab) | 实验室：骨架（功能正本在 `apps/qtcloud-feishu`） |
| `packages/quanttide-feishu-toolkit` | [quanttide-feishu-toolkit](https://github.com/quanttide/quanttide-feishu-toolkit) | 共享工具包 |

## 许可

[CC BY 4.0](LICENSE)
