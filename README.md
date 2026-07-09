# Epilog Releases

Sparkle update feed and release archives for the [Epilog](https://epilog.io) macOS app.

- `appcast.xml` — the Sparkle feed the app polls for updates. Entries are
  appended by `scripts/release_macos.sh` in the main (private) repo.
- Release assets — notarized, EdDSA-signed `Epilog-<version>.zip` archives.

Do not edit `appcast.xml` by hand unless you know what you're doing: each
item's `sparkle:edSignature` must match the zip byte-for-byte.
