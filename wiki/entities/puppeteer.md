---
title: Puppeteer
type: entity
tags: [工具, 浏览器自动化, 测试框架]
summary: Puppeteer 是一个用于控制 Chrome 或 Chromium 的 Node.js 库，在长期运行代理的开发中常作为端到端测试的核心工具，帮助 AI 代理模拟人类用户行为以验证功能有效性。
sources: ["raw/notebooklm-analysis/harness-design-long-running-apps.md"]
created: 2024-05-22
updated: 2024-05-22
layer: L1
confidence: high
reasoning: 该实体在报告中被明确提及为提升 Claude 代理端到端测试能力的关键工具，且具有明确的 MCP 服务器集成场景。
---

# Puppeteer

Puppeteer 是一个由 Google 开发的 Node.js 库，提供了一套高级 API 来通过 DevTools 协议控制 Chrome 或 Chromium 浏览器。在构建复杂的 Web 应用或长期运行的代理系统时，Puppeteer 扮演着至关重要的角色。它允许开发者通过编程方式模拟真实用户的操作，如点击、输入、导航以及页面截图，从而实现对 Web 应用的自动化测试和交互。

在 AI 代理的开发实践中，Puppeteer 被证明是提升代理性能的关键组件。由于大语言模型（如 Claude）在缺乏外部验证的情况下容易产生“功能已完成”的幻觉，通过集成 Puppeteer MCP 服务器，代理能够像人类用户一样在真实的浏览器环境中执行端到端测试。这种能力使得代理能够识别并修复那些仅通过静态代码分析无法发现的逻辑错误。然而，Puppeteer 的使用也存在局限性，例如它在处理浏览器原生模态框（如 alert 或 confirm）时可能存在视觉识别障碍，这要求开发者在使用时需结合其他工具进行补充。

## 在本视频中的角色

在关于长期运行代理的设计分析中，Puppeteer 作为一种核心的浏览器自动化工具被引入。它通过 MCP（Model Context Protocol）服务器与 Claude 代理集成，使得代理能够实时观察并验证其构建的 Web 应用功能。通过 Puppeteer，代理不仅能执行代码，还能通过截图和交互反馈来验证端到端的功能是否真正符合预期，从而显著提高了代理在复杂任务中的准确性和可靠性。

## 相关链接

- [[端到端测试]]
- [[用于长期运行代理的有效工具框架]]