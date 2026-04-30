# 2026-04-23 PBRS 尝试与 Mode C 细分

## 精华

这一天的主要产物是 FTC-guided PBRS 和 Type-I/Type-II Mode C 区分。

## 可保留贡献

Mode C 不应被写成单一“安全保证”：

- Type-I Mode C：接触质量天然好，FTC 不低，任务可以学，例如 walk、balance_simple。
- Type-II Mode C：FTC 不低但任务极难或 reward=0，例如 kitchen、maze。

这个区分非常有价值，因为它指出 FTC 的边界：FTC 能诊断接触规律性，但不能凭空提供任务进度信号。

## PBRS 的正确位置

PBRS 可以作为 Type-II Mode C 的探索补丁或诊断探针，但在没有 true reward 成功前，不应被写成已验证的核心算法贡献。
