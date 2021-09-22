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

> ~~-perfectworld  进入完美国服~~
>
> -refresh 144 -freq 144  强制游戏的刷新率，取决于你的显示器刷新率
>
> +fps_max XXX (1-999)  修改你的 FPS 上限

## 加载 cfg

将 cfg 文件夹内容复制到 Steam\\userdata\\**Your_USER_ID**\\730\\local\\cfg 目录下。

添加 `+exec auto` 启动参数或者在游戏内控制台输入 `exec auto`。
