# ArmSoM Rockchip Tools

Versioned Rockchip development-tool downloads, SHA-256 checksums, and usage references for ArmSoM developers.

[中文说明](README.zh-CN.md) · [ArmSoM Blog](https://blog.armsom.org/) · [ArmSoM Docs](https://docs.armsom.org/) · [ArmSoM products](https://www.armsom.org/)

## Download the right package

The 2026-11-15 snapshot contains **24 tool families and 35 platform/version packages**. Download individual archives from the table below or the [release page](https://github.com/ArmSoM/rockchip-tools/releases/tag/2026.11.15). GitHub's **Code → Download ZIP** downloads this catalog, not the tool binaries.

Version labels describe this supplied collection, not the latest vendor release. A host OS label does not imply support for every CPU architecture or every ArmSoM board. Match the actual board, SoC, carrier, storage, SDK/BSP and tool manual first.

| Tool | Purpose | Downloads |
|---|---|---|
| RKDevTool | Windows Rockusb flashing GUI | [Windows / 3.37 release notes](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/RKDevTool-windows-directory-snapshot.zip) |
| DriverAssitant | Windows Rockusb and ADB driver installation | [Windows / 5.13](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/DriverAssitant_v5.13.zip) |
| upgrade_tool | Command-line firmware flashing | [Linux / 2.44](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/upgrade_tool_v2.44_for_linux.zip) · [macOS / 2.13](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/upgrade_tool_v2.13_for_mac.zip) · [Windows / 2.46](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/upgrade_tool_v2.46.zip) |
| boot_merger | Loader packaging and unpacking | [Linux / 1.35 release notes](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/boot_merger-linux-directory-snapshot.zip) · [macOS / 1.3](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/boot_merger_v1.3_mac.zip) · [Windows / 1.32](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/boot_merger_v1.32.zip) |
| Firmware_Merger | Flat and compact flash image generation | [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/firmware-merger-linux-directory-snapshot.zip) |
| afptool, rkImageMaker and rockdev | Partition-image and update.img packaging | [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/rockdev-linux-directory-snapshot.zip) · [macOS / 2.1](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/rockdev_v2.1_mac.zip) · [Windows / 20230109](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/RKImageMaker_20230109.zip) |
| Linux_Diff_Firmware | Differential OTA image packaging | [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/linux-diff-firmware-directory-snapshot.zip) |
| DDR Bandwidth Tool | DDR bandwidth and utilization measurement | [Linux target / manual 1.4.1](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/ddr-bandwidth-linux-directory-snapshot.zip) |
| DDR_UserTool | DDR test image workflow | [Windows / 1.41](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/DDR_UserTool_v1.41.7z) |
| rk_ddrbin_tool | DDR initialization binary configuration | [Linux / 1.01](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/rk_ddrbin_tool_V1.01.7z) · [Windows / 1.07.2](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/rk_ddrBin_tool_V1.07.2.zip) |
| PinDebug | IOMUX, GPIO and voltage-domain inspection | [Linux / 1.11](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/pin_debug_tool_v1.11_for_linux.tar.gz) · [Windows / 1.18](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/pin_debug_tool_v1.18_20250322_win.zip) |
| USB SQ Tool | USB PHY signal tuning and test-command reference | [Windows / 1.5](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/Rockchip_USB_SQ_Tool_V1.5.7z) |
| rk_sign_tool and sign_tool | Firmware signing and signature verification | [Linux / 1.42](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/rk_sign_tool_v1.42_linux.zip) · [Linux / directory snapshot](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/rk_sign_tool-linux-directory-snapshot.zip) · [macOS / 1.2](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/sign_tool_v1.2_mac.zip) |
| SecureBootTool | Historical Secure Boot preparation workflow | [Host to verify / 1.85](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/SecureBootTool_v1.85_foruser.zip) |
| Linux SecurityAVB | AVB certificate and image preparation | [Linux / manual 2.2.5](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/linux-security-avb-without-keys.zip) |
| Linux SecurityDM | Historical dm-verity root filesystem packaging | [Linux / 1.01](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/Linux_SecurityDM_v1_01.tar.gz) |
| BoardProofTool | Board-protection configuration workflow | [Windows / 1.01](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/BoardProofTool_v1.01_20240823_02.zip) |
| EfuseTool | eFuse provisioning workflow | [Windows / 1.42](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/EfuseTool_v1.42.zip) |
| ParameterTool | Rockchip partition parameter editing | [Windows / 1.2](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/ParameterTool_v1.2.zip) |
| RKDevInfoWriteTool | Serial number and device information provisioning | [Windows / 1.3.7](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/RKDevInfoWriteTool-v1.3.7-clean.zip) |
| RKPCBATool | Board production-test integration | [Windows host + Linux target / 1.2.1](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/RKPCBATool_v1.2.1_20251226.zip) |
| HDCP Key Writer | Authorized HDCP key provisioning | [Windows / 1.0.5](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/Rockchip_HdcpKey_Writer_V1.0.5-clean.zip) |
| SDDiskTool | SD boot and upgrade media preparation | [Windows / 1.78](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/SDDiskTool_v1.78.zip) |
| programmer_image_tool | eMMC, SPI NOR and NAND programmer images | [Linux / 1.26](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/programmer_image_tool_v1.26_linux.tar.gz) · [Windows / 1.28](https://github.com/ArmSoM/rockchip-tools/releases/download/2026.11.15/programmer_image_tool_v1.28.zip) |

## Verify a download

Compare the SHA-256 of the downloaded file with the matching row in [catalog.json](catalog.json) or [SHA256SUMS](SHA256SUMS). A matching hash identifies this release asset; it is not a hardware validation or malware-free guarantee.

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath '.\downloaded-package.zip'
```

```sh
sha256sum downloaded-package.zip        # Linux
shasum -a 256 downloaded-package.zip    # macOS
```

## Packaging and first use

- Keep tool DLLs, resource folders, language files and configuration templates together when extracting.
- Repacked provisioning tools omit saved settings and logs. Configure a fresh session before use; the repack has not been executed against hardware.
- AVB sample keys are omitted. Generate your own test or production keys and keep them out of this repository.
- Start with device identification and read-only inspection. Flashing, erasing, changing I/O voltage and provisioning eFuse/OTP require a board-specific recovery or irreversible-operation plan.
- Manuals and release notes may refer to different software generations. Preserve the distinction; do not apply an old register address or chip setting to a newer SoC by analogy.

See [NOTICE.md](NOTICE.md), [PACKAGING-NOTES.json](PACKAGING-NOTES.json) and [CONTRIBUTING.md](CONTRIBUTING.md). Third-party licenses remain with their original components; there is no blanket open-source license for the binaries.
