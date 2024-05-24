# CS2 Config Backup

This is my usual CS2 configuration setting, just for backup.

## Preset

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

## Game Launch Parameters

`-fullscreen -high -console -nohltv -novid -nojoy -freq 165 -allow_third_party_software`

## Load CFG

将 cs2 文件夹内容复制到 `C:\Program Files (x86)\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\` 目录下。

`autoexec.cfg` 会在游戏启动时自动加载。
