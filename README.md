<p align="center">
  <img src="./assets/xfxcode-icon.png" width="104" height="104" alt="XFXCode icon" />
</p>

<h1 align="center">XFXCode Project</h1>

<p align="center">
  <strong>专为上海市民办新复兴初级中学开发的 AI IDE</strong>
</p>

<p align="center">
  面向校园创新教育、AI 编程实践、项目制学习和真实代码创作的桌面级智能开发环境。
</p>

<p align="center">
  <a href="https://github.com/EazyLee30/xfxcode-project/releases/latest"><strong>Download Latest Release</strong></a>
  ·
  <a href="#快速开始">快速开始</a>
  ·
  <a href="#核心能力">核心能力</a>
  ·
  <a href="#校验下载文件">校验文件</a>
</p>

<p align="center">
  <img alt="Release" src="https://img.shields.io/github/v/release/EazyLee30/xfxcode-project?style=for-the-badge&label=release" />
  <img alt="Windows" src="https://img.shields.io/badge/Windows-Portable_EXE-1677ff?style=for-the-badge&logo=windows11&logoColor=white" />
  <img alt="macOS" src="https://img.shields.io/badge/macOS-Apple_Silicon-111111?style=for-the-badge&logo=apple&logoColor=white" />
  <img alt="DeepSeek" src="https://img.shields.io/badge/DeepSeek_V4-Agent_Harness-00A67E?style=for-the-badge" />
</p>

---

## 项目定位

XFXCode Project 是 XFXCode 的公开下载与发布说明仓库。XFXCode 是一款专为 **上海市民办新复兴初级中学** 打造的 AI IDE：它把传统代码编辑器、AI Agent、工具调用、项目文件操作、技能系统和治理审计整合在一个桌面应用中，让学生和教师可以在真实工程环境里完成 AI 辅助编程、作品创作和代码学习。

它不是一个普通聊天机器人，也不是简单套壳网页。XFXCode 的设计目标是让 AI 真正进入“读代码、改代码、跑命令、看结果、可撤销、可审查”的完整学习闭环。

> 本仓库只提供公开下载、Release notes、安装包和校验值，不包含 XFXCode 私有源码。

## 一句话介绍

| 维度 | XFXCode 提供的能力 |
| --- | --- |
| 面向对象 | 上海市民办新复兴初级中学的 AI 编程教学与创新项目实践 |
| 产品形态 | Windows / macOS 桌面 AI IDE |
| AI 能力 | DeepSeek V4 Flash / Pro、Agent Harness、工具调用、Skills |
| 学习场景 | Python / Web / 项目制学习 / 代码讲解 / 自动修改 / 作品打磨 |
| 管理边界 | 文件变更可见、工具步骤可追踪、危险操作可确认、下载包可校验 |

## 下载

最新版本：

https://github.com/EazyLee30/xfxcode-project/releases/latest

| 平台 | 文件 | 说明 |
| --- | --- | --- |
| Windows x64 | `XFXCode_<version>_x64-portable.exe` | 免安装 portable EXE，下载后双击运行 |
| macOS Apple Silicon | `XFXCode_<version>_aarch64.dmg` | 打开 DMG 后拖入 Applications |
| 校验值 | `SHA256SUMS.txt` | 用于确认下载文件未损坏、未被替换 |

**不要下载** GitHub 自动生成的 `Source code (zip)` / `Source code (tar.gz)` 来安装 XFXCode。它们只是本公开下载仓库的快照，不是应用源码，也不是安装包。

## 快速开始

### Windows

1. 打开最新 Release。
2. 下载 `XFXCode_<version>_x64-portable.exe`。
3. 双击运行。
4. 如果 Windows SmartScreen 提示未知发布者，请确认文件来自本仓库官方 Release 页面后，再选择“更多信息 / 仍要运行”。

Windows 版本是 portable EXE，不需要 setup，不需要管理员安装，不进入安装向导。

### macOS

1. 打开最新 Release。
2. 下载 `XFXCode_<version>_aarch64.dmg`。
3. 打开 DMG，把 XFXCode 拖到 Applications。
4. 如果首次启动被 macOS 拦截，在“系统设置 > 隐私与安全性”里允许打开。

当前 macOS 构建面向 Apple Silicon。

## 第一次使用

1. 启动 XFXCode。
2. 点击“打开文件夹”，选择你的课程项目、练习项目或作品目录。
3. 打开“设置”，填入 DeepSeek API Key。
4. 选择默认模型：
   - `deepseek-v4-flash`：适合日常快速编码、问答、普通工具循环。
   - `deepseek-v4-pro`：适合审查、合并、高风险推理和复杂分析。
5. 在 AI 面板中选择工作方式：
   - **Ask**：只读理解代码、解释知识点、定位问题。
   - **Plan**：先生成可审查的实施计划和待办拆解，不急着改文件。
   - **Agent**：允许 AI 调用工具修改项目文件。

API Key 会保存在本机设置中。请不要把 API Key 粘贴进聊天内容、项目源码或公开截图。

## 核心能力

### 1. 桌面级 IDE 体验

- Monaco 多标签代码编辑器。
- 项目资源管理器。
- 集成终端。
- AI 面板与状态栏。
- 设置中心和技能中心。
- 支持 Ctrl / Command + 鼠标滚轮缩放编辑器字号。

### 2. DeepSeek V4 Agent Harness

XFXCode 针对 DeepSeek V4 做了专门的 Agent Harness 融合：

- `deepseek-v4-flash` 用于快速执行、定位、普通工具循环。
- `deepseek-v4-pro` 用于审查、合并、高风险 replay 和复杂推理。
- 支持 thinking / tool-call continuity。
- 支持 stage-aware `tool_choice`。
- 支持 context cache telemetry。
- 原生工具调用不稳定时，可切换 ReAct XML 手动工具解析 fallback。

### 3. Ask / Plan / Agent 三模式

| 模式 | 适合场景 | 文件修改 |
| --- | --- | --- |
| Ask | 解释代码、知识点讲解、查找问题、阅读项目 | 默认不主动修改 |
| Plan | 复杂任务拆解、课堂讨论、方案评审、执行前确认 | 先产出计划，不直接改文件 |
| Agent | 实现功能、修复 bug、重构代码、生成页面、运行命令 | 可通过工具修改 |

这种设计很适合课堂环境：先用 Ask 理解，再用 Plan 拆解任务和讨论方案，确认后再用 Agent 实践，最后 review 变更。

### 4. Plan 模式：先规划，再执行

Plan 模式是 XFXCode 面向教学和复杂任务设计的“刹车层”。当一个需求涉及多个文件、多个步骤或存在不确定性时，Plan 会先让 AI 输出结构化计划，而不是立刻动手改代码。

Plan 模式适合：

- 把大作业拆成可执行的待办列表。
- 在动手前比较不同实现方案。
- 让学生先讲清楚“为什么这么做”，再进入 Agent 执行。
- 给教师一个检查点，确认任务边界、风险和验证方式。
- 对重构、页面生成、工具安装、批量修改等高影响操作先做预案。

典型流程：

```text
Ask：先解释这个项目现在的结构。
Plan：为“新增一个课程作品展示页”生成实施计划，不要改文件。
Agent：按计划执行第一步，并在完成后说明改了哪些文件。
Review：查看消息下方的文件变更卡片，必要时撤销或继续下一步。
```

### 5. 文件变更可见、可追踪、可撤销

每条 Assistant 回复下方都会展示本轮变更：

- 修改了几个文件。
- 每个文件的路径。
- 新增 / 删除行数。
- 点击打开文件。
- 复制回答、反馈、查看时间。
- 对可安全恢复的变更执行撤销。

新建文件、多文件撤销、不可撤销变更等风险操作会有更明确的提示，避免误操作。

### 6. Skills 能力系统

XFXCode 支持 Agent Skills，让 AI 按任务加载更专业的指令和资料：

- 内置 bundled skills。
- 用户级 `~/.xfxcode/skills`。
- 项目级 `.xfxcode/skills`。
- `.agents/skills` / `.claude/skills`。
- ClawHub skills。
- 本地导入、URL 导入、AI 生成的技能草稿。

这让 XFXCode 不只是“模型调用器”，而是可以逐步沉淀学校自己的课程技能、项目模板和知识库。

## 校园使用场景

| 场景 | 示例 |
| --- | --- |
| 编程入门 | 解释 Python / JavaScript 代码，指出变量、函数、循环和条件判断 |
| 作品开发 | 生成网页、小游戏、数据展示页面、课程项目原型 |
| 任务规划 | 用 Plan 模式拆解功能需求，先讨论方案再进入实现 |
| 代码修复 | 读取报错、定位文件、修改代码、解释为什么这样改 |
| 项目制学习 | 围绕一个作品目录持续迭代，保留文件结构和变更记录 |
| 教师演示 | 用 Ask / Plan / Agent 展示“理解 -> 计划 -> 修改 -> 验证”的完整过程 |
| AI 素养教育 | 让学生看到 AI 调用了什么工具、改了什么文件、哪些操作需要确认 |

## 安全与治理

XFXCode 的 AI 执行有明确边界：

- Ask 模式偏只读。
- Plan 模式先生成计划和待办，适合执行前确认。
- Agent 模式才允许写文件。
- 工具调用过程可见。
- 失败工具不会伪装成成功文件变更。
- 大文件或无快照变更会标记为不可撤销。
- 删除新建文件、多文件撤销等操作需要确认。
- Governance trace 记录工具暴露、模型路由、缓存命中和 replay metadata。

AI 可以提升学习效率，但不替代学生理解。建议课堂和项目提交中保留 review、讲解和测试环节。

## 校验下载文件

Release 中会附带 checksum。你也可以手动计算：

macOS:

```bash
shasum -a 256 XFXCode_<version>_aarch64.dmg
```

Windows PowerShell:

```powershell
Get-FileHash .\XFXCode_<version>_x64-portable.exe -Algorithm SHA256
```

把输出和 Release 中的 `SHA256SUMS.txt` 对比即可。

## 源码与授权

本仓库是公开下载仓库，只包含说明、Release notes、安装包和校验值，不包含 XFXCode 源码。

XFXCode 当前是闭源 / 专有软件。除非另有书面许可：

- 你可以下载并运行官方 Release 二进制。
- 你不得复制、修改、再分发、售卖或重新授权 XFXCode 源码。
- 你不得冒用 XFXCode 名称、品牌或官方构建。
- 第三方依赖仍遵循各自许可证。

## English

XFXCode Project is the public download and release-notes repository for XFXCode, a desktop AI IDE developed for Shanghai Xin Fuxing Private Junior High School.

This repository contains download instructions, Release notes, binaries, and checksums only. It does not contain the private XFXCode application source code.

Available builds:

- Windows x64 portable EXE: `XFXCode_<version>_x64-portable.exe`
- macOS Apple Silicon DMG: `XFXCode_<version>_aarch64.dmg`

GitHub automatically adds `Source code (zip)` and `Source code (tar.gz)` to every release. Those archives are only snapshots of this public download repository. To install XFXCode, download the `.exe` or `.dmg` asset from the Release page.

XFXCode supports Ask, Plan, and Agent workflows: Ask explains, Plan breaks work into reviewable steps, and Agent executes file changes through governed tools.
