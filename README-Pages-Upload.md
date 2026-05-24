# Cloudflare Pages 上传说明

这个目录已经是可直接上传到 Cloudflare Pages 的前端发布目录。

目录位置：

`C:\Users\Polaris\Documents\Codex\2026-05-23\new-chat-3\ruoyi-ui-pages-dist`

## 说明

- 不需要 Nginx
- 不需要再执行 `npm build`
- 这个目录已经包含：
  - `index.html`
  - `assets/`
  - `_redirects`

## 如果你走 GitHub + Pages

把这个目录里的内容作为仓库根目录上传。

Pages 配置填写：

- Framework preset：`None`
- Build command：留空
- Build output directory：`/`

## 为什么加 `_redirects`

这是给 Vue3 单页应用用的。

作用是：

- 直接打开子路由不会 404
- 浏览器刷新子页面不会 404
