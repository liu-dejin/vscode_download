# 📦 VS Code Extension Downloader

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.2-green.svg)

> **VS Code Extension Downloader** 是一个高效的油猴脚本（UserScript），旨在优化 Visual Studio Code Marketplace 的下载体验。它允许用户直接下载插件的 `.vsix` 安装包，无论是最新版本还是历史版本。

## 🌟 背景与痛点

在某些开发环境（如 Trae IDE、内网环境或旧版 VS Code）中，我们经常需要手动下载插件的 `.vsix` 文件进行离线安装。官方市场虽然提供了 Version History，但下载路径往往隐藏较深或需要手动拼接 URL，操作繁琐。

图来源于trae官方文档从 VS Code 的插件市场安装

![image-20251226221701073](.\trae%E5%AE%98%E6%96%B9%E6%96%87%E6%A1%A3%E4%BB%8E%20VS%20Code%20%E7%9A%84%E6%8F%92%E4%BB%B6%E5%B8%82%E5%9C%BA%E5%AE%89%E8%A3%85.png)

本脚本通过在页面注入快捷按钮，完美解决了这一痛点。



## ✨ 主要功能

- **🚀 一键下载最新版**：
  在插件详情页面的 Install 按钮旁添加醒目的 **"最新版 vX.X.X"** 按钮，点击即可直接获取当前最新 `.vsix` 文件。

- **📜 历史版本直链**：
  自动将 **Version History** 列表中的纯文本版本号转换为**直接下载链接**。无需跳转，点击版本号即可下载对应历史版本。

- **⚡ 高效便捷**：
  自动解析 `publisher`、`extension name` 和 `version`，按照官方 API 规则生成下载地址，安全可靠。

## 🛠️ 安装指南

1. **安装管理器**：首先确保您的浏览器已安装 [Tampermonkey](https://www.tampermonkey.net/) (油猴) 扩展。
2. **安装脚本**：
   - 点击 [此处安装脚本](#) (如果有发布链接)
   - 或者新建脚本，将 `vscode_marketplace_downloader.user.js` 的内容复制进去并保存。

## 📖 使用说明

1. 打开 [VS Code Marketplace](https://marketplace.visualstudio.com/) 网站。
2. 搜索并进入任意插件的详情页面（例如 Python, Vue 等）。
3. **下载最新版**：点击标题区域红色的 **"最新版 v..."** 按钮。
4. **下载历史版**：点击 **Version History** 选项卡，直接点击列表中的 **版本号** 链接。
5. 将下载好的 `.vsix` 文件拖入 IDE (如 VS Code 或 Trae) 即可完成安装。

## 🤝 贡献

欢迎提交 Issue 或 Pull Request 来改进此脚本！

## 📄 开源协议

本项目遵循 [MIT License](LICENSE) 开源协议。
