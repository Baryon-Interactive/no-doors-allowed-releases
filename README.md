# No Doors Allowed: Vesper metadata

Signed store metadata for [No Doors Allowed](https://vesperplay.xyz/app/no-doors-allowed),
a voxel heist game by Baryon Interactive, distributed through
[Vesper](https://github.com/Baryon-Interactive/vesper).

The official catalogue registers this game's developer key and reads its
metadata from this repository's
[`vesper-metadata` release](https://github.com/Baryon-Interactive/no-doors-allowed-releases/releases/tag/vesper-metadata):

| File | Content |
| --- | --- |
| `store.json` | Title, summary, tags, cover, screenshots, requirements, platforms |
| `description.md` | Store page text |
| `targets.json` | Developer-signed channels, build manifests and download sources, bound to the exact bytes of the two files above |

`metadata/` holds the same files and their signed version history. To change
the store page, edit `store.json` or `description.md`, sign a new targets
version with the developer key, and replace the three release assets. The
catalogue picks the change up within about 15 minutes. See the
[publishing guide](https://github.com/Baryon-Interactive/vesper/blob/main/docs/publishing.md).

Builds are hosted at `https://packs.vesperplay.xyz/{release}/{pack_id}`:
`stable` is the Windows build and `stable-web-wasm32` is the browser build.
The signing key is never stored here.
