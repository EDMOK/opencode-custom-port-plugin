# opencode VS Code Extension

A Visual Studio Code extension that integrates [opencode](https://opencode.ai) directly into your development workflow.

## Prerequisites

This extension requires the [opencode CLI](https://opencode.ai) to be installed on your system. Visit [opencode.ai](https://opencode.ai) for installation instructions.

## Features

- **Quick Launch**: Use `Cmd+Esc` (Mac) or `Ctrl+Esc` (Windows/Linux) to open opencode in a split terminal view, or focus an existing terminal session if one is already running.
- **New Session**: Use `Cmd+Shift+Esc` (Mac) or `Ctrl+Shift+Esc` (Windows/Linux) to start a new opencode terminal session, even if one is already open. You can also click the opencode button in the editor title bar.
- **Context Awareness**: Automatically share your current selection or tab with opencode.
- **File Reference Shortcuts**: Use `Cmd+Option+K` (Mac) or `Alt+Ctrl+K` (Linux/Windows) to insert file references. For example, `@File#L37-42`.
- **Port Configuration**: Configure a fixed port number for opencode server in VS Code settings, or leave empty for automatic port assignment (16384-65535).
- **Automatic Port Conflict Resolution** (Windows): When using a fixed port, the extension automatically detects if the port is already in use and terminates the existing process before starting a new session.

## Configuration

You can customize the extension behavior through VS Code settings:

- **opencode.port**: Set a fixed port number (1024-65535) for the opencode server. Leave empty for automatic port assignment in the range 16384-65535.

To access settings:
1. Open VS Code Settings (`Cmd+,` on Mac, `Ctrl+,` on Windows/Linux)
2. Search for "opencode"
3. Configure the port setting as needed

## Commands

The extension provides the following commands accessible via Command Palette (`Cmd+Shift+P` / `Ctrl+Shift+P`):

- **Open opencode**: Launch opencode in the current terminal or focus existing session
- **Open opencode in new tab**: Start a new opencode session in a new terminal tab
- **Add Filepath to Terminal**: Insert current file path reference into opencode

## Support

This is an early release. If you encounter issues or have feedback, please create an issue at https://github.com/EDMOK/opencode-vscode-extension/issues.

## Installation

### From VS Code Marketplace
1. Open VS Code
2. Go to Extensions view (`Cmd+Shift+X` / `Ctrl+Shift+X`)
3. Search for "opencode"
4. Click Install

---

# opencode VS Code 自定义端口扩展（中文说明）

将 [opencode](https://opencode.ai) 直接集成到您的开发工作流中的 Visual Studio Code 扩展。

## 前提条件

此扩展需要安装 [opencode CLI](https://opencode.ai)。请访问 [opencode.ai](https://opencode.ai) 获取安装说明。

## 功能特性

- **快速启动**：使用 `Cmd+Esc`（Mac）或 `Ctrl+Esc`（Windows/Linux）在分屏终端视图中打开 opencode，或者如果已有会话正在运行则聚焦到现有会话。
- **新会话**：使用 `Cmd+Shift+Esc`（Mac）或 `Ctrl+Shift+Esc`（Windows/Linux）启动新的 opencode 终端会话，即使已有会话处于打开状态。您还可以点击编辑器标题栏中的 opencode 按钮。
- **上下文感知**：自动与 opencode 共享您当前的选择或标签页。
- **文件引用快捷键**：使用 `Cmd+Option+K`（Mac）或 `Alt+Ctrl+K`（Linux/Windows）插入文件引用。例如：`@File#L37-42`。
- **端口配置**：在 VS Code 设置中为 opencode 服务器配置固定端口号，或留空以自动分配端口（16384-65535）。
- **自动端口冲突解决**（Windows）：使用固定端口时，扩展会自动检测端口是否已被占用，并在启动新会话前终止现有进程。

## 配置

您可以通过 VS Code 设置自定义扩展行为：

- **opencode.port**：为 opencode 服务器设置固定端口号（1024-65535）。留空将在 16384-65535 范围内自动分配端口。

访问设置方法：
1. 打开 VS Code 设置（Mac 上 `Cmd+,`，Windows/Linux 上 `Ctrl+,`）
2. 搜索 "opencode"
3. 根据需要配置端口设置

## 命令

扩展提供以下可通过命令面板（`Cmd+Shift+P` / `Ctrl+Shift+P`）访问的命令：

- **Open opencode**：在当前终端中启动 opencode 或聚焦现有会话
- **Open opencode in new tab**：在新终端标签页中启动新的 opencode 会话
- **Add Filepath to Terminal**：将当前文件路径引用插入到 opencode 中

## 支持

这是早期版本。如果遇到问题或有反馈，请在 https://github.com/EDMOK/opencode-vscode-extension/issues 创建 issue。

## 安装

### 从 VS Code 市场安装
1. 打开 VS Code
2. 进入扩展视图（`Cmd+Shift+X` / `Ctrl+Shift+X`）
3. 搜索 "opencode"
4. 点击安装


