# Updating a tool

1. Keep the original archive and record its source and SHA-256 locally.
2. Read the included manual and release notes. Version labels must describe the package actually supplied; do not infer a current release from an old PDF cover.
3. Inspect nested archives. Exclude operational logs, production identities and secret key material from public assets; document any repack precisely.
4. Add a dated GitHub Release asset, then update `catalog.json`, `SHA256SUMS` and the download table together.
5. Update the matching guide and its Chinese, English, Russian and German Blog variants. Preserve accurate commands, units, platform scope and limitations.
6. Verify every download, checksum, source link, translation relationship and relevant Blog build before reporting completion.

Keep binary packages in Releases rather than Git history. Never replace an existing release asset silently; publish a new version or an explicitly identified corrected archive.
