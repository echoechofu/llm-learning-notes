# 学习进度

[返回学习目录](README.md)

这里记录已经整理成文的阅读成果。日期表示笔记整理时间，不代表论文实验的执行时间。

## 2026-10-28：第一批公开笔记

### HealthBench

已按三条线重新组织论文：

- [题目生成](notes/healthbench/01-question-generation.md)：医生的职责、情境种子、对话来源、筛选提示词和七个主题。
- [Rubric 构建](notes/healthbench/02-rubric-construction.md)：题目专属规则、共识规则、适用性投票、主题与评价轴。
- [实际评价](notes/healthbench/03-evaluation.md)：逐条判断、正负权重、归一化总分、元评测、Macro F1、worst-at-k 和长度控制。

已整理 [9 道重点题及全部评分条目](notes/healthbench/04-real-examples.md)，并保留 42 道公开样题用于对照。样题记录与源数据核对一致。

阅读时保留的边界：论文没有给出每题固定的评审人数，也没有完整披露每道题的生成履历；示例分数不能当作模型的实测成绩。相关说明已放在对应章节。

### SECL

已整理 [论文概览](notes/secl/overview.md) 和 [按实验流程展开的详细笔记](notes/secl/study-notes.md)：自报置信度、熵触发、冻结教师、干扰答案、NormPTrue、Bin-gate、方向性目标、LoRA，以及指标与消融结果。

已区分回答准确率、置信度校准和正确／错误辨别能力：ECE 改善不代表 AUROC 必然改善。结果表和长数据流反例均保留论文出处。

仍未解决的阅读疑点：NormPTrue 正文与附录的公式不一致；数字 token 的归一化、概率读取和目标梯度处理等实现细节尚未完成源码核验。笔记明确保留这些疑点，尚无独立复现结果。
