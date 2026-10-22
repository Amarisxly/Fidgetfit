# FidgetFit 轻弹玩家 · PWA

## 文件
- `index.html` — App 本体
- `manifest.webmanifest` — 应用名称、图标、全屏显示、长按图标的快捷方式
- `sw.js` — 离线缓存：首次打开后断网也能用
- `icons/` — 主屏幕图标（含 Android 自适应图标和 iPhone 图标）

## 中英文切换
- 首页右上角「中 / EN」，或「我的 → App → 语言 · Language」。
- 选择会记在本机，下次打开保持；首次打开时跟随手机系统语言。
- 动作库搜索支持中英文关键词（如「颈」或 neck）。

## 上线（任选一种，都免费）
PWA 必须通过 https 访问才能安装，双击本地文件只能预览，不能安装。

1. **Netlify Drop**：打开 app.netlify.com/drop，把整个 `fidgetfit-pwa` 文件夹拖进去，得到一个 https 链接。
2. **Vercel**：新建项目，上传这个文件夹，框架选 Other。
3. **GitHub Pages**：把文件夹内容推到仓库，在 Settings → Pages 打开。

## 安装到手机
- **iPhone**：用 Safari 打开链接 → 分享 → 添加到主屏幕。
- **Android**：用 Chrome 打开链接 → 页面里「我的 → 安装」，或浏览器菜单「安装应用」。
- **电脑**：Chrome / Edge 地址栏右侧的安装图标。

## 更新版本
改完 `index.html` 后，把 `sw.js` 第一行的 `VERSION` 改个数字（如 `fidgetfit-v2`），用户下次打开会自动拿到新版。当前版本：`fidgetfit-v7`（中英文切换、每个动作的专属小人姿势、每日真实打卡、动作结束震动、可延长时间）。

如果你已经部署在 Vercel（如 fidgetfit.vercel.app），把这个文件夹重新上传/推送一次即可更新。
