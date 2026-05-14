---
title: Anthropic
type: entity
tags:
  - AI公司
  - 科技企业
  - 托管智能体
summary: Anthropic 是一家专注于构建可靠、可解释且可控 AI 系统的研究与安全公司，其开发的 Claude 系列模型在智能体开发与长周期任务处理领域处于行业前沿。
sources:
  - raw/notebooklm-analysis/managed-agents.md
created: 2024-05-22
updated: 2024-05-22
layer: L1
confidence: high
reasoning: 该实体是 AI 领域的核心参与者，且在提供的源文档中作为技术方案（Managed Agents）的提供方和研究主体出现，信息明确。
---

# Anthropic

Anthropic 是一家总部位于美国的人工智能研究与安全公司，致力于开发可靠、可解释且具有高度可控性的 AI 系统。作为生成式 AI 领域的核心推动者，Anthropic 不仅在基础模型研发上投入巨大，还积极探索如何将 AI 模型转化为能够独立执行复杂任务的“智能体”（Agents）。该公司强调 AI 的安全性与对齐（Alignment），旨在确保其模型在处理长周期、多步骤任务时，能够保持逻辑的一致性与操作的安全性。

在工程实践层面，Anthropic 持续在其官方工程博客中分享关于构建有效智能体、设计任务执行框架（Harnesses）的深度见解。他们通过不断挑战和更新对模型能力的假设，推动了 AI 智能体架构的演进，例如在处理上下文限制、任务规划与执行解耦等关键技术挑战上，提供了重要的行业参考。

### 在本视频中的角色

在本视频（及相关技术文档）中，Anthropic 是“托管智能体”（Managed Agents）概念的提出者与技术推动者。视频内容主要围绕 Anthropic 工程师团队如何通过解耦“大脑”（模型推理）与“双手”（执行工具）来优化智能体表现展开。Anthropic 提供的 [[Claude]] 系列模型（如 [[Claude Sonnet 4.5]]）被作为核心案例，用于分析模型在面对长上下文任务时的行为模式，以及如何通过工程手段解决模型在任务执行中的局限性。

### 相关链接

* [[Claude]]
* [[Claude Sonnet 4.5]]
* [[Managed Agents]]
* [[扩展托管智能体：将大脑与双手解耦]]