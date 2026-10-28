# 来源与许可

[返回学习目录](README.md)

本仓库的中文学习笔记、译文、教学示例与原始论文／数据分开标示。论文报告的结果仍归属于原作者；笔记中的整理与推导不表示原作者认可，也不表示已独立复现。

## HealthBench

### 论文与官方实现

- [HealthBench 论文 PDF](https://cdn.openai.com/pdf/bd7a39d5-9e9f-47b3-903c-8b847ca650c7/healthbench_paper.pdf)
- [OpenAI simple-evals](https://github.com/openai/simple-evals)
- [官方评测列表及许可说明](https://github.com/openai/simple-evals#evals)
- [官方 healthbench_eval.py](https://github.com/openai/simple-evals/blob/main/healthbench_eval.py)

### 本仓库包含的材料

| 材料 | 来源与处理 |
|---|---|
| `assets/healthbench/examples-42.json` | 从 [2025-05-07 固定版本题库](https://openaipublic.blob.core.windows.net/simple-evals/healthbench/2025-05-07-06-14-12_oss_eval.jsonl) 选择 42 道题；保留原始题目 ID、消息、rubric、权重、标签及 canary |
| `assets/healthbench/question-bank.html` | 使用上述样题制作的离线阅读页面，包含中文辅助讲解；原始英文数据保留 |
| `notes/healthbench/04-real-examples.md` | 从 42 道样题中选出 9 道，展开原文、评分条目和中文讲解 |
| `assets/healthbench/grader-code-excerpt.md` | 2026-10-28 获取的官方代码第 1–220 行，含评分器模板与分数计算函数；文件内记录来源和 blob SHA。这不是对论文发表时实现版本的认定 |

官方仓库将 HealthBench 列为 **MIT License**。本仓库保留 [完整 MIT 许可及版权声明](third-party/healthbench/LICENSE)；该许可适用于相应第三方材料，不自动作为本仓库全部原创笔记的许可。

论文另提出：为避免评测数据进入训练语料或被联网模型检索，希望读者不要在网上展示具体样例。此处如实记录这一评测使用请求，并保留原数据中的识别标记；它与 MIT 的再分发许可是不同层面的说明。

原题或 rubric 存在歧义时，笔记在原文旁标注问题，不悄悄改写原始数据。中文翻译仅辅助阅读，以原始英文和源文件为准。

## SECL

- **题目：** Self-Calibrating Language Models via Test-Time Discriminative Distillation
- **论文条目：** [arXiv:2604.09624](https://arxiv.org/abs/2604.09624)
- **本次阅读版本：** [arXiv:2604.09624v1，25 页](https://arxiv.org/pdf/2604.09624v1)
- **对应笔记：** [论文概览](notes/secl/overview.md)、[实验流程与术语](notes/secl/study-notes.md)

笔记里的页码均指向上述 v1 版本；公式差异、未核实的实现细节和论文结果的限制均在正文保留。仓库不存放论文 PDF，也不包含独立复现实验结果。
