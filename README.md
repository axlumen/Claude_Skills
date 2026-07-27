# Skills 技能库

Claude Code 全局 AI 技能模块，所有项目通用。

> 最后更新：2026-07-27
>
> **原则：** 此目录只放跨项目通用技能。项目专属技能放在对应项目的 `.claude/skills/` 下。
>
> **当前数量：** 19 个全局 skill + 9 个 Obsidian 项目 skill。

## 技能总览（18 个）

### 开发辅助（3）

| 技能 | 说明 |
|------|------|
| test-driven-development | 测试驱动开发，红-绿-重构循环 |
| code-refactoring-refactor-clean | 代码重构专家，Clean Code 原则 |
| improve-codebase-architecture | 改进代码架构，SOLID 原则和设计模式 |

### 设计能力（4）

| 技能 | 说明 |
|------|------|
| frontend-design | 通用前端设计指南，token-first 哲学，**兜底通用** |
| full-output-enforcement | 完整输出强制（防代码截断） |
| excalidraw-diagram | 从文本生成 Excalidraw 图表（支持动画） |
| mermaid-visualizer | 从文本生成专业 Mermaid 图表 |

### 内容与思维（4）

| 技能 | 说明 |
|------|------|
| humanizer | 去除 AI 写作痕迹（33 文件，仅明确要求润色时触发） |
| caveman | 超压缩通信模式，省 ~75% token |
| brainstorming | 创意工作前的头脑风暴/需求探索 |
| zoom-out | 拉远视角，获取宏观上下文 |

### 规划执行（3）

| 技能 | 说明 |
|------|------|
| writing-plans | 编写多步骤任务实施计划 |
| executing-plans | 执行已有实施计划（带审查检查点） |
| planning-with-files-zh | Manus 风格文件规划系统（中文） |

### 效率工具（1）

| 技能 | 说明 |
|------|------|
| ai-session-archiver | 跨工具归档、清理本地 AI 对话记录 |

### 安全分析（1）

| 技能 | 说明 |
|------|------|
| reverse-flow-skill | 逆向工程工作流（二进制/固件/脚本/漏洞分析），激活口令「真心为你」 |

### 自动化 & 元技能（3）

| 技能 | 说明 |
|------|------|
| find-skills | 查找可安装的 Skills |
| skill-creator | 创建/优化/测试 Skills |
| teaching-system | 综合性教学系统（Bloom 掌握学习理论） |

## 项目专属 Skills（9 个）

以下 Skills 不在此目录，而是放在各自项目中：

| 项目 | 位置 | Skills |
|------|------|--------|
| Obsidian Vault | `E:\文档\Obsidian\.claude\skills\` | obsidian-knowledge-brain, obsidian-canvas-creator, zhengxi-views, llm-wiki, table-github-capability-router, equity-research |

## 详细索引

详见 [skills-index.md](skills-index.md)（含变更记录和分类说明）。

## 大文件 Skill 触发守卫

以下 skill 文件数较多，description 加了显式触发条件避免误加载：

| 技能 | 文件数 | 触发条件 |
|------|--------|---------|
| obsidian-knowledge-brain | 44 | 按需加载（On-demand），手动口令触发 |
| humanizer | 33 | 用户明确要求润色/去AI味 |
| ai-session-archiver | 27 | 关键词：归档对话/导出session/清理对话记录 |
| skill-creator | 21 | 用户要求创建/优化 skill |
