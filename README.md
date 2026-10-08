# 一餐一记

适合手机屏幕的吃饭记账网页。可以上传照片、标注金额、编辑记录和统计花费。

无需登录和后端。账目与照片保存在当前设备当前浏览器的 IndexedDB 中，不上传到 GitHub。

## 发布到 GitHub Pages

1. 新建公开仓库，例如 `meal-diary`。
2. 将本目录的 `index.html`、`.nojekyll` 和 `README.md` 上传到仓库根目录。
3. 仓库 Settings → Pages → Build and deployment，选择 Deploy from a branch。
4. 选择 `main` 分支和 `/ (root)`，点击 Save。
5. 等待 Pages 显示发布成功，使用该页面提供的实际网址。通常是 `https://你的用户名.github.io/meal-diary/`，此示例不是已发布地址。

GitHub Pages 官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

## 国内访问

GitHub Pages 不保证中国大陆各网络稳定访问。需要提供稳定的国内入口时，可将同一份 index.html 部署到国内静态托管服务，按服务商要求准备域名、备案及 HTTPS。源码仍可由 GitHub 管理。

## 数据注意事项

- 同一手机不同浏览器的数据互不相通，更换网站域名也不会自动迁移数据。
- 清理网站数据、卸载浏览器或系统回收存储可能导致记录丢失，请定期使用页面的备份功能。
- 从原网址迁移时，先在原网址备份，再在新网址恢复。
- 不要向公开仓库上传个人账本备份或照片。
- 尚未在 iOS/Android 微信真机验证存储持久化、图片选择及备份下载。
