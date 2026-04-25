# XFXCode Downloads

XFXCode 公开下载仓库。这里只发布下载说明、Release notes、安装包和校验值，不包含 XFXCode 源码。

Latest release:

https://github.com/EazyLee30/xfxcode-downloads/releases/latest

## 下载

- Windows x64 免安装版：`XFXCode_<version>_x64-portable.exe`
- macOS Apple Silicon：`XFXCode_<version>_aarch64.dmg`

Windows 版本是 portable EXE，下载后双击运行，不需要 setup，不需要安装向导。

## 安装

### Windows

1. 打开最新 Release。
2. 下载 `XFXCode_<version>_x64-portable.exe`。
3. 双击运行。
4. 如果 Windows SmartScreen 提示未知发布者，请确认文件来自本仓库官方 Release 页面后，再选择“更多信息 / 仍要运行”。

### macOS

1. 打开最新 Release。
2. 下载 `XFXCode_<version>_aarch64.dmg`。
3. 打开 DMG，把 XFXCode 拖到 Applications。
4. 如果 macOS 首次启动时拦截，在“系统设置 > 隐私与安全性”里允许打开。

当前 macOS 构建面向 Apple Silicon。

## 第一次使用

1. 启动 XFXCode。
2. 点击“打开文件夹”，选择项目目录。
3. 打开“设置”。
4. 填入 DeepSeek API Key。
5. 选择默认模型：
   - `deepseek-v4-flash`：日常快速编码。
   - `deepseek-v4-pro`：审查、合并、高风险推理任务。
6. 使用 **Ask** 做只读理解和分析，使用 **Agent** 让 XFXCode 通过工具修改文件。

## 主要能力

- Monaco 多标签编辑器、资源管理器、终端、AI 面板、设置和技能中心。
- DeepSeek V4 Flash / Pro 模型 profile。
- Agent / Ask 双模式。
- 文件读写、搜索、创建、移动、删除等工具调用。
- 联网搜索和网页抓取工具。
- Agent Skills：支持内置、本地、项目、ClawHub 和生成式技能。
- DeepSeek V4 Agent Harness：stage-aware profile、tool choice、cache telemetry、governance trace。
- 每条 Assistant 回复下方展示文件变更卡片，支持打开文件、复制、反馈、时间和安全撤销。

## 校验文件

Release 中会附带 checksum。你也可以手动计算：

macOS:

```bash
shasum -a 256 XFXCode_<version>_aarch64.dmg
```

Windows PowerShell:

```powershell
Get-FileHash .\XFXCode_<version>_x64-portable.exe -Algorithm SHA256
```

把输出和 Release 中的 checksum 对比即可。

## 源码与授权

本仓库是公开下载仓库，只包含说明和 Release 二进制，不包含 XFXCode 源码。

XFXCode 当前是闭源 / 专有软件。除非另有书面许可：

- 你可以下载并运行官方 Release 二进制。
- 你不得复制、修改、再分发、售卖或重新授权 XFXCode 源码。
- 你不得冒用 XFXCode 名称、品牌或官方构建。
- 第三方依赖仍遵循各自许可证。

## English

This repository is the public download repository for XFXCode. It contains download instructions, Release notes, binaries, and checksums only. It does not contain the XFXCode source code.

XFXCode is a lightweight desktop AI IDE for agentic coding workflows. It helps you open a project, ask an AI agent to inspect and edit files, review file changes, and keep tool execution visible through governance traces.

Available builds:

- Windows x64 portable EXE: `XFXCode_<version>_x64-portable.exe`
- macOS Apple Silicon DMG: `XFXCode_<version>_aarch64.dmg`

The Windows build is portable. Download it and double-click the EXE. There is no setup installer.

XFXCode is currently proprietary / closed-source software. Public Release downloads do not grant permission to copy, modify, redistribute, resell, or relicense the source code.
