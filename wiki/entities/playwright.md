---
title: Playwright
type: entity
tags: [自动化测试, 浏览器自动化, 评估工具, 软件工程]
summary: Playwright 是一个由 Microsoft 开发的开源浏览器自动化框架，在多代理架构中常被用作评估器与实时网页交互的接口。
sources: ["raw/notebooklm-analysis/harness-design-long-running-apps.md"]
created: 2024-05-22
updated: 2024-05-22
layer: L1
confidence: high
reasoning: 该实体在报告中被明确提及为评估器与前端页面交互的核心工具，是实现自动化评估循环的关键组件。
---

# Playwright

Playwright 是一个功能强大的开源自动化库，旨在通过单一 API 实现对 Chromium、Firefox 和 WebKit 等主流浏览器的跨平台控制。它不仅支持端到端的自动化测试，还广泛应用于网页抓取、性能监控以及复杂的 UI 交互模拟。Playwright 的核心优势在于其对现代 Web 应用（如单页应用 SPA）的深度支持，能够处理异步加载、动态内容渲染以及复杂的网络请求拦截，这使其成为构建自动化工作流的首选工具。

### 在本视频中的角色

在 [[用于长期运行应用程序开发的工具框架设计]] 的上下文中，Playwright 被集成在评估器代理（Evaluator Agent）的工具集中，作为一种 MCP（Model Context Protocol）工具存在。它的主要作用是赋予评估器“视觉”与“交互”能力：当生成器代理创建出 HTML/CSS/JS 前端后，评估器通过 Playwright 直接加载并浏览实时页面。

Playwright 在此流程中执行以下关键任务：
1. **实时交互**：评估器通过 Playwright 模拟用户行为，对页面进行点击、滚动或导航，以验证交互逻辑。
2. **视觉捕获**：在评分前，Playwright 负责对页面进行截图，使评估器能够基于视觉呈现进行美学与布局评估。
3. **实现审查**：评估器利用 Playwright 深入研究页面的实现细节，确保生成的代码不仅在视觉上符合要求，在技术实现上也达到预设标准。

这种基于 Playwright 的实时反馈机制，构成了 [[多代理结构]] 中闭环迭代的核心，确保了生成器能够根据真实的渲染结果进行持续优化。

### 相关链接
- [[用于长期运行应用程序开发的工具框架设计]]
- [[多代理结构]]