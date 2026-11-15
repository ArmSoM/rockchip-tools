# Provenance and distribution notes

ArmSoM maintains this catalog and accompanying usage guides. Rockchip and the respective upstream contributors remain the authors of the supplied third-party tools and documents. Hosting a binary here does not make its source code available and does not relicense it as MIT, Apache, or another open-source license.

This collection is a dated snapshot of the Rockchip tools supplied to ArmSoM, not a statement that every binary is the newest available release. Individual archives retain their embedded licenses, notices and original manuals. A dependency license (for example Qt's LGPL notice) is not a blanket license for every bundled application.

`catalog.json` records source-relative paths, original archive hashes, download hashes, version labels and repackaging details. `PACKAGING-NOTES.json` identifies deliberately omitted files. The original source collection was not modified.

Two provisioning-tool archives have been repacked to omit historic session logs, saved configuration and a device-name payload. Linux AVB's bundled test-key directory is omitted; users must generate and protect their own keys. Executable bytes are unchanged in these repacks. Other archives are original files or explicitly identified directory snapshots/gzip wrappers.

Downloads do not contain a grant of HDCP credentials or certification, ArmSoM board validation, universal SoC compatibility, or a hardware warranty. No flashing, provisioning, fuse programming, voltage adjustment or performance measurement was performed to prepare this catalog. Consult the matched SDK/BSP, hardware revision and board documentation before using tools that write device state.

Report packaging defects through repository issues. Never attach production private keys, HDCP key material, customer serial-number databases or unredacted device logs.
