# 📚 PracticeMaster（刷题助手）

一个纯前端、零依赖的在线刷题工具，支持多种题型（单选、多选、判断、填空、简答），内置 AI 解析、错题强化、模拟测试等功能，题库以 Excel（.xlsx）格式导入即可使用。

## 🚀 在线体验

| 部署平台 | 访问链接 |
|---------|---------|
| **GitHub Pages** | [https://WasteRoadJ.github.io/PracticeMaster/](https://WasteRoadJ.github.io/PracticeMaster/) |
| **教具库** | [https://s.jiaojuku.com/p/nacegq](https://s.jiaojuku.com/p/nacegq) |

> 💡 推荐使用 Chrome、Edge 等现代浏览器打开。

## 📋 测试题库

可直接复制以下 URL 导入题库，体验全部功能：
- https://raw.githubusercontent.com/WasteRoadJ/PracticeMaster/main/测试题库.xlsx

**导入方法**：左侧菜单 → 📥 导入 → 🌐 导入URL题库 → 粘贴上述链接。

## ✨ 功能特性

- **📥 多方式导入**：支持本地 Excel 文件（.xlsx）、加密题库（.enc）、URL 远程题库
- **✏️ 刷题模式**：勾选/填写答案后提交，自动判断对错并记录错题
- **📖 背题模式**：直接显示正确答案与解析，适合快速记忆
- **🎲 顺序/随机切换**：可随时切换题目顺序模式
- **🔥 错题强化**：需连续答对指定次数才能移出错题，巩固薄弱知识点
- **📝 模拟测试**：自定义各题型数量、分值和限时，模拟真实考试环境
- **🤖 AI 解析**：点击 AI 解析按钮，调用在线接口获取题目详解（支持更换 API 地址）
- **⭐ 收藏功能**：收藏重点题目，导航栏金色边框标记，支持导出收藏本
- **🔁 题库转化**：内置提示词，可配合 AI（DeepSeek、豆包等）实现 Word/文本 ↔ Excel 双向转化
- **📤 多格式导出**：支持导出完整题库（含答题进度）、加密题库、错题本、收藏本、打印版
- **🌓 主题切换**：支持浅色/深色/自动（跟随系统）三种主题模式
- **⚡ 快捷键**：数字键 1-8 选择选项，Enter 提交，↑/↓ 切换题目，数字 9 随机跳转

## 🏁 快速开始

### 本地使用

本项目为纯静态 HTML 文件，无需任何构建工具或服务器环境：

1. 下载 `刷题助手.html` 文件
2. 直接用浏览器打开即可使用
3. 导入你的 Excel 题库（.xlsx）开始刷题

### 题库格式要求

题库需为 Excel（.xlsx）格式，支持以下表头（推荐使用在线体验中的导出功能获取模板）：

| 表头 | 说明 |
|------|------|
| 题目内容 | 题目的完整文字 |
| 答案 | 正确答案（单选/多选用数字或字母，判断用 1/2 或正确/错误） |
| 题目类型 | single / multiple / judge / fill / essay |
| 题型分类 | 自定义分类名称 |
| 题目图片 | 可选，图片 URL 或 Base64 编码 |
| 解析 | 可选，题目的详细解析 |
| 选项1~8 | 选项内容（判断题自动补充"正确""错误"） |

支持五种题型：
- **单选题**（single）
- **多选题**（multiple）
- **判断题**（judge）
- **填空题**（fill）
- **简答题**（essay）

### 发布到 GitHub Pages

1. Fork 本项目或将文件上传到你的 GitHub 仓库
2. 进入仓库 → Settings → Pages
3. Source 选择 `main` 分支，根目录 `/ (root)`，保存
4. 稍等片刻即可通过 `https://<你的用户名>.github.io/<仓库名>/` 访问

## 🔧 题库转化（配合 AI 使用）

在「其他 → 题库转化」中提供了完整的提示词，可直接复制到以下 AI 平台使用：

- [DeepSeek](https://chat.deepseek.com/)
- [豆包](https://www.doubao.com/chat/)

支持的转化方向：
- **Word/文本 → Excel**：将 Word 或文本格式的题库转为标准 Excel 题库
- **Excel → Word/文本**：将 Excel 题库转为可打印的 Word 文档格式

> ⚠️ AI 转化结果不能保证百分百正确，转化完成后请务必人工校对。

## 🛠️ 技术栈

- 纯 HTML + CSS + JavaScript
- [Tailwind CSS](https://tailwindcss.com/)（CDN 引入）
- [SheetJS (xlsx)](https://sheetjs.com/)：Excel 文件解析与生成
- [CryptoJS](https://cryptojs.gitbook.io/docs/)：加密题库支持
- [JSZip](https://stuk.github.io/jszip/)：处理 Excel 内嵌图片

## 🤝 致谢

- **原作者**：本项目基于 52pojie 论坛网友发布的「[题库刷题 v5.0](https://www.52pojie.cn/thread-2021709-1-1.html)」二次开发，已获得原作者授权。
- 感谢原作者的开源分享，为本项目奠定了坚实的基础。

## 📄 许可证

本项目采用 MIT 许可证。详见 [LICENSE](LICENSE) 文件。

---

**⭐ 如果这个项目对你有帮助，欢迎点个 Star！**
