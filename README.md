# dingtalk-auto-clock

## 📖 简介

基于auto.js和[DingDing-Automatic-Clock-in](https://github.com/georgehuan1994/DingDing-Automatic-Clock-in)的钉钉全自动打卡脚本
支持日历定时打卡以及QQ远程打卡

## 📐 工具介绍

### Auto.js

Auto.js 是利用安卓系统的 「无障碍服务」 实现类似于按键精灵一样，可以通过代码模拟一系列界面动作的辅助工具。

与 「按键精灵」 不同的是，它的模拟动作并不是简单的使用在界面定坐标点来实现，而是找控件来实现的。

免费版：[Auto.js 4.1.1a Alpha2-armeabi-v7a-release](https://github.com/georgehuan1994/DingDing-Automatic-Clock-in/raw/master/Autojs%204.1.1a%20Alpha2-armeabi-v7a-release.apk "Auto.js 4.1.1a Alpha2-armeabi-v7a-release")

github：[GitHub - hyb1996/Auto.js](https://github.com/hyb1996/Auto.js)

官方文档：[首页 - Auto.js](https://hyb1996.github.io/AutoJs-Docs/)

推荐使用[VS Code 插件](https://github.com/hyb1996/Auto.js-VSCode-Extension)进行调试，调试完成后，还能通过此插件将脚本保存到手机上。

## 🕹️ 使用方法

### 远程打卡

- 向本机的 QQ 发送消息 「打卡」
- 向本机的 QQ 发送消息 「查询」

### 暂停/恢复定时打卡

- 向本机的 QQ 发送消息 「暂停」
- 向本机的 QQ 发送消息 「恢复」

### 代码修改

- 钉钉账号和密码可填可不填，填了账号和密码支持钉钉自动登录。
- 发送反馈消息的QQ和邮箱最好填上，不然接收不到反馈消息。
- 默认QQ模式，可改成邮箱模式。
- 熄屏快捷键每个手机不一样，代码中以小米手机长按home键为主。


## ⚠️ 注意事项 (必读!!!)

- AutoJs Pro 版本屏蔽了一些主流应用，如果要使用 QQ 作为回复方式，不要使用 AutoJs Pro 版！
- 首次启动 AutoJs，需要为其开启无障碍权限。
- 运行脚本前，请在 AutoJs 菜单栏中（从屏幕左边划出），开启 「通知读取权限」。
- 若无法通过 `app.launchPackage()` 方法启动应用，请开启该应用的「自启动」「允许后台弹窗」。
- AutoJs 可息屏运行，需要在系统设置中开启通知亮屏。
- 为保证 AutoJs 进程不被系统清理，可调整它们的电池管理策略、加入管理应用的白名单，为其开启前台服务、添加应用锁...
- 虽然脚本可执行完整的打卡步骤，但推荐开启钉钉的极速打卡功能，在钉钉启动时即可完成打卡，应把后续的步骤视为极速打卡失败后的保险措施。
