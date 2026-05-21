# 🚀 Simone 导航站

一个基于 [liuzi6612/nav](https://github.com/liuzi6612/nav) 深度定制的个性化书签管理与静态导航系统。

![Build Status](https://img.shields.io/github/actions/workflow/status/YOUR_USERNAME/YOUR_REPO/build-web.yml?branch=main&label=Build%20Status&style=flat-square)
![Stars](https://img.shields.io/github/stars/YOUR_USERNAME/YOUR_REPO?style=flat-square)

## 🌟 站点简介

**Simone 导航站** 致力于收集和整理数字化时代的优质资源。本项目复刻自知名开源导航项目，通过 GitHub Actions 自动化构建，旨在打造一个极简、纯净、高效的资源索引中心。

### 📂 核心收录领域
- 💻 **技术前沿**：计算机科学、互联网、硬核科技、AI 人工智能、Vibecoding。
- 👨‍💻 **开发者之路**：编程学习、代码实践、开源项目。
- 📢 **数字营销**：自媒体运营、新媒体、短视频、广告营销、流量变存。
- 📖 **深度阅读**：书籍资源分享、读后感记录、笔记管理、知识库搭建。
- 🔓 **开源共享**：
  - **学习资源**：论文、电子书、教学视频、音频课。
  - **生产力工具**：职场资源、软件、移动端 App、浏览器插件、在线工具。
  - **影音娱乐**：国内外优质影视资源、兴趣社群。

---

## 🛠 核心功能

- **自动化流水线**：基于 GitHub Actions，修改 `db.json` 或 `bookmarks.html` 后自动触发构建。
- **数据驱动渲染**：前端页面根据 `data/db.json` 自动生成分类和卡片。
- **书签一键导入**：支持将浏览器导出的 HTML 书签文件批量转化为导航条目。
- **响应式布局**：完美适配 PC、平板与手机端，随时随地查阅资源。

---

## 🚀 快速上手

### 1. 资源添加与修改
所有数据存放在 `data/db.json`。按照以下格式添加新资源：
```json
{
  "category": "计算机",
  "links": [
    {
      "name": "示例网站",
      "url": "https://example.com",
      "desc": "这是一个网站描述",
      "icon": "https://example.com/favicon.ico"
    }
  ]
}
```

### 2. 批量导入书签
1. 将浏览器导出的 `bookmarks.html` 放入仓库。
2. 运行脚本解析书签并更新 `db.json`。
3. 提交代码：`git add . && git commit -m "Update links" && git push`。

---

## ⚙️ 构建与维护

本项目使用 GitHub Actions 进行部署。

- **自动构建**：每次 Push 到 `main` 分支都会触发 `Build web`。
- **统计同步**：若发现页面展示数量与统计不符，请检查 `db.json` 中的嵌套层级是否过深，建议保持在两层以内以获得最佳展示效果。

---

## 📂 目录结构

```text
.
├── .github/workflows/   # 自动化部署工作流
├── data/                # 核心数据库 (db.json)
├── public/              # 静态资源文件
├── scripts/             # 书签解析、统计、数据处理脚本
├── index.html           # 导航站模板
└── README.md            # 项目说明文档
```

---

## 🤝 鸣谢

- 感谢项目原型 [liuzi6612/nav](https://github.com/liuzi6612/nav) 提供的优秀框架。

---
*Powered by Simone | 持续收集，终身学习。*
