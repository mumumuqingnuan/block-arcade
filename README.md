# 方块时光 · 俄罗斯方块

传统经典、霓虹光影双模式，支持电脑键盘与手机触屏。

## 怎么玩

- 点「开始游戏」。电脑用方向键移动、旋转，空格落底，P 暂停。
- 手机上点棋盘下方的「左移」「旋转」「右移」「下落」「落到底」。
- 点「大屏显示」放大棋盘，点「返回普通显示」退出。
- 音乐需要先点击开始游戏才能播放，可在「声音与动效」中关闭。

进度和声音设置自动保存在本设备、本浏览器。重新打开同一链接后，点「继续游戏」。传统与霓虹的进度分别保存。更换设备、浏览器或清除网站数据后无法恢复原存档；原 Sites 链接的存档不会自动迁移。

## 添加到手机或电脑桌面

使用浏览器打开 https://mumumuqingnuan.github.io/block-arcade/ 。

- 游戏顶部的「添加到桌面」会显示对应设备的步骤，也可切换查看全部设备。打开说明会暂停并保存游戏；关闭后手动继续。
- 安卓手机 / 平板：Chrome → ⋮ → 安装并创建快捷方式 → 安装；部分版本显示「添加到主屏幕」。
- iPhone / iPad：Safari → 分享 / 共享 → 添加到主屏幕 → 添加；如有「作为网页 App 打开」，将它打开。
- Windows：Edge / Chrome 安装网页应用，再在 edge://apps 或 chrome://apps 中创建桌面快捷方式。
- Mac：Safari → 分享 → 添加到程序坞（macOS 14+）；Chrome 也可安装网页应用，并通过 chrome://apps 创建快捷方式。
- 浏览器支持安装提示时，说明中会显示「在这台设备上安装」按钮。没有该按钮时，仍可按对应设备步骤操作。

添加时会使用「方块时光」名称和方块图标。浏览器的菜单名称可能不同，网站不能自行把图标放到桌面。首次添加需手动确认；本版本未提供离线网页缓存。

桌面应用与普通浏览器可能使用独立存档，建议添加后固定从同一个图标打开。

官方操作说明：[安卓 Chrome](https://support.google.com/chrome/answer/9658361?co=GENIE.Platform%3DAndroid&hl=zh-Hans)、[电脑 Chrome](https://support.google.com/chrome/answer/9658361?co=GENIE.Platform%3DDesktop&hl=zh-Hans)、[iPhone Safari](https://support.apple.com/zh-cn/guide/iphone/iphea86e5236/ios)、[Mac Safari](https://support.apple.com/guide/safari/add-to-dock-ibrw9e991864/mac)、[Microsoft Edge](https://support.microsoft.com/en-us/edge/install-manage-or-uninstall-apps-in-microsoft-edge)。

## 托管

此目录是完整静态网站，无需登录、API 密钥或后端服务。GitHub Pages 可选择 main 分支的根目录发布。

## 源文件

`source.zip` 包含可编辑源码、依赖锁文件和测试，不包含账号凭据或玩家存档。解压后使用 Node.js 22.13+ 和 pnpm：

```sh
pnpm install --frozen-lockfile
pnpm test
pnpm run build
```

将生成的 `dist/` 内容放入网站根目录即可。样式和玩法来自原站点 https://block-arcade.wendyrh.chatgpt.site/ ，迁移版使用本机存档。
