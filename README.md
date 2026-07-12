# PS Vita 3.74 Japanese PCH-2000 Recovery

使用 QCMA 为日版 PS Vita PCH-2000 准备 3.74 系统恢复文件的资料归档，可用于现有说明中的 `C3-3822-5` 恢复场景。

> [!WARNING]
> 本仓库的 Release 面向日版 PCH-2000。其他区域或型号必须使用对应区域的官方 `psp2-updatelist.xml` 和固件文件，不能直接照搬本包。

## 准备工作

1. 安装 [QCMA 0.4.1](https://github.com/codestation/qcma/releases/download/v0.4.1/Qcma_setup-0.4.1.exe)。
2. 下载 Release 中的 [`PSV374JP.7z`](https://github.com/Electr0Whale/vita-374-jp-recovery/releases/download/backup/PSV374JP.7z)。
3. 将压缩包内容解压到 QCMA 配置的 PS Vita 更新目录。

对于其他区域的设备，需要从 Sony 对应区域的 `psp2-updatelist.xml` 获取三个 `PSP2UPDAT.PUP` 文件，并同步调整 XML 中的本地文件名，避免重名。

## QCMA 设置

- 固件版本填写为 `03.740.000`。
- **不要选中** `Ignore local file psp2-updatelist.xml on update folder`。

![QCMA 3.74 settings](QCMA%20Settings.png)

## 恢复流程

1. 让 PS Vita 进入安全模式。
2. 选择升级系统软件。
3. 连接运行 QCMA 的电脑。
4. 确认设备识别到 3.74 更新文件后继续。
5. 等待升级完成，不要在写入期间断开电源或 USB 连接。

## 来源

本说明整理自时鹏亮的《[PSV 救砖图文教程](https://shipengliang.com/games/psv%e6%95%91%e7%a0%96%e5%9b%be%e6%96%87%e6%95%99%e7%a8%8b.html)》，原页面标注更新时间为 2024-07-05；仓库内容进行了针对现有 Release 的截取和整理。

Sony、PlayStation Vita 和系统固件的权利归各自权利人所有。本仓库不代表 Sony 官方支持。
