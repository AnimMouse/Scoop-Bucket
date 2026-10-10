# Anim Mouse's Personal Scoop Bucket

[![Tests](https://github.com/AnimMouse/Scoop-Bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/AnimMouse/Scoop-Bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/AnimMouse/Scoop-Bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/AnimMouse/Scoop-Bucket/actions/workflows/excavator.yml)

Personal bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## Apps

| App | Description |
| --- | --- |
| [`libjxl`](bucket/libjxl.json) | [JPEG XL](https://jpeg.org/jpegxl) encoder and decoder, exposing only `cjxl` and `djxl` instead of all 21 libjxl tools |
| [`mpv-v3`](bucket/mpv-v3.json) | Stable [mpv](https://mpv.io) release from the [shinchiro builds](https://sourceforge.net/projects/mpv-player-windows/), compiled for x86-64-v3 (requires AVX2: Intel Haswell / AMD Zen or newer) |
| [`rclone`](bucket/rclone.json) | [rclone](https://rclone.org) without the persisted `rclone.conf`, so it uses the standard config location (`%APPDATA%\rclone\rclone.conf`) |

Manifests are checked for new versions and updated automatically every 4 hours.

## How do I install these apps?

Add this bucket, then install an app from it:

```pwsh
scoop bucket add animmouse https://github.com/AnimMouse/Scoop-Bucket
scoop install animmouse/<app>
```

For example, to install mpv-v3:

```pwsh
scoop install animmouse/mpv-v3
```

Installed apps are updated with the usual `scoop update *`.
