# xiaotong-work-releases
小瞳 Work 安装包与自动更新资源
# 小瞳 Work

小瞳 Work 是基于 [Proma](https://github.com/proma-ai/Proma) fork 改造的团队专属 AI 桌面 Agent，面向科学城（广州）数字科技集团有限公司同事，用于日常办公、知识处理与复杂任务协作。

## 现在能做什么

- **Chat 模式**：支持多模型对话、附件解析、图片输入、Markdown、Mermaid、KaTeX、代码高亮、并排对话、系统提示词和上下文管理。
- **Agent 模式**：使用内置 Pi Agent Runtime，支持工作区隔离、权限模式、文件操作、长任务流式输出、计划确认和用户追问。
- **团队模型渠道**：预置团队内部模型渠道和默认模型，成员安装后即可使用，也可以自行添加兼容渠道。
- **主动办公助手**：内置小瞳 Work 身份与公司背景，会在首次使用时主动了解同事的岗位、职责和常见工作，帮助建立更贴合实际办公场景的协作方式。
- **内嵌浏览器自动化**：Agent 可以操作内置受管浏览器，打开网页、观察页面结构、点击或填写控件、切换标签页，并访问本地开发服务。
- **Skills、MCP 与项目指令**：每个项目可以独立配置 Skills 和 MCP Server，并通过 `AGENTS.md` 声明受信项目指令。
- **协作与远程任务**：复杂任务可以拆分为可追踪的协作子 Agent，并支持通过飞书 / Lark 等机器人桥接触发本机工作流。
- **记忆与工具**：Chat 和 Agent 可以使用工作区记忆、联网搜索、内置工具和 Agent 推荐等能力。
- **本地优先**：会话、工作区、附件、配置和 Skills 默认存储在 `~/.xiaotong-work/`，使用 JSON / JSONL 文件组织。
- **桌面体验**：支持文件预览、全局快捷键、快速任务窗口、Agent 运行状态、语音输入以及亮色、暗色和跟随系统主题。

## 模式选择

### Chat 适合

- 日常问答、解释、翻译、润色和轻量代码讨论。
- 读取附件后进行总结、改写和比较。
- 使用联网搜索或记忆工具增强一次性对话。
- 同时比较多个模型的输出，或使用不同系统提示词进行探索。

### Agent 适合

- 修改、创建和整理本地文件。
- 调研、编写报告和处理多步骤任务。
- 使用 MCP、Skills、Shell、Git 和项目文件等外部上下文。
- 需要权限确认、计划模式、后台任务或远程机器人持续跟进的工作。

简单说：**只需要回答时用 Chat，需要行动和交付结果时用 Agent。**

## 截图

### Chat 快速分析

用 Chat 处理轻量但真实的分析任务，整理关注点、生成对比表并快速完成文案。

![Chat 快速分析](./docs/assets/screenshots/proma-chat-demo.png)

### Agent 工作台

Agent 可以在项目根目录和会话工作台中读取文件、推进任务、输出结论，并把可复用文件保留在文件面板中。

![Agent 工作台](./docs/assets/screenshots/proma-agent-demo.png)

### Skills

每个工作区都可以沉淀专属 Skills，把团队经验转化为可重复使用的工作流程。

![工作区 Skills](./docs/assets/screenshots/proma-skills-demo.png)

### Skills 与 MCP

同一个工作区可以管理 stdio / HTTP MCP Server，按需启用或关闭，为不同项目提供不同的外部上下文。

![MCP 配置](./docs/assets/screenshots/proma-mcp-demo.png)

### 流式语音输入

小瞳 Work 支持豆包流式语音输入，既可以向应用内输入框写入内容，也可以向其他应用当前光标位置输入；没有可用光标时会写入剪贴板。

![流式语音输入](./docs/assets/screenshots/proma-typeless-input.png)
