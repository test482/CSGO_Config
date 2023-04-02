# CSGO Config Backup

This is my usual CSGO configuration setting, just for backup.

## 预设置

- Windows 10 **关闭 XBOX DVR**

直接导入下面的注册表文件：

```text
Windows Registry Editor Version 5.00
[HKEY_CURRENT_USER\System\GameConfigStore]
"GameDVR_Enabled"=dword:0
[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Windows\GameDVR]
"AllowGameDVR"=dword:0
[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\PolicyManager\default\ApplicationManagement\AllowGameDVR]
"value"=dword:0
```

- Windows 10 **禁用全屏优化**：右键 “属性” —— “兼容性” —— 勾选 “禁用全屏优化”

- Windows 10 设置 —— 轻松使用 —— 关闭『允许使用快捷键启动粘滞键』、『允许使用快捷键启动筛选键』

- **NVIDIA 显卡设置**（可参考[此篇文章](https://www.wevg.org/archives/csgo-fps-optimized/)）

- Realtek 音频管理器**关闭耳机虚拟化**

## 启动参数

`-novid -nojoy -tickrate 128 +exec auto`

> `-perfectworld` 进入完美国服
>
> `-refresh 144 -freq 144` 强制游戏的刷新率，取决于你的显示器刷新率
>
> `+fps_max XXX` (1-999) 修改你的 FPS 上限
>
> `-disable_d3d9ex` 这个参数可以修复 amd 显卡用户加载地图时候卡在 retrieving server info（接受服务器信息）很长一段时间的问题；但是，似乎会导致游戏开局几回合有轻微卡顿，以及 alt + tab 切屏后卡顿一段时间。有部分[社区用户报告](https://www.reddit.com/r/csgo/comments/kv0q2d/csgo_stuck_on_retrieving_server_info_after/)该选项可能会导致偶发闪退（为了避免闪退似乎需要将某个材质选项设置为低）

## 加载 cfg

将 cfg 文件夹内容复制到 Steam\\userdata\\**Your_USER_ID**\\730\\local\\cfg 目录下。

添加 `+exec auto` 启动参数或者在游戏内控制台输入 `exec auto`。
