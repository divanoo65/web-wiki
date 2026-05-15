---
title: Claude Code
type: entity
tags: [AI-Agent, Anthropic, Evaluation]
summary: Claude Code 是由 Anthropic 开发的一种灵活的智能体框架，旨在通过核心原语支持长期运行的智能体构建与迭代。
sources: ["raw/notebooklm-analysis/demystifying-evals-for-ai-agents.md"]
created: 2024-05-22
updated: 2024-05-22
layer: L1
confidence: high
reasoning: 该实体在报告中被明确定义为智能体框架，并作为评估实践的典型案例被引用。
---

# Claude Code

Claude Code 是由 Anthropic 推出的一个灵活的智能体框架（Agent harness/scaffold）。在 AI 智能体开发生态中，它不仅仅是一个单一的模型，而是一个能够处理输入、编排工具调用并返回结果的系统。开发者可以通过 Agent SDK 使用 Claude Code 的核心原语，从而构建出能够执行长期、复杂任务的智能体。

在实际应用中，Claude Code 的演进过程体现了从“直觉驱动”到“评估驱动”的开发范式转变。在项目早期，Claude Code 依赖于内部员工和外部用户的反馈进行快速迭代；随着系统复杂度的提升，团队引入了专门的评估机制。这些评估覆盖了从简洁性、文件编辑等基础能力，到过度工程（over-engineering）等复杂行为的衡量。通过将评估集成到开发流程中，团队能够有效识别性能回归、指导模型改进，并确保在生产环境扩展时系统的稳定性。Claude Code 的实践证明了在智能体开发中，建立一套严谨的评估体系对于区分噪声与真实改进、实现自动化测试至关重要。

### 在本视频中的角色
Claude Code 在视频中被用作“智能体框架”的典型案例。它展示了如何通过评估套件来衡量智能体在特定任务（如文件编辑或行为控制）中的表现，并强调了评估对于长期运行智能体在生产环境中的重要性。

### 相关链接
- [[智能体评估]]
- [[评估套件]]