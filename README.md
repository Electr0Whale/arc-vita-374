# PS Vita 3.74 Japanese PCH-2000 QCMA Recovery Archive (`arc-vita-374`)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-PlayStation%20Vita%20(PCH--2000)-003791.svg?style=flat-square" alt="Platform">
  <img src="https://img.shields.io/badge/Firmware-3.74%20(03.740.000)-blue.svg?style=flat-square" alt="Firmware">
  <img src="https://img.shields.io/badge/Tool-QCMA%200.4.1-orange.svg?style=flat-square" alt="QCMA">
  <img src="https://img.shields.io/badge/Target%20Region-Japan%20(NTSC--J)-red.svg?style=flat-square" alt="Region">
</p>

使用 QCMA 为日版 PS Vita PCH-2000 准备 3.74 系统恢复与离线更新文件的应急资料归档，适用于解决开机异常、引导丢失及 `C3-3822-5` 故障恢复场景。

A recovery kit archive for restoring Japanese PlayStation Vita PCH-2000 consoles running firmware 3.74 using offline QCMA configuration.

---

> [!WARNING]
> 本仓库之 Release 固件包与更新列表仅适用于 **日版 PCH-2000**。其他区域型号（港版、美版、欧版等）必须获取对应区域官方 `psp2-updatelist.xml` 与匹配固件，不可直接混刷。

---

## 恢复准备与工具

1. **安装传输客户端**：下载并安装 [QCMA 0.4.1](https://github.com/codestation/qcma/releases/download/v0.4.1/Qcma_setup-0.4.1.exe)；
2. **下载恢复固件包**：从本仓库 Release 获取预配好的 [`PSV374JP.7z`](https://github.com/Electr0Whale/arc-vita-374/releases/download/backup/PSV374JP.7z)；
3. **解压部署**：将压缩包内文件解压至 QCMA 设置的 PS Vita 更新目录（Updates 文件夹）。

---

## QCMA 关键参数设置

在 QCMA 的 `Other` / `CMA` 设置标签页中确认：
- **Use this version for updates**：填写为 `03.740.000`
- **严禁勾选** `Ignore local file psp2-updatelist.xml on update folder`（必须优先使用本地更新描述 XML）

<p align="center">
  <img src="QCMA%20Settings.png" alt="QCMA 3.74 settings" width="600">
</p>

---

## 实机救砖与升级流程

1. **进入安全模式**：PS Vita 在关机状态下，同时按住 `电源键` + `PS 键` + `R 键` 持续数秒，直到进入 Recovery Menu；
2. **选择更新**：选择第 5 项 `更新系统软件` (Update System Software) $\to$ `从 PS3 / 电脑更新` (Update from PC)；
3. **连接主机**：使用原装 USB 数据线将掌机连接至已开启 QCMA 的电脑；
4. **确认版本**：确认屏幕提示检测到 `3.74` 离线更新包后确认写入；
5. **等待写入**：刷入期间请勿断开 USB 连线或拔出电池，等待系统自动重启进入初始桌面。

---

## 来源与版权说明

- 本指南整理自时鹏亮《[PSV 救砖图文教程](https://shipengliang.com/games/psv%e6%95%91%e7%a0%96%e5%9b%be%e6%96%87%e6%95%99%e7%a8%8b.html)》；
- PlayStation、PS Vita、Sony 及官方固件软件版权归 Sony Interactive Entertainment Inc. 所有。本项目仅供个人离线设备维护与历史软硬件故障抢修参考。
