# ArmSoM Rockchip Tools

Rockchip development-tool downloads, SHA-256 checksums, and usage references maintained by ArmSoM.

[中文说明](README.zh-CN.md) · [ArmSoM Blog](https://blog.armsom.org/) · [ArmSoM Docs](https://docs.armsom.org/) · [ArmSoM products](https://www.armsom.org/)

## Download the right package

The **2026-11-15 collection contains 24 tool families and 35 platform/version packages**. Binaries are stored directly in this Git repository. Download the individual packages below; cloning or downloading the entire repository retrieves approximately 569 MiB of packages. The large Linux PinDebug package is split into two parts, with reconstruction instructions at its download link.

Version labels describe the supplied collection, not the latest vendor release. A host OS label does not imply support for every host CPU architecture or ArmSoM board. Match the board, SoC, carrier, storage, SDK/BSP and manual before using a tool.

| Tool | Purpose | Downloads |
|---|---|---|
| RKDevTool | Windows Rockusb flashing GUI | [Windows / 3.37 release notes](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/rkdevtool/RKDevTool-windows-directory-snapshot.zip) |
| DriverAssitant | Windows Rockusb and ADB driver installation | [Windows / 5.13](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/driver-assistant/DriverAssitant_v5.13.zip) |
| upgrade_tool | Command-line firmware flashing | [Linux / 2.44](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/upgrade-tool/upgrade_tool_v2.44_for_linux.zip) · [macOS / 2.13](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/upgrade-tool/upgrade_tool_v2.13_for_mac.zip) · [Windows / 2.46](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/upgrade-tool/upgrade_tool_v2.46.zip) |
| boot_merger | Loader packaging and unpacking | [Linux / 1.35 release notes](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/boot-merger/boot_merger-linux-directory-snapshot.zip) · [macOS / 1.3](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/boot-merger/boot_merger_v1.3_mac.zip) · [Windows / 1.32](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/boot-merger/boot_merger_v1.32.zip) |
| Firmware_Merger | Flat and compact flash image generation | [Linux / directory snapshot](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/firmware-merger/firmware-merger-linux-directory-snapshot.zip) |
| afptool, rkImageMaker and rockdev | Partition-image and update.img packaging | [Linux / directory snapshot](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/firmware-pack-tools/rockdev-linux-directory-snapshot.zip) · [macOS / 2.1](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/firmware-pack-tools/rockdev_v2.1_mac.zip) · [Windows / 20230109](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/firmware-pack-tools/RKImageMaker_20230109.zip) |
| Linux_Diff_Firmware | Differential OTA image packaging | [Linux / directory snapshot](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/diff-firmware/linux-diff-firmware-directory-snapshot.zip) |
| DDR Bandwidth Tool | DDR bandwidth and utilization measurement | [Linux target / manual 1.4.1](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/ddr-bandwidth/ddr-bandwidth-linux-directory-snapshot.zip) |
| DDR_UserTool | DDR test image workflow | [Windows / 1.41](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/ddr-user-tool/DDR_UserTool_v1.41.7z) |
| rk_ddrbin_tool | DDR initialization binary configuration | [Linux / 1.01](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/ddrbin-tool/rk_ddrbin_tool_V1.01.7z) · [Windows / 1.07.2](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/ddrbin-tool/rk_ddrBin_tool_V1.07.2.zip) |
| PinDebug | IOMUX, GPIO and voltage-domain inspection | [Linux / 1.11](https://github.com/ArmSoM/rockchip-tools/blob/main/downloads/pin-debug/README.md) · [Windows / 1.18](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/pin-debug/pin_debug_tool_v1.18_20250322_win.zip) |
| USB SQ Tool | USB PHY signal tuning and test-command reference | [Windows / 1.5](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/usb-sq-tool/Rockchip_USB_SQ_Tool_V1.5.7z) |
| rk_sign_tool and sign_tool | Firmware signing and signature verification | [Linux / 1.42](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/rk-sign-tool/rk_sign_tool_v1.42_linux.zip) · [Linux / directory snapshot](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/rk-sign-tool/rk_sign_tool-linux-directory-snapshot.zip) · [macOS / 1.2](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/rk-sign-tool/sign_tool_v1.2_mac.zip) |
| SecureBootTool | Historical Secure Boot preparation workflow | [Host to verify / 1.85](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/secureboot-tool/SecureBootTool_v1.85_foruser.zip) |
| Linux SecurityAVB | AVB certificate and image preparation | [Linux / manual 2.2.5](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/linux-avb/linux-security-avb-without-keys.zip) |
| Linux SecurityDM | Historical dm-verity root filesystem packaging | [Linux / 1.01](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/linux-dm/Linux_SecurityDM_v1_01.tar.gz) |
| BoardProofTool | Board-protection configuration workflow | [Windows / 1.01](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/board-proof/BoardProofTool_v1.01_20240823_02.zip) |
| EfuseTool | eFuse provisioning workflow | [Windows / 1.42](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/efuse-tool/EfuseTool_v1.42.zip) |
| ParameterTool | Rockchip partition parameter editing | [Windows / 1.2](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/parameter-tool/ParameterTool_v1.2.zip) |
| RKDevInfoWriteTool | Serial number and device information provisioning | [Windows / 1.3.7](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/devinfo-write/RKDevInfoWriteTool-v1.3.7-clean.zip) |
| RKPCBATool | Board production-test integration | [Windows host + Linux target / 1.2.1](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/pcba-tool/RKPCBATool_v1.2.1_20251226.zip) |
| HDCP Key Writer | Authorized HDCP key provisioning | [Windows / 1.0.5](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/hdcp-key-writer/Rockchip_HdcpKey_Writer_V1.0.5-clean.zip) |
| SDDiskTool | SD boot and upgrade media preparation | [Windows / 1.78](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/sd-disk-tool/SDDiskTool_v1.78.zip) |
| programmer_image_tool | eMMC, SPI NOR and NAND programmer images | [Linux / 1.26](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/programmer-image-tool/programmer_image_tool_v1.26_linux.tar.gz) · [Windows / 1.28](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/programmer-image-tool/programmer_image_tool_v1.28.zip) |

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
