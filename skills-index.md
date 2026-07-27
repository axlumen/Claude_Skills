# Skills 索引

> 全局 Skills — 所有项目通用。最后更新：2026-07-27。
>
> **原则：** 只放跨项目通用的技能。项目专属技能放在对应项目的 `.claude/skills/` 下。
>
> **当前数量：** 19 个全局 skill + 9 个 Obsidian 项目 skill。

---

## coding/ 开发辅助

| 技能 | 说明 |
|------|------|
| test-driven-development | 测试驱动开发，红-绿-重构循环，含哲学、实操、反模式 |
| code-refactoring-refactor-clean | 代码重构专家，Clean Code 原则和最佳实践 |
| improve-codebase-architecture | 改进代码架构，SOLID 原则和设计模式 |

## design/ 设计能力

| 技能 | 说明 |
|------|------|
| frontend-design | 通用前端设计指南，token-first 哲学，技术栈中立。**兜底通用**：仪表盘/产品 UI/多步流程/数据表。landing/portfolio/极简/粗野/品牌等有更专门的 skill 时优先用专门的（见 description 互斥说明） |
| full-output-enforcement | 完整输出强制——防止代码截断，禁止占位符模式，处理 token 限制下的分段输出 |
| excalidraw-diagram | 从文本生成 Excalidraw 图表，支持 Obsidian(.md)、标准(.excalidraw)、动画三种模式 |
| mermaid-visualizer | 从文本生成专业 Mermaid 图表，流程图/架构图/对比图/思维导图，内置语法错误预防 |

## writing & thinking/ 内容与思维

| 技能 | 说明 |
|------|------|
| humanizer | 去除 AI 写作痕迹（33 文件，仅在用户明确要求润色/去AI味时触发） |
| caveman | 超压缩通信模式，省 ~75% token，保持技术准确性 |
| brainstorming | 创意工作前的头脑风暴，探索用户意图和需求 |
| zoom-out | 拉远视角，获取更宏观的上下文和高层理解 |

## planning/ 规划执行

| 技能 | 说明 |
|------|------|
| writing-plans | 编写多步骤任务实施计划（编码前使用） |
| executing-plans | 执行已有实施计划，带审查检查点 |
| planning-with-files-zh | Manus 风格文件规划系统（中文），创建 task_plan.md/findings.md/progress.md，支持会话恢复 |

## productivity/ 效率工具

| 技能 | 说明 |
|------|------|
| ai-session-archiver | 跨工具扫描、统一归档、定期清理本地 AI 对话记录（Cursor/Claude Code/Codex/Cline/GLM 等） |

## security/ 安全分析

| 技能 | 说明 |
|------|------|
| reverse-flow-skill | 逆向工程工作流——二进制/固件/移动应用/脚本/协议分析，含恶意软件分析、漏洞发现、补丁差异、根因分析，激活口令「真心为你」 |

## automation/ 自动化 & 元技能

| 技能 | 说明 |
|------|------|
| find-skills | 查找可安装的 Skills |
| skill-creator | 创建/优化/测试 Skills，支持评估和基准测试 |
| teaching-system | 综合性教学系统，结合 Bloom 掌握学习理论，支持任何主题的系统化学习 |

---

## 项目专属 Skills（不在此目录）

以下 Skills 应放在对应项目的 `.claude/skills/` 下：

### Obsidian Vault (`E:\文档\Obsidian\.claude\skills\`)

| 技能 | 说明 |
|------|------|
| obsidian-knowledge-brain | 知识大脑 v4.0，跨会话记忆 + 自动知识库（44 文件，按需加载） |
| obsidian-canvas-creator | Obsidian Canvas 画布创建（Obsidian 专有格式） |
| zhengxi-views | 正熙视角——基金经理郑希知识库（88 文件语料 + 基金数据，按需读取） |
| llm-wiki | Karpathy 风格 LLM 知识库，自编译 Obsidian markdown wiki |
| table-github-capability-router | GitHub 入库 + 能力路由表（Markdown-first 工作流，README 即 SOP） |
| equity-research | 股权研究套件（3-statement/DCF/comps/earnings/sector 五合一路由） |

---

## 变更记录

### 2026-07-27
- ✅ 新增 reverse-flow-skill（逆向工程工作流，19 个全局 skill）

### 2026-07-22
- 🗑️ 删除 design 类 taste-skill 整簇（7 个）：design-taste-frontend、minimalist-ui、industrial-brutalist-ui、redesign-existing-projects、stitch-design-taste、imagegen-frontend-web、brandkit——统一由 frontend-design 覆盖
- 🗑️ 删除 storage-analyzer（磁盘分析）
- 🗑️ 删除不存在的索引条目：js-reverse-automation--skill、interactive-learning、teach、financial-plugins
- ✅ 添加遗漏索引：teaching-system、ai-session-archiver、llm-wiki、table-github-capability-router
- 🔒 humanizer 加触发守卫（33 文件，仅在明确要求润色时触发）
- 🔒 obsidian-knowledge-brain 改 Always → On-demand（44 文件，按需加载）
- 🔄 金融 5 skill 合并为 equity-research（3-statement-model + comps-analysis + dcf-model + earnings-analysis + sector-overview → 1 个路由 + 5 个 reference，358 行总计）

### 2026-06-26
- ✅ 通用 skill 已从项目移至全局（brainstorming、caveman、executing-plans、writing-plans、planning-with-files-zh、zoom-out）
- ✅ 去重完成：humanizer、excalidraw-diagram、mermaid-visualizer 项目级副本已删除
- ✅ 清理垃圾数据：telemetry（失败事件日志）
- ✅ 清理误放项目：impeccable（125MB 完整 npm 项目，可通过 npx 按需安装）
- ✅ 清理无用 skill：mintlify（文档站工具）、ppt-master（PPT 生成，83MB）、defuddle（与 WebFetch 重叠）
