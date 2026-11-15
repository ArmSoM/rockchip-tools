# ArmSoM Rockchip Tools

Rockchip development-tool downloads, SHA-256 checksums, and usage references maintained by ArmSoM.

[中文说明](README.zh-CN.md) · [ArmSoM Blog](https://blog.armsom.org/) · [ArmSoM Docs](https://docs.armsom.org/) · [ArmSoM products](https://www.armsom.org/)

## Download the right package

The **2026-11-15 collection contains 24 tool families: 34 platform/version packages are available**. Tools are stored in this Git repository. Open the matching tool directory below, choose a platform/version, and use GitHub to obtain the file; the current download files total approximately 552 MiB. A full Git clone also includes historical files. The large Linux PinDebug package is split into two parts, with reconstruction instructions in its directory README.

Version labels describe the supplied collection, not the latest vendor release. A host OS label does not imply support for every host CPU architecture or ArmSoM board. Match the board, SoC, carrier, storage, SDK/BSP and manual before using a tool.

| Tool | Purpose | GitHub directory / guide |
|---|---|---|
| RKDevTool | Windows Rockusb flashing GUI | [Windows / 3.37 release notes](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/rkdevtool) |
| DriverAssitant | Windows Rockusb and ADB driver installation | [Windows / 5.13](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/driver-assistant) |
| upgrade_tool | Command-line firmware flashing | [Linux / 2.44](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/upgrade-tool) · [macOS / 2.13](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/upgrade-tool) · [Windows / 2.46](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/upgrade-tool) |
| boot_merger | Loader packaging and unpacking | [Linux / 1.35 release notes](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/boot-merger) · [macOS / 1.3](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/boot-merger) · [Windows / 1.32](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/boot-merger) |
| Firmware_Merger | Flat and compact flash image generation | [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/firmware-merger) |
| afptool, rkImageMaker and rockdev | Partition-image and update.img packaging | [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/firmware-pack-tools) · [macOS / 2.1](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/firmware-pack-tools) · [Windows / 20230109](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/firmware-pack-tools) |
| Linux_Diff_Firmware | Differential OTA image packaging | [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/diff-firmware) |
| DDR Bandwidth Tool | DDR bandwidth and utilization measurement | [Linux target / manual 1.4.1](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/ddr-bandwidth) |
| DDR_UserTool | DDR test image workflow | [Windows / 1.41](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/ddr-user-tool) |
| rk_ddrbin_tool | DDR initialization binary configuration | [Linux / 1.01](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/ddrbin-tool) · [Windows / 1.07.2](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/ddrbin-tool) |
| PinDebug | IOMUX, GPIO and voltage-domain inspection | [Linux / 1.11](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/pin-debug) · [Windows / 1.18](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/pin-debug) |
| USB SQ Tool | USB PHY reference documentation | [Usage guide](guides/en/usb-sq-tool.md) |
| rk_sign_tool and sign_tool | Firmware signing and signature verification | [Linux / 1.42](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/rk-sign-tool) · [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/rk-sign-tool) · [macOS / 1.2](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/rk-sign-tool) |
| SecureBootTool | Historical Secure Boot preparation workflow | [Host to verify / 1.85](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/secureboot-tool) |
| Linux SecurityAVB | AVB certificate and image preparation | [Linux / manual 2.2.5](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/linux-avb) |
| Linux SecurityDM | Historical dm-verity root filesystem packaging | [Linux / 1.01](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/linux-dm) |
| BoardProofTool | Board-protection configuration workflow | [Windows / 1.01](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/board-proof) |
| EfuseTool | eFuse provisioning workflow | [Windows / 1.42](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/efuse-tool) |
| ParameterTool | Rockchip partition parameter editing | [Windows / 1.2](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/parameter-tool) |
| RKDevInfoWriteTool | Serial number and device information provisioning | [Windows / 1.3.7](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/devinfo-write) |
| RKPCBATool | Board production-test integration | [Windows host + Linux target / 1.2.1](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/pcba-tool) |
| HDCP Key Writer | Authorized HDCP key provisioning | [Windows / 1.0.5](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/hdcp-key-writer) |
| SDDiskTool | SD boot and upgrade media preparation | [Windows / 1.78](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/sd-disk-tool) |
| programmer_image_tool | eMMC, SPI NOR and NAND programmer images | [Linux / 1.26](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/programmer-image-tool) · [Windows / 1.28](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/programmer-image-tool) |

## Verify downloads

Use [SHA256SUMS](SHA256SUMS) for physical download files and [catalog.json](catalog.json) for source provenance, sizes, package hashes and the full PinDebug archive hash.

```sh
sha256sum path/to/download.zip
```

```powershell
Get-FileHash .\download.zip -Algorithm SHA256
```

Compare all 64 hexadecimal characters with the corresponding catalog entry before extraction. Extract into a new directory, retain bundled manuals and dependencies, and select the exact board's firmware and Loader from its SDK. A matching hash checks file identity; it does not certify hardware compatibility.

## Documentation and support

Original manuals remain inside their packages. [NOTICE.md](NOTICE.md) explains provenance and redistribution notes; [PACKAGING-NOTES.json](PACKAGING-NOTES.json) records the omitted logs, saved provisioning settings and sample-key directory. Upstream binaries are not relabeled as ArmSoM-developed or universally open source.

ArmSoM's tool articles provide host setup, workflows, version boundaries and troubleshooting. Board-specific setup remains in [ArmSoM Docs](https://docs.armsom.org/). No hardware flashing, security provisioning or performance test was performed for this collection. Keep private keys, HDCP credentials and device databases outside this repository.

Updates should retain distinct version labels and original notices. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Usage guides

- [RKDevTool download and workflow: Loader, partitions and update.img](guides/en/rkdevtool.md)
- [DriverAssitant 5.13: install Rockusb and ADB drivers on Windows](guides/en/driver-assistant.md)
- [upgrade_tool download: command-line Rockchip firmware workflow](guides/en/upgrade-tool.md)
- [boot_merger: prepare a Rockchip Loader without mixing DDR and boot components](guides/en/boot-merger.md)
- [Firmware_Merger: flat RK, flat GPT and compact GPT images](guides/en/firmware-merger.md)
- [afptool and rkImageMaker: understand and package Rockchip update.img](guides/en/firmware-pack-tools.md)
- [Linux_Diff_Firmware: build a Rockchip differential OTA package](guides/en/diff-firmware.md)
- [DDR Bandwidth Tool: measure memory traffic and interpret Rockchip counters](guides/en/ddr-bandwidth.md)
- [DDR_UserTool 1.41: select DDR test configurations for a board](guides/en/ddr-user-tool.md)
- [rk_ddrbin_tool: inspect and change DDR initialization parameters](guides/en/ddrbin-tool.md)
- [PinDebug: inspect Rockchip IOMUX, GPIO and voltage domains](guides/en/pin-debug.md)
- [USB SQ Tool 1.5: from USB eye-diagram diagnosis to PHY settings](guides/en/usb-sq-tool.md)
- [rk_sign_tool and sign_tool: prepare and verify signed Rockchip firmware](guides/en/rk-sign-tool.md)
- [SecureBootTool 1.85: understand a historical Rockchip Secure Boot workflow](guides/en/secureboot-tool.md)
- [Linux SecurityAVB: keys, signed boot images and version boundaries](guides/en/linux-avb.md)
- [Linux SecurityDM: inspect dm-verity and encrypted-rootfs packaging](guides/en/linux-dm.md)
- [BoardProofTool 1.01: download, CPU ID handling and integration checklist](guides/en/board-proof.md)
- [EfuseTool 1.42: prepare a traceable Secure Boot provisioning station](guides/en/efuse-tool.md)
- [ParameterTool 1.2: review Rockchip partition parameters before flashing](guides/en/parameter-tool.md)
- [RKDevInfoWriteTool: controlled serial-number and MAC provisioning](guides/en/devinfo-write.md)
- [RKPCBATool 1.2.1: configure Linux board functional tests and operator checks](guides/en/pcba-tool.md)
- [HDCP Key Writer: package authorized keys and control device provisioning](guides/en/hdcp-key-writer.md)
- [SDDiskTool 1.78: distinguish SD boot, upgrade and PCBA media](guides/en/sd-disk-tool.md)
- [programmer_image_tool: convert update.img for eMMC, SPI NOR and NAND programmers](guides/en/programmer-image-tool.md)

[EN](guides/en/) · [中文](guides/zh/) · [RU](guides/ru/) · [DE](guides/de/)


## PDF previews and tool directories

| Tool | GitHub directory / guide | PDF preview |
|---|---|---|
| RKDevTool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/rkdevtool) | [RKDevTool_manual_v1.2_cn.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/27081f89d32f.pdf) · [RKDevTool_manual_v1.2_en.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/6a8a5813c129.pdf) · [开发工具使用说明_v1.0.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/be6d064c5f70.pdf) |
| upgrade_tool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/upgrade-tool) | [命令行开发工具使用文档.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/925b67105873.pdf) · [命令行开发工具使用文档v1.1.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/8a7aa375abfc.pdf) |
| DDR Bandwidth Tool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/ddr-bandwidth) | [Rockchip_Introduction_DDR_Bandwidth_Tool_CN.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/35fc41c5ec2e.pdf) |
| PinDebug | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/pin-debug) | [PinDebug_UserManual.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/1cae2e2c0777.pdf) |
| USB SQ Tool | [GitHub](guides/en/usb-sq-tool.md) | [Rockchip_Introduction_USB_SQ_Tool_CN_V1.4.0.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/0ec9ef065fdc.pdf) |
| rk_sign_tool and sign_tool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/rk-sign-tool) | [sign_tool用户使用手册.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/8528f18eea87.pdf) |
| SecureBootTool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/secureboot-tool) | [Rockchip Secure Boot Application Note_v1.2_20160202.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/094883c784c1.pdf) |
| Linux SecurityAVB | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/linux-avb) | [Rockchip_User_Manual_Linux_AVB_EN.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/50f19e52844b.pdf) |
| RKPCBATool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/pcba-tool) | [Rockchip_Developer_Guide_Linux_PCBA_CN.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/31be89bdda4b.pdf) · [Rockchip_Developer_Guide_Linux_PCBA_EN.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/6cb5fb2c60e8.pdf) |
| HDCP Key Writer | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/hdcp-key-writer) | [Rockchip_User_Guide_HDCP_Key_Flash.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/e1ef88b767b1.pdf) |
| programmer_image_tool | [GitHub](https://github.com/ArmSoM/rockchip-tools/tree/main/downloads/programmer-image-tool) | [Linux — user_manual.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/454e7646c90d.pdf) · [Windows — user_manual.pdf](https://github.com/ArmSoM/rockchip-tools/blob/main/manuals/47ce51e919d3.pdf) |
