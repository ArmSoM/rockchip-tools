# ArmSoM Rockchip 工具下载库

本仓库收录 24 类工具、35 个平台或版本包，整理日期为 2026-11-15。工具包直接存入 Git 仓库，通过 [完整下载表](README.md#download-the-right-package) 选择单个文件；下载整个仓库约需 569 MiB。Linux PinDebug 大文件分为两个分卷，下载入口附带拼接和校验方法。

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
