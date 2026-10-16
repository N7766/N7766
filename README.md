# N7766 · LLM / Agent

关注 **LLM 后训练、实验评测与 Agent 应用开发**。使用 Python、PyTorch 和 FastAPI，把模型实验与可运行的软件连接起来。

Building reproducible LLM experiments and evidence-grounded agent applications.

## 代表项目

| 项目 | 解决的问题与个人实践 | 展示入口 | 状态 |
| --- | --- | --- | --- |
| **[DPO 推理链压缩](https://github.com/N7766/dpo-cot-compression)** | 构建偏好数据，对比 SFT / DPO 的准确率与输出长度，记录配置和实验边界 | [项目与结果概览](https://github.com/N7766/dpo-cot-compression/blob/main/docs/PORTFOLIO.md) | 已有实验结果；验证集参与检查点选择 |
| **[LabLens 实验分析 Agent](https://github.com/N7766/lablens-agent)** | 工具调用、确定性指标计算、BM25 检索、复合筛选/Pareto、数值与来源检查、通用导入、可核对计划与调用轨迹 | [演示结果](https://github.com/N7766/lablens-agent/blob/main/docs/demo.md) · [评测记录](https://github.com/N7766/lablens-agent/blob/main/docs/v0.7-evaluation.md) | v0.7；有限请求规则与可核对修正 |
| **[拾题 · QuestionGlass](https://github.com/N7766/QuestionGlass)** | 原生 macOS 刷题进度工具，支持离线存档、撤销和多题库 | [下载 v1.2](https://github.com/N7766/QuestionGlass/releases/tag/v1.2) · [源码与构建](https://github.com/N7766/QuestionGlass#从源码构建) | 已发布 macOS 应用 |

## 当前在做

LabLens v0.7 加入有限完整中文查询规则，核对原文的筛选条件、完整集合、排序与并列要求；页面对照实际参数，未知表达明确未核对。209项工程测试通过，兼容25份历史结果文件；浏览器、安装包与Python3.11/3.13 CI已验证。

新6题两组各重复2次：原流程9/12完整任务，加规则流程11/12；本组未触发新增规则反馈，分差不能归因为修正收益。另重放两条错误回复后各真实修正一次：排序错误修正成功，Pareto截断再次被规则拒绝，1/2成功；该事后选择实验不计入新题成绩。全部失败、冻结源码与费用公开，两位助手复核，不是独立人工审核或通用正确率。

[查看完整真实评测](https://github.com/N7766/lablens-agent/blob/main/docs/v0.7-evaluation.md) · [三分钟演示与代码讲解](https://github.com/N7766/lablens-agent/blob/main/docs/walkthrough.md)

[查看开发计划与验收条件](https://github.com/N7766/lablens-agent/issues) · [查看版本记录](https://github.com/N7766/lablens-agent/releases)

## 技术实践

- **模型实验：**PyTorch、LoRA、SFT / DPO、数据构建与结果分析。
- **Agent 工程：**Python、FastAPI、Pydantic、Function Calling、BM25、Pytest。
- **应用交付：**SwiftUI / AppKit、本地持久化、应用构建与发布。

每个项目区分已实现、已验证和待完成内容；具体配置、复现方式及局限见对应仓库。
