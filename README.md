# 电子信封（NFC/手机可打开）

这是一个**单文件静态网页**，用于展示带开合动画的“电子信封”。你可以把它部署到 GitHub Pages，然后把生成的网址写入 NFC 标签里，手机碰一下即可跳转打开。

## 快速开始（GitHub Pages 部署）

1. 登录 GitHub，右上角点击 **New repository** 新建仓库，建议仓库名：`love-envelope`（或任意你喜欢的名字）。
2. 创建后在仓库页面点击 **Add file → Upload files**，将 `index.html` 上传（本项目只有这一个文件）。
3. 打开仓库的 **Settings → Pages**：
   - 在 **Build and deployment** 将 **Source** 设为 **Deploy from a branch**；
   - 在 **Branch** 选择 `main` 分支，**/ (root)**；点击 **Save**。
4. 等待 30 秒～2 分钟，GitHub 会给出你的网站地址，形式通常是：  
   `https://你的GitHub用户名.github.io/仓库名/`
5. 把这个地址写入 NFC 标签即可。

> 提示：以后想修改信的内容，只需要在 GitHub 网页端直接编辑 `index.html` 并保存即可，几秒钟后页面会自动更新。

## 本地预览
直接双击打开 `index.html` 即可（推荐用手机浏览器或在桌面浏览器开启移动端预览）。

## 个性化
- 改页面标题与副标题：在 `<head>` 的 `<title>` 和 `<meta name="description">` 修改。
- 主题与配色：在 `<style>` 里的 `:root` CSS 变量调整颜色。
- 默认深色模式已适配；喜欢纯浅色可删掉 `@media (prefers-color-scheme: dark)` 块。
- 若希望打开页面就自动展开信封，可把地址加上 `#open`（例如 `.../index.html#open`）。

祝告白顺利 ❤️
