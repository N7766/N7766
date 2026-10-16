# N7766 · LLM / Agent

关注 **LLM 后训练、实验评测与 Agent 应用开发**。使用 Python、PyTorch 和 FastAPI，把模型实验与可运行的软件连接起来。

Building reproducible LLM experiments and evidence-grounded agent applications.

## 代表项目

| 项目 | 解决的问题与个人实践 | 展示入口 | 状态 |
| --- | --- | --- | --- |
| **[DPO 推理链压缩](https://github.com/N7766/dpo-cot-compression)** | 构建偏好数据，对比 SFT / DPO 的准确率与输出长度，记录配置和实验边界 | [项目与结果概览](https://github.com/N7766/dpo-cot-compression/blob/main/docs/PORTFOLIO.md) | 已有实验结果；验证集参与检查点选择 |
| **[LabLens 实验分析 Agent](https://github.com/N7766/lablens-agent)** | 工具调用、确定性指标计算、BM25 检索、复合筛选/Pareto、数值与来源检查、通用导入、可核对计划与调用轨迹 | [演示结果](https://github.com/N7766/lablens-agent/blob/main/docs/demo.md) · [评测记录](https://github.com/N7766/lablens-agent/blob/main/docs/v0.6-evaluation.md) | v0.6；显式规划、分句核对与有界修正 |
| **[拾题 · QuestionGlass](https://github.com/N7766/QuestionGlass)** | 原生 macOS 刷题进度工具，支持离线存档、撤销和多题库 | [下载 v1.2](https://github.com/N7766/QuestionGlass/releases/tag/v1.2) · [源码与构建](https://github.com/N7766/QuestionGlass#从源码构建) | 已发布 macOS 应用 |

## 当前在做

LabLens v0.6 已交付显式动作规划：排序、极值、top-k与并列选项明确编译；原问题逐句关联、最多一次本地校验修正、可编辑预览与结果离线重算。159项工程测试通过，Python3.11/3.13 CI、安装包与浏览器流程已验证。

新4道组合题三组各重复2次：旧单次规划0/8完整任务，新单次7/8，新两次预算6/8；全部24条都只调用一次，没有触发修正，不能据此声称修正收益。保留错误Pareto截断、完整源文件快照、原始轨迹和费用；这是同一快照的小样本助手评分，无独立人工审核，不作通用Agent成功率。

[查看完整真实评测](https://github.com/N7766/lablens-agent/blob/main/docs/v0.6-evaluation.md) · [三分钟演示与代码讲解](https://github.com/N7766/lablens-agent/blob/main/docs/walkthrough.md)

[查看开发计划与验收条件](https://github.com/N7766/lablens-agent/issues) · [查看版本记录](https://github.com/N7766/lablens-agent/releases)

## 技术实践

- **模型实验：**PyTorch、LoRA、SFT / DPO、数据构建与结果分析。
- **Agent 工程：**Python、FastAPI、Pydantic、Function Calling、BM25、Pytest。
- **应用交付：**SwiftUI / AppKit、本地持久化、应用构建与发布。

每个项目区分已实现、已验证和待完成内容；具体配置、复现方式及局限见对应仓库。
