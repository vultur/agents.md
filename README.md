<div align="center">

# AGENTS.md

用户级智能体全局指导

旨在通过上下文工程减少模型幻觉并提升智能体性能

使用基于最佳实践的持久性上下文，确保所有项目遵循一致的执行策略

</div>

## 项目概述

`AGENTS.md` 为 AI 智能体提供可预测的上下文指导，包括构建步骤、编码风格及工作流程中的常用命令。

通过将全局指导与项目特定的覆盖规则相结合，无论打开哪个代码库，你都能够以一致的预期开始每个任务。

## 核心指令

> [!TIP]
> **设计哲学**：结论必须有依据、推理必须可解释、过程必须可审计；无法确认时优先拒绝或降级回答。

- 🎓 **批判思维**：基于证据和逻辑评估，审视假设与结论减少幻觉
- 🧠 **逐步推理**：采用链式思考分解任务，确保逻辑完整可追溯
- 🔍 **事实验证**：引用可靠来源，承认不确定性，杜绝编造信息
- ⚖️ **保持中立**：消除情绪偏向，专注任务目标与可验证事实
- 🔄 **循环自检**：结构化输出并多轮验证，保证结果一致可控

## 使用指南

### AI 大语言模型

作为系统指令或用户消息（如 ChatGPT、Claude、Gemini 等）：

```markdown
请将以下内容视为你的全局行为规范，在本对话及后续任务中**始终遵循，不得偏离**：

<agents.md>
（粘贴完整 AGENTS.md 内容）
</agents.md>
```

### AI 编程智能体

作为智能体的**全局指导**（如 Codex、Claude Code、Gemini CLI 等）：

- Codex：[使用 AGENTS.md 进行自定义说明](https://developers.openai.com/codex/guides/agents-md)
- OpenCode：[在 AGENTS.md 中设置全局规则](https://opencode.ai/docs/zh-cn/rules/#全局级)
- Cursor CLI：[使用 AGENTS.md 定义智能体指令](https://cursor.com/docs/rules#agentsmd)
- Gemini CLI：[使用 GEMINI.md 导入实现上下文模块化](https://geminicli.com/docs/cli/gemini-md/#modularize-context-with-imports)
- Claude Code：[使用 CLAUDE.md 导入其它文件](https://code.claude.com/docs/zh-CN/memory#agents-md)

### AI IDE 工具/助手

作为智能体的**用户规则**使用。

## 参考文档

- [Codex 最佳实践](https://developers.openai.com/codex/learn/best-practices)
- [Gemini 提示设计策略](https://ai.google.dev/gemini-api/docs/prompting-strategies?hl=zh-cn)
- [Claude 提示词最佳实践](https://platform.claude.com/docs/zh-CN/test-and-evaluate/strengthen-guardrails/reduce-hallucinations)
