# ArmSoM Rockchip 工具下载库

本仓库收录 24 类工具，其中 34 个平台或版本包可下载、1 个包暂停等待安全核验，整理日期为 2026-11-15。工具包直接存入 Git 仓库，通过 [完整下载表](README.md#download-the-right-package) 选择单个文件；当前下载文件约 552 MiB；完整 Git 克隆还包含历史文件。Linux PinDebug 大文件分为两个分卷，下载入口附带拼接和校验方法。

每个工具按实际版本、运行平台和原始资料分别说明。目录名、工具版本和 PDF 手册版本不是同一个概念，也不表示支持所有 ArmSoM 产品。先确认板卡、SoC、存储、SDK/BSP 和运行主机架构，再选择工具及固件。

## 下载后检查

1. 根据下载表选择工具和主机平台，不混用 Linux、Windows、macOS 包。
2. 使用 `Get-FileHash`（PowerShell）或 `sha256sum`（Linux）计算文件 SHA-256，与 [校验表](SHA256SUMS) 对照。
3. 解压到独立目录，保留说明书、依赖库和原厂声明；不要只复制一个可执行文件。
4. 使用板卡对应 SDK 的 Loader、固件、分区参数和原理图。本文档整理没有进行刷机、熔丝烧写、调压或硬件兼容性测试。

## 来源与整理范围

工具与原始说明仍属于 Rockchip 和各组件作者。ArmSoM 提供目录、校验和使用说明，不将原厂二进制声明为 ArmSoM 开发或统一套用开源许可证。部分组件包含自己的许可文本，按原文保留。

设备信息和 HDCP 工具的干净重打包版本移除了历史日志、保存的配置和设备名称数据；AVB 包移除了示例密钥目录，执行程序保持原字节。请重新配置自己的测试环境和密钥。完整记录见 [NOTICE.md](NOTICE.md) 和 [PACKAGING-NOTES.json](PACKAGING-NOTES.json)。

[ArmSoM 技术博客](https://blog.armsom.org/zh/) · [ArmSoM 产品手册](https://docs.armsom.org/) · [ArmSoM 官网](https://www.armsom.org/)

## 使用指南

- [RKDevTool 下载与使用：Loader、分区镜像和整包固件烧录](guides/zh/rkdevtool.md)
- [DriverAssitant 5.13：Windows Rockusb 与 ADB 驱动安装排查](guides/zh/driver-assistant.md)
- [upgrade_tool 下载与使用：命令行烧录、设备选择和结果校验](guides/zh/upgrade-tool.md)
- [boot_merger 使用流程：正确组合 DDR、下载代码与 Loader](guides/zh/boot-merger.md)
- [Firmware_Merger：Flat RK、Flat GPT 与 Compact GPT 固件打包](guides/zh/firmware-merger.md)
- [afptool 与 rkImageMaker：理解并打包 Rockchip update.img](guides/zh/firmware-pack-tools.md)
- [Linux_Diff_Firmware：制作和验证 Rockchip 差分 OTA 包](guides/zh/diff-firmware.md)
- [DDR Bandwidth Tool：测量 Rockchip 内存带宽并读懂统计指标](guides/zh/ddr-bandwidth.md)
- [DDR_UserTool 1.41：为板卡选择 DDR 测试配置](guides/zh/ddr-user-tool.md)
- [rk_ddrbin_tool：读取和修改 DDR 初始化参数](guides/zh/ddrbin-tool.md)
- [PinDebug：排查 Rockchip IOMUX、GPIO 与电压域配置](guides/zh/pin-debug.md)
- [USB SQ Tool 1.5：从 USB 眼图排查到 PHY 参数与代码生成](guides/zh/usb-sq-tool.md)
- [rk_sign_tool 与 sign_tool：Rockchip 固件签名和校验流程](guides/zh/rk-sign-tool.md)
- [SecureBootTool 1.85：理解历史 Rockchip 安全启动工具链](guides/zh/secureboot-tool.md)
- [Linux SecurityAVB：密钥、启动镜像签名与版本边界](guides/zh/linux-avb.md)
- [Linux SecurityDM：检查 dm-verity 与加密根文件系统打包流程](guides/zh/linux-dm.md)
- [BoardProofTool 1.01：下载、CPU ID 完整性与集成准备](guides/zh/board-proof.md)
- [EfuseTool 1.42：建立可追溯的安全启动配置工位](guides/zh/efuse-tool.md)
- [ParameterTool 1.2：烧录前检查 Rockchip 分区参数](guides/zh/parameter-tool.md)
- [RKDevInfoWriteTool：受控写入序列号与 MAC 信息](guides/zh/devinfo-write.md)
- [RKPCBATool 1.2.1：配置 Linux 板卡功能测试与人工判定](guides/zh/pcba-tool.md)
- [HDCP Key Writer：授权密钥打包与设备写入流程](guides/zh/hdcp-key-writer.md)
- [SDDiskTool 1.78：区分 SD 启动卡、升级卡与 PCBA 测试卡](guides/zh/sd-disk-tool.md)
- [programmer_image_tool：将 update.img 转为 eMMC、SPI NOR 与 NAND 烧录器文件](guides/zh/programmer-image-tool.md)

[EN](guides/en/) · [中文](guides/zh/) · [RU](guides/ru/) · [DE](guides/de/)

[USB SQ Tool 1.5: download withheld / 暂停下载](SECURITY-REVIEW.md)
