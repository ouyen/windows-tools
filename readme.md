# windows tools

## 设置windows时间与linux双系统时间一致

+ windows下运行`在 Windows 上设置硬件时间为 UTC.bat`  （管理员）即Powershell（管理员）中执行

```
reg add "HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\TimeZoneInformation" /v RealTimeIsUniversal /d 1 /t REG_QWORD /f
```

+ Linux： sudo timedatectl set-local-rtc 0

## 解除uwp应用locolhost限制

> 使得uwp应用可以访问locolhost（比如Unigram可以使用本地代理）

## 右键菜单（适用于win11）

> 将右键菜单还原到win10（旧版）

## kms激活 by [沧水](https://kms.cangshui.net)

> 激活windows & office

## [Wu10Man_Portable](https://github.com/WereDev/Wu10Man)

> 禁用/恢复 windows更新

## [MediaCreationTool.bat](https://github.com/AveYo/MediaCreationTool.bat)

> 更新win11绕过tpm限制

## 制作win11 iso镜像

~~编辑 Windows 10 的 ISO 文件，删除 sources 文件夹下的 install.wim，然后将 Windows 11 的 install.esd 添加到该文件夹，保存（另存为）ISO 文件即可。~~

使用上面的## [MediaCreationTool.bat](https://github.com/AveYo/MediaCreationTool.bat) ，拖动win11.iso到bypass11/Quick_11_iso_esd_wim_TPM_toggle.bat上即可