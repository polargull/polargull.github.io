# 付玮 · 个人简历站

单文件静态简历网站（`index.html`），无构建工具、无外部依赖，可直接部署到 GitHub Pages 和 Gitee Pages。

## 本地预览

直接双击 `index.html` 用浏览器打开即可。

## 部署到 GitHub Pages

1. 在 GitHub 创建仓库，仓库名为 `你的用户名.github.io`（这样站点地址就是 `https://你的用户名.github.io`）。
2. 把 `index.html` 推送到仓库 main 分支：
   ```bash
   git init
   git add index.html README.md
   git commit -m "init: personal resume site"
   git branch -M main
   git remote add origin https://github.com/你的用户名/你的用户名.github.io.git
   git push -u origin main
   ```
3. 进入仓库 Settings → Pages，Source 选择 `Deploy from a branch`，Branch 选择 `main` / `(root)`，保存。
4. 等待 1–3 分钟，访问 `https://你的用户名.github.io`。

## 复制一份到 Gitee

1. 在 Gitee 新建同名仓库 `你的用户名`（Gitee Pages 要求仓库即用户名）。
2. 推送同样内容：
   ```bash
   git remote add gitee https://gitee.com/你的用户名/你的用户名.git
   git push gitee main
   ```
3. 进入 Gitee 仓库 → 服务 → Gitee Pages，部署分支选 `main`，目录选 `/`，点击启动。按当前政策部分功能可能需要实名认证，以 Gitee 最新说明为准。

## 部署后建议更新

- `index.html` 中邮箱已是求职邮箱 `457995133@qq.com`；如需加 GitHub / 博客链接，编辑 `<section id="contact">` 一节。
- Agent 作品集三个项目的状态标签（`计划中` / `进行中` / `已完成`）在 `#agents` 区块内，完成后把状态改为 `status-done` 并补上仓库链接。
- 页脚年份在 `2026` 处，按需更新。
