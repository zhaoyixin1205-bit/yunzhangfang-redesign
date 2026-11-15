# 云帐房官网改版 · 部署说明

本站为纯静态站点（无后端依赖），可发布到任意静态托管平台，生成对外公开链接。

## 方式一：WorkBuddy 桌面端「发布为应用」
1. 打开 WorkBuddy 桌面端，找到「发布为应用」入口。
2. 选择本文件夹（`yunzhangfang-redesign`）作为发布目录。
3. 语言选「静态 / static」，发布后即可获得 workbuddy 分享链接。

## 方式二：Netlify Drop（最简单，无需 Git）
1. 打开 https://app.netlify.com/drop
2. 把本文件夹直接拖进去。
3. 自动生成 `https://xxxx.netlify.app` 公开链接。
（已内置 `netlify.toml`，无需额外配置。）

## 方式三：Vercel
1. 打开 https://vercel.com/new ，选择「Upload」或导入包含本文件夹的 Git 仓库。
2. Framework 选「Other」，Output Directory 为 `.`。
3. 部署后获得 `https://xxxx.vercel.app` 链接。
（已内置 `vercel.json`。）

## 方式四：GitHub Pages
1. 将本文件夹内容推送到一个 GitHub 仓库。
2. 仓库 Settings → Pages → Source 选 `main` 分支根目录。
3. 获得 `https://<用户名>.github.io/<仓库名>/` 链接。

## 本地预览
直接用浏览器打开 `index.html` 即可；或在本文件夹执行：
`python3 -m http.server 8080` 然后访问 http://localhost:8080

## 文件清单
- index.html / products.html / solutions.html / cases.html / about.html / news.html
- assets/styles.css（设计系统） / assets/app.js（交互）
- netlify.toml / vercel.json（托管配置）
