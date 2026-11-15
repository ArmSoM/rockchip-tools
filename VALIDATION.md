# Collection validation — 2026-11-15

- 24 tool families; 34 available platform/version packages; USB SQ Tool 1.5 withheld as documented in [SECURITY-REVIEW.md](SECURITY-REVIEW.md).
- 35 physical download files, including the two-part Linux PinDebug archive. All available files match SHA256SUMS; reconstructed PinDebug matches the full archive hash.
- 96 usage guides: 24 topics in English, Chinese, Russian and German. Command blocks and package hashes match across language editions.
- 16 original PDF manuals, 213 pages in total. Copied PDF hashes match the input documents; filenames and hashes are in manuals/index.json.
- Package links returned HTTP 200. This is a file and documentation review, not execution, malware certification or hardware validation.
- Three repacks omit historical logs/device configuration or AVB sample keys; see PACKAGING-NOTES.json. Individual upstream notices remain intact.

The guides distinguish package versions from manual revisions. Where a full manual is missing, the guide describes verified package contents, preparation and unresolved integration requirements instead of inventing device-write operations.
