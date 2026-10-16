# N7766 · LLM / Agent

关注 **LLM 后训练、实验评测与 Agent 应用开发**。使用 Python、PyTorch 和 FastAPI，把模型实验与可运行的软件连接起来。

Building reproducible LLM experiments and evidence-grounded agent applications.

## 代表项目

| 项目 | 解决的问题与个人实践 | 展示入口 | 状态 |
| --- | --- | --- | --- |
| **[DPO 推理链压缩](https://github.com/N7766/dpo-cot-compression)** | 构建偏好数据，对比 SFT / DPO 的准确率与输出长度，记录配置和实验边界 | [项目与结果概览](https://github.com/N7766/dpo-cot-compression/blob/main/docs/PORTFOLIO.md) | 已有实验结果；验证集参与检查点选择 |
| **[LabLens 实验分析 Agent](https://github.com/N7766/lablens-agent)** | 工具调用、确定性指标计算、BM25 检索、复合筛选/Pareto、数值与来源检查、通用导入、可核对计划与调用轨迹 | [演示结果](https://github.com/N7766/lablens-agent/blob/main/docs/demo.md) · [评测记录](https://github.com/N7766/lablens-agent/blob/main/docs/v0.10-evaluation.md) | v0.10；比较方向与资料步骤核对 |
| **[拾题 · QuestionGlass](https://github.com/N7766/QuestionGlass)** | 原生 macOS 刷题进度工具，支持离线存档、撤销和多题库 | [下载 v1.2](https://github.com/N7766/QuestionGlass/releases/tag/v1.2) · [源码与构建](https://github.com/N7766/QuestionGlass#从源码构建) | 已发布 macOS 应用 |

## 当前在做

LabLens v0.10 新增明确比较方向与资料步骤核对：检查基线/候选是否写反，识别错误操作、遗漏和重复；工作台并列展示原文要求与实际步骤。380项工程测试通过，83份历史结果兼容，可运行离线示例并演示“可重算不等于任务正确”。

在已有DPO真实摘要和Atlas合成快照上编写6道新组合题，两组各重复两次：开关新检查最终均12/12，不宣称自然成功率提升。另将3个人为错误分别交给模型做一次真实替换，3/3通过，作为独立受控修正证据。全部原始输出、首轮失败、费用和冻结源码公开；有限规则与助手非盲复核不是通用语义证明或独立人工审核。

[查看完整真实评测](https://github.com/N7766/lablens-agent/blob/main/docs/v0.10-evaluation.md) · [三分钟演示与代码讲解](https://github.com/N7766/lablens-agent/blob/main/docs/walkthrough.md)

[查看开发计划与验收条件](https://github.com/N7766/lablens-agent/issues) · [查看版本记录](https://github.com/N7766/lablens-agent/releases)

## 技术实践

- **模型实验：**PyTorch、LoRA、SFT / DPO、数据构建与结果分析。
- **Agent 工程：**Python、FastAPI、Pydantic、Function Calling、BM25、Pytest。
- **应用交付：**SwiftUI / AppKit、本地持久化、应用构建与发布。

每个项目区分已实现、已验证和待完成内容；具体配置、复现方式及局限见对应仓库。
