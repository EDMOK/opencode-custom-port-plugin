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

### Manual Installation
1. Download the latest `.vsix` file from the [releases page](https://github.com/EDMOK/opencode-vscode-extension/releases)
2. In VS Code, open Command Palette (`Cmd+Shift+P` / `Ctrl+Shift+P`)
3. Run "Extensions: Install from VSIX..."
4. Select the downloaded `.vsix` file

## Development

1. `code sdks/vscode` - Open the `sdks/vscode` directory in VS Code. **Do not open from repo root.**
2. `bun install` - Run inside the `sdks/vscode` directory.
3. Press `F5` to start debugging - This launches a new VS Code window with the extension loaded.

#### Making Changes

`tsc` and `esbuild` watchers run automatically during debugging (visible in the Terminal tab). Changes to the extension are automatically rebuilt in the background.

To test your changes:

1. In the debug VS Code window, press `Cmd+Shift+P`
2. Search for `Developer: Reload Window`
3. Reload to see your changes without restarting the debug session
