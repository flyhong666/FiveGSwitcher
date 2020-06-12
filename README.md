# FiveGSwitcher

### 温馨提示

最新版本已在[酷安](https://www.coolapk.com/apk/280295)认领并发布。

若无法正常安装，可下载[备份版本](https://www.coolapk.com/apk/288773)。

### 通知栏增加5G开关

在通知栏编辑模式中长按“5G开关”拖动到上方即可使用，弥补5G手机没有快捷开关的问题。

### 支持ADB Shell命令

方便ROOT权限的设备运行自动化脚本。[issue#2](https://github.com/ysy950803/FiveGSwitcher/issues/2)

```shell
# 开启5G，关闭则为false
am start -n com.ysy.fivegswitcher/.MainActivity --ez enable_5g true
```

### FAQ

**0、其他厂商ROM可以使用吗？**

此工具只能MIUI系统使用哦，谢谢各位的支持。

**1、添加开关后不可用（灰色状态）？**

目前发现在MIUI 12和12.5稳定版部分机型上有这个问题，会导致快捷方式TileService被系统杀死并重启（我尝试了MIUI开发版和原生Android就不会），暂时没有百分百的解决办法。可尝试开启本应用的自启动权限，并重新添加快捷开关到你通知中心的第一页（即下拉后第一眼就能看见的位置），最后重启手机。

**2、点击开关后，图标状态没有改变（没反应）或者很久才响应？**

问题本质同1。

**3、长按5G开关后，无法跳转到设置页面？**

请在应用的权限设置中允许后台弹出界面或开启自启动。
