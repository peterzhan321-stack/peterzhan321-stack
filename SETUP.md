# 🚀 部署指南

## 一键部署到 GitHub

### 第一步：创建 GitHub 仓库

你需要创建一个**和你 GitHub 用户名同名**的特殊仓库：

1. 去 https://github.com/new
2. 仓库名填：`peterzhan321-stack`（必须和你的用户名完全一致）
3. 选择 **Public**
4. ✅ 勾选 "Add a README file"
5. 点击 **Create repository**

### 第二步：初始化 Git 并推送

```bash
# 进入项目目录
cd C:\Users\21649\Desktop\github-profile

# 初始化 git
git init

# 添加远程仓库（替换成你自己的用户名）
git remote add origin https://github.com/peterzhan321-stack/peterzhan321-stack.git

# 添加所有文件
git add .

# 提交
git commit -m "✨ feat: awesome GitHub profile README"

# 推送（如果已有 README.md，先 force push）
git branch -M main
git push -u origin main --force
```

### 第三步：启用 GitHub Pages（可选）

如果你的仓库不是 public，或者想用自定义域名：

1. 去仓库 Settings → Pages
2. Source 选择 `main` 分支
3. 保存

### 第四步：等待 GitHub Actions

- 贡献蛇动画会在第一次推送后自动生成
- 如果看不到蛇动画，去仓库的 **Actions** 标签页，手动触发一次 `snake.yml` workflow

---

## 🎨 自定义修改

### 更改名字
在 README.md 中搜索 `peter`，替换成你想要的名字。

### 更改技术栈徽章
在 `## 🛠️ Tech Stack` 部分，修改 badge：

```html
<img src="https://img.shields.io/badge/-语言-颜色?style=for-the-badge&logo=logo&logoColor=white" />
```

可用的 logo 参考：https://simpleicons.org/

### 更改颜色主题
README 中使用的是 **Tokyo Night** 主题（深蓝色调）。如果想换成其他主题：

| 主题名 | 适用组件 |
|--------|----------|
| `tokyonight` | GitHub Stats, Trophies |
| `radical` | Activity Graph |
| `dracula` | 随机引言 |

### 添加新板块
在 README.md 中合适的位置添加 Markdown 内容即可。

---

## 📝 更新日志

- 2026-06-28: 初始创建，包含所有炫酷效果
