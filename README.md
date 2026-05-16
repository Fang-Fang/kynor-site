# Kynor GitHub Pages Static Website

这是一个可直接部署到 GitHub Pages 的静态品牌官网首页。

## 文件
- `index.html`：网站首页
- `styles.css`：全部样式

## 部署到 GitHub Pages
1. 新建 GitHub 仓库，例如 `kynor-site`
2. 上传本文件夹里的 `index.html` 和 `styles.css`
3. 进入仓库 Settings → Pages
4. Source 选择 `Deploy from a branch`
5. Branch 选择 `main` / root
6. 保存后等待 GitHub 生成网址

## 绑定域名 kynor.shop
1. 在 GitHub Pages 的 Custom domain 填写 `kynor.shop`
2. 在阿里云域名 DNS 添加记录：
   - `CNAME`：`www` → `你的GitHub用户名.github.io`
   - 根域名 `@` 可用 A 记录指向 GitHub Pages 官方 IP
3. 勾选 Enforce HTTPS

## 替换图片
当前版本使用 CSS 绘制产品占位图，不依赖图片文件。后续可把产品图放到 `assets/`，再替换 HTML 中 `.product-image` 区块。
