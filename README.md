# 论文修改日志

本仓库整理 TC-PPO 论文在 2026-04-16 至 2026-04-27 期间的关键修改记录。

整理原则：

- 保留真实数据、关键决策、论文叙事变化和未完成问题。
- 删除过程性噪声、工具调试流水账、重复的待办和情绪化判断。
- 将日志从“每天发生了什么”重排为“论文如何变清楚、变可信”。

## 快速入口

- [总览](./总览.md)
- [精炼时间线](./01-精炼时间线/)
- [主题索引](./02-主题索引/)
- [下一步行动清单](./03-行动清单/下一步.md)
- [原始日志留档](./00-原始日志/)

## 核心结论

TC-PPO 论文的主线最终应收束为：

> TC-PPO 不是单纯的 performance booster，而是一个 physics-grounded diagnostic framework。FTC 和 Mode A/B/C taxonomy 的价值在于解释何时 PPO 崩溃、何时门控有效、何时门控会误伤或失效。

最值得保留的论文贡献有三类：

1. FTC 指标和两层失效诊断。
2. Adaptive P5/P75 阈值校准与 soft gating。
3. PBRS/Kitchen 作为边界案例和诊断探针，而非未验证的主贡献。

## 当前可信数据锚点

- Mode A 已验证任务：stair, sit-hard, slide, powerlift, cabinet, push, package。
- Slide: TC-PPO 35.3±0.7 vs vanilla 32.2±0.4，+9.6%。
- Powerlift variance: TC-PPO 5.5 vs vanilla 8.3，-33.7%。
- Kitchen PBRS: shaped reward 0.375±0.000，但 true task reward 0.00±0.00。
- Mode B 负例：truck、basketball、insert-normal。

## 仓库状态

这是从 Obsidian TC-PPO 日志中抽取出的精炼版本。`00-原始日志/` 保留原文，其他目录为重新组织后的高信噪比材料。
