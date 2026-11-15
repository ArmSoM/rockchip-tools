# ArmSoM Rockchip 工具下载中心

这里集中维护 Rockchip 开发工具的版本化下载、校验值和使用说明。当前快照包含 **24 类工具、35 个平台/版本下载包**。

请到 [下载目录](README.md#download-the-right-package) 选择对应工具，或进入 [GitHub Releases](https://github.com/ArmSoM/rockchip-tools/releases/tag/2026.11.15)。仓库的 Code → Download ZIP 仅下载目录与说明，不包含工具本体。

## 使用前确认

1. 核对电脑操作系统与处理器架构，再核对板卡、SoC、载板、存储和 SDK/BSP。Windows/Linux/macOS 包不能混用。
2. 比较下载文件与 [catalog.json](catalog.json) 中的 SHA-256。版本字段描述当前收集到的文件，不宣称为厂商最新版本。
3. 完整解压后阅读随包 PDF、README 和更新记录；不要只复制一个 EXE 而遗漏 DLL 或资源目录。
4. 先识别设备和保存当前信息，再安排写入。擦除、改电压、eFuse/OTP 和密钥配置不是通用的一键操作。
5. 两个写号工具的公开副本已去除历史日志、旧会话配置及设备名称数据；Linux AVB 去除了示例密钥目录。请重新建立自己的配置和密钥。工具可执行文件未改动，原始本地资料未改动。

[ArmSoM 技术博客](https://blog.armsom.org/zh/) · [ArmSoM 文档](https://docs.armsom.org/) · [ArmSoM 产品](https://www.armsom.org/)

工具属于原作者，现有许可与声明予以保留；这里不把全部二进制重新声明为开源软件。具体封装记录见 [PACKAGING-NOTES.json](PACKAGING-NOTES.json)，来源与边界见 [NOTICE.md](NOTICE.md)。本文准备过程没有烧录或硬件实测。
