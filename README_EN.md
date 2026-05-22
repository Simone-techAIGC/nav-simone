# 🚀 Simone Nav

A personalized bookmark management and static navigation system deeply customized based on [liuzi6612/nav](https://github.com/liuzi6612/nav).

![Build Status](https://img.shields.io/github/actions/workflow/status/YOUR_USERNAME/YOUR_REPO/build-web.yml?branch=main&label=Build%20Status&style=flat-square)
![License](https://img.shields.io/github/license/YOUR_USERNAME/YOUR_REPO?style=flat-square)

## 🌟 Introduction

**Simone Nav** is dedicated to collecting and organizing high-quality resources in the digital age. Forked from a popular open-source navigation framework, this project leverages GitHub Actions for automated deployment, aiming to create a minimalist, clean, and efficient resource index.

### 📂 Core Categories
- 💻 **Cutting-edge Tech**: Computer Science, Internet, Tech Trends, AI, and Vibecoding.
- 👨‍💻 **Developer Hub**: Programming tutorials, Code practices, and Open-source projects.
- 📢 **Digital Marketing**: Self-media operations, Short videos, Advertising, and Growth hacking.
- 📖 **Deep Reading**: Book sharing, Reading notes, Knowledge base construction, and Productivity.
- 🔓 **Open Source & Resources**:
  - **Learning**: Papers, E-books, Educational videos, and Audio courses.
  - **Productivity**: Career resources, Software, Mobile Apps, Browser Extensions, and Tools.
  - **Media**: Global movie/TV resources and interest communities.

---

## 🛠 Key Features

- **CI/CD Pipeline**: Fully automated build process via GitHub Actions whenever `db.json` or `bookmarks.html` is updated.
- **Data-Driven Rendering**: The UI is dynamically generated based on `data/db.json`.
- **Easy Import**: Supports batch converting browser-exported HTML bookmarks into navigation items.
- **Responsive Design**: Optimized for PC, Tablet, and Mobile devices.

---

## 🚀 Getting Started

### 1. Adding Resources
All data is stored in `data/db.json`. Follow this format to add new items:
```json
{
  "category": "Computer Science",
  "links": [
    {
      "name": "Example Site",
      "url": "https://example.com",
      "desc": "Site description goes here",
      "icon": "https://example.com/favicon.ico"
    }
  ]
}
```

### 2. Batch Import
1. Place your `bookmarks.html` in the root directory.
2. Run the import script to parse and update `db.json`.
3. Push changes: `git add . && git commit -m "Update links" && git push`.

---

## ⚙️ Build & Maintenance

This project uses GitHub Actions for deployment.

- **Auto Build**: Every push to the `main` branch triggers the `Build web` workflow.
- **Count Synchronization**: If the displayed item count differs from the statistics, check if your `db.json` nesting exceeds two levels. Flat structures are recommended for optimal performance.

---

## 📂 Project Structure

```text
.
├── .github/workflows/   # CI/CD workflows
├── data/                # Core database (db.json)
├── public/              # Static assets
├── scripts/             # Parsing and stat scripts
├── index.html           # UI Template
└── README.md            # Project documentation
```

---

## 🤝 Acknowledgments

- Special thanks to the original project [liuzi6612/nav](https://github.com/liuzi6612/nav).

---
*Powered by Simone | Stay Curious, Stay Learning.*
