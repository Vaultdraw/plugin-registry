# Vaultdraw plugin registry

The list of community plugins that Vaultdraw's **Settings → Plugins → Browse** shows. It is one file, [`index.json`](index.json), read only when you open Browse and only after you allow plugin downloads.

The list is empty for now.

## Adding a plugin

1. Build and package it: `vaultdraw-plugin package` (see the [plugin SDK docs](https://github.com/Vaultdraw/vaultdraw/blob/main/sdk/docs/registry.md)).
2. Open a pull request that adds the zip under `packages/` and one entry to `index.json` with its `sha256`.

Every install is checked against that checksum, and a plugin asks for your review before it runs.
