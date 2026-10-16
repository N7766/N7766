# N7766 · LLM / Agent

关注 **LLM 后训练、实验评测与 Agent 应用开发**。使用 Python、PyTorch 和 FastAPI，把模型实验与可运行的软件连接起来。

Building reproducible LLM experiments and evidence-grounded agent applications.

## 代表项目

| 项目 | 解决的问题与个人实践 | 展示入口 | 状态 |
| --- | --- | --- | --- |
| **[DPO 推理链压缩](https://github.com/N7766/dpo-cot-compression)** | 构建偏好数据，对比 SFT / DPO 的准确率与输出长度，记录配置和实验边界 | [项目与结果概览](https://github.com/N7766/dpo-cot-compression/blob/main/docs/PORTFOLIO.md) | 已有实验结果；验证集参与检查点选择 |
| **[LabLens 实验分析 Agent](https://github.com/N7766/lablens-agent)** | 工具调用、确定性指标计算、BM25 检索、复合筛选/Pareto、数值与来源检查、通用导入、可核对计划与调用轨迹 | [演示结果](https://github.com/N7766/lablens-agent/blob/main/docs/demo.md) · [评测记录](https://github.com/N7766/lablens-agent/blob/main/docs/v0.11-evaluation.md) | v0.11；可分享的离线证据报告 |
| **[拾题 · QuestionGlass](https://github.com/N7766/QuestionGlass)** | 原生 macOS 刷题进度工具，支持离线存档、撤销和多题库 | [下载 v1.2](https://github.com/N7766/QuestionGlass/releases/tag/v1.2) · [源码与构建](https://github.com/N7766/QuestionGlass#从源码构建) | 已发布 macOS 应用 |

## 当前在做

LabLens v0.11 把可复核结果生成可直接阅读的 HTML / Markdown 报告：导出前校验并重算，完整保留结果、比较方向、资料来源及未处理要求。查询、计划和历史文件均可从工作台导出，命令行也可使用；本轮报告生成不调用模型。

457项工程测试通过；166份历史收据导出两种格式，加22类边界检查，376/376通过。这是离线交付与兼容性验证，不是新增模型成功率。历史错误保留，当前规则无法识别的表达继续标明范围；报告可重算不证明实验来源真实或任务理解正确。

[直接阅读示例报告](https://github.com/N7766/lablens-agent/blob/main/docs/reports/v0.11/README.md) · [验收与边界](https://github.com/N7766/lablens-agent/blob/main/docs/v0.11-evaluation.md) · [三分钟演示](https://github.com/N7766/lablens-agent/blob/main/docs/walkthrough.md)

[查看开发计划与验收条件](https://github.com/N7766/lablens-agent/issues) · [查看版本记录](https://github.com/N7766/lablens-agent/releases)

## 技术实践

- **模型实验：**PyTorch、LoRA、SFT / DPO、数据构建与结果分析。
- **Agent 工程：**Python、FastAPI、Pydantic、Function Calling、BM25、Pytest。
- **应用交付：**SwiftUI / AppKit、本地持久化、应用构建与发布。

每个项目区分已实现、已验证和待完成内容；具体配置、复现方式及局限见对应仓库。
