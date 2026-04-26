# PEGit

**Prompt Version Git** — 将 Git 的版本控制能力应用于 AI Prompt 管理

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

## 📖 简介

PEGit 是一个用于管理 AI Prompt 版本控制的工具。它借鉴 Git 的核心概念（分支、合并、回滚、标签），为 Prompt 工程提供完整的版本管理能力。

### 核心特性

- 🔄 **版本追踪** — 记录每个 Prompt 的变更历史
- 🌿 **分支管理** — 支持 Prompt 的并行实验和迭代
- 🔀 **合并与冲突解决** — 合并不同版本的 Prompt
- 🏷️ **标签与发布** — 标记稳定的 Prompt 版本
- 👥 **协作** — 支持多用户 Prompt 协作开发
- 📊 **Diff 对比** — 可视化 Prompt 版本差异

## 🚀 快速开始

### 安装

```bash
# 从源码安装
git clone https://github.com/gxy2016/PEGit.git
cd PEGit
pip install -e .
```

### 基本用法

```bash
# 初始化 Prompt 仓库
pegit init

# 添加 Prompt 文件
pegit add prompts/my-prompt.md

# 提交变更
pegit commit -m "feat: 优化角色扮演 Prompt"

# 查看历史
pegit log

# 创建分支进行实验
pegit branch experiment-v2
pegit checkout experiment-v2
```

## 📁 项目结构

```
PEGit/
├── pegit/              # 核心库
│   ├── __init__.py
│   ├── core.py         # 核心版本控制逻辑
│   ├── storage.py      # 存储后端
│   └── cli.py          # 命令行接口
├── prompts/            # 示例 Prompt 模板
├── tests/              # 测试套件
├── docs/               # 文档
├── README.md
├── CHANGELOG.md
├── LICENSE
├── pyproject.toml
└── .github/            # GitHub 配置
    ├── ISSUE_TEMPLATE/
    ├── PULL_REQUEST_TEMPLATE.md
    └── workflows/
```

## 🛠️ 技术栈

- **语言**: Python 3.9+
- **包管理**: pip / pyproject.toml
- **测试**: pytest
- **CI/CD**: GitHub Actions

## 📋 开发指南

### 环境设置

```bash
# 创建虚拟环境
python -m venv venv
source venv/bin/activate  # Linux/macOS
# venv\Scripts\activate   # Windows

# 安装依赖
pip install -e ".[dev]"
```

### 运行测试

```bash
pytest tests/ -v
```

### 提交规范

本项目遵循 [Conventional Commits](https://www.conventionalcommits.org/) 规范：

```
feat: 新功能
fix: 修复 bug
docs: 文档更新
style: 代码格式
refactor: 重构
test: 测试相关
chore: 构建/工具链
```

## 🤝 贡献

欢迎贡献！请查看 [PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md) 了解提交流程。

1. Fork 本仓库
2. 创建功能分支 (`git checkout -b feature/amazing-feature`)
3. 提交变更 (`git commit -m 'feat: add amazing feature'`)
4. 推送到分支 (`git push origin feature/amazing-feature`)
5. 提交 Pull Request

## 📜 许可证

本项目采用 [MIT License](LICENSE)。

## 📮 联系方式

- 提交 Issue: [GitHub Issues](https://github.com/gxy2016/PEGit/issues)
- 讨论: [GitHub Discussions](https://github.com/gxy2016/PEGit/discussions)
