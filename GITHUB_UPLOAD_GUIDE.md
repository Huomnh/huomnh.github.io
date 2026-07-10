# GitHub 上传使用文档

这份文档适用于将这个 Astro 博客项目上传到 GitHub，并进行基础的版本管理与部署准备。

项目基于 Astro + Svelte + TypeScript，依赖管理使用 pnpm。上传前请确保本地环境已经准备好。

---

## 1. 环境准备

请先确认你的电脑已经安装以下内容：

- Git
- Node.js 22+
- pnpm 9+

### 检查版本

```bash
git --version
node -v
pnpm -v
```

如果没有安装 pnpm，可以执行：

```bash
npm install -g pnpm
```

---

## 2. 进入项目目录

如果你已经在项目根目录中，可以直接跳过这一步。否则执行：

```bash
cd 你的项目目录
```

例如：

```bash
cd e:\Huomnh博客\Astro\huomnh.github.io
```

---

## 3. 安装依赖

在项目根目录执行：

```bash
pnpm install
```

这个项目的安装脚本会强制使用 pnpm，因此请不要使用 npm 安装。

---

## 4. 本地验证项目

安装完成后，建议先在本地运行一次检查，确保项目可以正常启动：

```bash
pnpm check
pnpm type-check
pnpm build
```

如果你想先预览网站，可以运行：

```bash
pnpm dev
```

然后在浏览器打开：

```text
http://localhost:4321
```

---

## 5. 初始化 Git 仓库（如果还没有）

如果这个项目还没有初始化为 Git 仓库，请执行：

```bash
git init
git branch -M main
```

如果你已经有 Git 仓库，跳过这一步即可。

---

## 6. 添加并提交代码

先查看当前修改内容：

```bash
git status
```

添加所有文件：

```bash
git add .
```

提交：

```bash
git commit -m "chore: init project"
```

你也可以使用更清楚的提交信息，例如：

```bash
git commit -m "feat: initialize firefly blog"
```

---

## 7. 创建 GitHub 仓库

在 GitHub 网页上操作：

1. 登录 GitHub
2. 点击右上角的 “+”
3. 选择 “New repository”
4. 填写仓库名称，例如：
   - `huomnh-blog`
   - `firefly-site`
5. 选择公开或私有
6. 点击 “Create repository”

---

## 8. 关联本地仓库到 GitHub

将本地仓库与 GitHub 仓库连接：

```bash
git remote add origin https://github.com/你的GitHub用户名/你的仓库名.git
```

例如：

```bash
git remote add origin https://github.com/yourname/firefly-site.git
```

如果之前已经添加过远程仓库，可以先查看：

```bash
git remote -v
```

然后更新为新的地址：

```bash
git remote set-url origin https://github.com/你的GitHub用户名/你的仓库名.git
```

---

## 9. 推送到 GitHub

第一次推送：

```bash
git push -u origin main
```

之后再更新时：

```bash
git add .
git commit -m "update: modify content"
git push
```

---

## 10. 可选：部署到 GitHub Pages

如果你想把这个站点部署到 GitHub Pages，可以参考下面的思路：

1. 在 GitHub 仓库设置中开启 Pages
2. 选择部署来源为 GitHub Actions 或分支
3. 如果使用静态站点，通常需要额外配置构建流程

注意：这个项目本身是 Astro 项目，直接部署到 GitHub Pages 需要额外配置构建脚本或使用其他托管平台（如 Vercel、Cloudflare Pages、Netlify）会更省事。

如果你想要，我也可以继续帮你补一份“适用于这个项目的 GitHub Pages 部署配置文档”。

---

## 11. 常见问题

### 1）提示 pnpm 不是命令

执行：

```bash
npm install -g pnpm
```

### 2）依赖安装失败

清理缓存后再试：

```bash
pnpm store prune
pnpm install
```

### 3）Git 提示身份未配置

```bash
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
```

### 4）push 时报错认证失败

GitHub 现在通常需要使用个人访问令牌（PAT）而不是直接密码。你可以在 GitHub 设置中生成 token，然后使用它替代密码进行认证。

---

## 12. 推荐的最小上传流程

如果你只是想快速上传到 GitHub，按下面顺序即可：

```bash
pnpm install
pnpm build
git init
git branch -M main
git add .
git commit -m "chore: upload project"
git remote add origin https://github.com/你的GitHub用户名/你的仓库名.git
git push -u origin main
```

---

## 13. 说明

这个项目包含较多静态资源、配置文件和生成文件，建议上传前确认以下内容：

- 你不需要把本地依赖目录提交到 Git
- 生成出来的构建产物通常不需要手动提交
- 如果你有敏感信息，请不要提交到仓库中

如果你后续想把这个项目发布到 GitHub 并且顺便配置自动部署，我也可以继续帮你把相关步骤补完整。