# PinDebug Linux split archive

The Linux 1.11 package is larger than GitHub's 100 MiB single-file limit. Download **both parts** into one directory. They are consecutive pieces of the unchanged `.tar.gz` file, not independent installations.

- [Part 1: pin_debug_tool_v1.11_for_linux.tar.gz.001](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/pin-debug/pin_debug_tool_v1.11_for_linux.tar.gz.001)
- [Part 2: pin_debug_tool_v1.11_for_linux.tar.gz.002](https://raw.githubusercontent.com/ArmSoM/rockchip-tools/main/downloads/pin-debug/pin_debug_tool_v1.11_for_linux.tar.gz.002)

## Reconstruct on Linux / macOS

```sh
cat pin_debug_tool_v1.11_for_linux.tar.gz.001 pin_debug_tool_v1.11_for_linux.tar.gz.002 > pin_debug_tool_v1.11_for_linux.tar.gz
sha256sum pin_debug_tool_v1.11_for_linux.tar.gz
tar -xzf pin_debug_tool_v1.11_for_linux.tar.gz
```

On macOS, use `shasum -a 256` instead of `sha256sum`.

## Reconstruct in Windows PowerShell

```powershell
$outputArchive = [System.IO.File]::Create((Join-Path $PWD 'pin_debug_tool_v1.11_for_linux.tar.gz'))
try {
  foreach ($partName in @('pin_debug_tool_v1.11_for_linux.tar.gz.001', 'pin_debug_tool_v1.11_for_linux.tar.gz.002')) {
    $inputPart = [System.IO.File]::OpenRead((Join-Path $PWD $partName))
    try { $inputPart.CopyTo($outputArchive) } finally { $inputPart.Dispose() }
  }
} finally { $outputArchive.Dispose() }
Get-FileHash .\pin_debug_tool_v1.11_for_linux.tar.gz -Algorithm SHA256
```

The output command overwrites an existing reconstructed archive with this name. Keep original parts until validation succeeds. Extract the resulting gzip/tar with 7-Zip. This reconstructs the **Linux** application; it does not turn it into a Windows application.

## Expected complete-archive SHA-256

`16cb25b8fc2533e8f730a790c7486ab5042baa964b3bdb95a161ddce143c4a34`

## 中文说明

两个分卷必须一起下载，按 `.001`、`.002` 的顺序二进制拼接。校验合并文件的 SHA-256 后，再解压 `.tar.gz`。不要单独运行或改名某个分卷。Windows 用户若只需要 Windows 程序，应回到仓库首页下载 Windows 1.18 包。
