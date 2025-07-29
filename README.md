# Aolarhapsody Monorepo

> Aolarhapsody 项目的官方 monorepo，包含前端、后端和内部工具链。

[English](./README.en.md) | 简体中文

<p align="center">
  <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
  <img src="https://img.shields.io/badge/pnpm-v10.13.1-orange" alt="pnpm version">
  <img src="https://img.shields.io/badge/TypeScript-^5.0.0-blue" alt="TypeScript version">
  <img src="https://img.shields.io/badge/React-^18.0.0-cyan" alt="React version">
  <img src="https://img.shields.io/badge/Node.js-^20.0.0-green" alt="Node.js version">
</p>

## 📖 项目简介

本项目是一个基于 pnpm workspace 的 monorepo，用于管理 Aolarhapsody 的所有代码。它整合了现代化的前端和后端技术，并配备了一套强大的、受 `vben` 启发的内部脚本工具，以确保代码质量和开发效率。

## ✨ 技术栈

-   **前端**: `React`, `TypeScript`, `Vite`
-   **后端**: `Node.js`, `TypeScript`, `Express` (或类似的框架)
-   **包管理器**: `pnpm`
-   **代码质量**: `ESLint`, `Prettier`, `Stylelint`, `Commitlint`, `Cspell`
-   **Git Hooks**: `lefthook`
-   **内部工具**: 使用 `cac`, `@clack/prompts`, `unbuild` 构建的自定义 CLI 工具。

## 📂 项目结构

```
.
├── backend/         # 后端服务
├── frontend/        # 前端应用
├── scripts/         # 内部 CLI 工具和脚本
│   ├── ash/         # 辅助脚本集合 (ash)
│   ├── turbo-run/   # 交互式脚本运行器 (ar-turbo)
│   └── deploy/      # 部署相关脚本和配置
├── package.json
└── pnpm-workspace.yaml
```

## 🚀 快速开始

1.  **克隆项目**
    ```bash
    git clone <repository-url> aolarhapsody-monorepo
    cd aolarhapsody-monorepo
    ```

2.  **安装依赖**
    > 本项目强制使用 pnpm 作为包管理器。
    ```bash
    pnpm install
    ```

3.  **启动开发环境**
    ```bash
    # 启动所有服务的开发模式
    pnpm dev

    # 或单独启动前端
    pnpm dev:front

    # 或单独启动后端
    pnpm dev:backend
    ```

## 🛠️ 可用脚本

-   `pnpm dev`: 启动所有包的开发模式。
-   `pnpm build`: 构建所有包。
-   `pnpm check`: 运行所有的代码检查（linting, cspell）。
-   `pnpm format`: 格式化所有代码。
-   `pnpm clean`: 清理所有构建产物和 `node_modules`。

## 📄 许可证

本项目采用 [LICENSE](./LICENSE) 许可证。
