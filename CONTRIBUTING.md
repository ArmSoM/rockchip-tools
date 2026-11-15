# Updating a tool

1. Keep the original archive and record its source and SHA-256 locally.
2. Read the included manual and release notes. Version labels must describe the package actually supplied; do not infer a current release from an old PDF cover.
3. Inspect nested archives. Exclude operational logs, production identities and secret key material from public assets; document any repack precisely.
4. Add the versioned package to its `downloads/<tool>/` directory, then update `catalog.json`, `SHA256SUMS` and the download table together. Ordinary Git files must remain below 100 MiB; document reconstruction and both part/full hashes if an archive is split.
5. Update the matching guide and its Chinese, English, Russian and German Blog variants. Preserve accurate commands, units, platform scope and limitations.
6. Verify every download, checksum, source link, translation relationship and relevant Blog build before reporting completion.

This collection stores packages in Git at the owner's request. Do not silently replace a version with different bytes; use a new version or an explicitly identified corrected filename. As the collection grows, consider moving future large packages to Releases to limit clone size, while preserving existing download URLs.
