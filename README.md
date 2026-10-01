# 正则实验室

简洁的中文 JavaScript 正则表达式测试工具。无需安装依赖，可直接打开 `index.html`，也可通过 GitHub Pages 发布。

在线使用：https://cj8631.github.io/regex-tester/

- 实时匹配高亮、匹配位置与捕获组详情。
- 暖白与墨绿配色，支持明暗主题切换和手机布局。
- 随输入更新的中文语法注释。
- 替换预览、常用示例和语法速查。
- 正则在 Web Worker 中执行，超过 2 秒自动停止。
- 测试文本在浏览器内处理，不上传、不持久保存。

## 发布到 GitHub Pages

1. 登录 [GitHub](https://github.com)，创建公开仓库，建议名称为 `regex-tester`。
2. 在仓库的文件页面选择 **Add file → Upload files**。空仓库可点击 **uploading an existing file**。
3. 上传本文件夹中的 `index.html` 和 `README.md`，以及 `.nojekyll`（若文件选择器可见），点击 **Commit changes**。`index.html` 必须位于仓库根目录，不要把外层 `regex-tester-site` 文件夹一起上传。
4. 打开仓库 **Settings → Pages**。
5. 在 **Build and deployment** 中，将 **Source** 设为 **Deploy from a branch**。
6. 将 **Branch** 设为 **main**，目录设为 **/(root)**，点击 **Save**。如果提交所在分支名称不同，选择实际分支。
7. 等待部署完成，刷新 Pages 设置页，点击 **Visit site**。通常需要几分钟，部署进度可在 **Actions** 查看。

网站地址通常是 `https://你的GitHub用户名.github.io/regex-tester/`，实际地址以 Pages 设置页显示的链接为准。其他人打开网站不需要 GitHub 账号。

`.nojekyll` 用于告诉 GitHub Pages 直接发布静态文件；本项目即使只上传 `index.html` 也可以运行。

## 更新网页

本发布目录的 `index.html` 是工作区 `regex-tester.html` 的副本。

修改原文件后，先用更新后的内容覆盖本目录的 `index.html`，再上传到同一个 GitHub 仓库并提交。GitHub Pages 会自动重新部署。

本项目不需要本地 Web 服务器持续运行，也不需要电脑保持开机。
