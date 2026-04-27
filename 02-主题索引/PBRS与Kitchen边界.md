# PBRS 与 Kitchen 边界

## 结论

PBRS 不应被写成已验证的第四主贡献。它目前更适合被写成：

- design-and-formalization contribution；
- diagnostic probe；
- Type-II Mode C 的边界案例；
- future work 的直接入口。

## 为什么要降调

Kitchen 实验中 shaped reward 上升到 0.375±0.000，但 true task reward 仍为 0.00±0.00。这说明势函数可能驱动代理优化替代目标，而非完成真实任务。

## 精确表述

Ng PBRS 定理在数学上并不会因为环境 reward 为 0 而失效；更准确的问题是：

> When the environment reward provides no learning signal, the shaped reward can dominate optimization, and practical alignment with the true task objective is no longer guaranteed.

## Phi 定义风险

正文中必须区分：

- object-only Phi：用于 PBRS sensitivity / failure analysis。
- two-phase approach Phi：用于后续 limitation 或改进方向。

不区分会让审稿人误以为论文在同一个符号下切换定义。
