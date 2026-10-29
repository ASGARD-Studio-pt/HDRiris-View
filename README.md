# HDRiris View

**A fast desktop library and lighting-preview workspace for HDRI collections.**

HDRiris View keeps large `.hdr` and `.exr` libraries organized, searchable, and
ready to preview without leaving the desktop. Browse panoramas, test lighting on
PBR materials and custom models, and send an environment directly to your DCC.

> This is the official download and release repository for HDRiris View. The
> application is proprietary; its source code is not published here.

[Download HDRiris View](https://github.com/ASGARD-Studio-pt/HDRiris-View/releases)
· [Website](https://hdriris.asgard-studio.pt/)
· [Support](https://hdriris.asgard-studio.pt/support/)
· [Report an issue](https://github.com/ASGARD-Studio-pt/HDRiris-View/issues)

## Capture your own HDRIs with HDRiris

HDRiris View works with any compatible HDR or OpenEXR library, but it is also
the desktop companion to **HDRiris**—ASGARD Studio's mobile app for capturing
360° HDR environments on location.

Use HDRiris on your phone to follow a guided capture, process the environment
on-device, preview its lighting on 3D models or in AR, and export a 4K OpenEXR
or Radiance HDR file. Bring that file into HDRiris View to organize, inspect,
tag, and use it in your desktop workflow.

[Discover HDRiris](https://hdriris.asgard-studio.pt/)
· [Download on the App Store](https://apps.apple.com/us/app/hdriris/id6816681680)
· [Get it on Google Play](https://play.google.com/store/apps/details?id=pt.asgardstudio.hdriris)

## What it does

- Watches one or more folders and recursively indexes Radiance HDR (`.hdr`) and
  OpenEXR (`.exr`) files.
- Generates cached thumbnails and automatically detects library changes.
- Searches, filters, sorts, favorites, and browses assets in grid or list views.
- Switches between equirectangular panorama and real-time lighting previews.
- Adjusts exposure, environment rotation, camera pitch, material color,
  metalness, and roughness while evaluating an HDRI.
- Imports self-contained GLB 2.0 models with authored PBR materials and embedded
  PNG or JPEG textures for custom lighting previews.
- Reveals the original file in Finder or File Explorer and sends HDRIs directly
  to Blender.
- Offers optional automatic AI tag suggestions that run locally on the user's
  computer.

## Download and system requirements

Official installers and their SHA-256 checksums are published on the
[Releases page](https://github.com/ASGARD-Studio-pt/HDRiris-View/releases).

| Platform | Requirements | Download |
| --- | --- | --- |
| macOS | macOS 12 or newer; Apple silicon | `HDRiris-View-macOS-arm64.dmg` |
| Windows | Windows 10 or 11; x86-64 | `HDRiris-View-Windows-x64-Setup.exe` |

HDRiris View does not currently support Intel Macs, Windows on Arm, or Linux.

### Windows SmartScreen notice

The Windows 1.0 installer is not code-signed and may show a Microsoft Defender
SmartScreen **Unknown publisher** warning. This is expected for the initial free
release. Download the installer only from this repository and compare it with
the SHA-256 value in the release's `SHA256SUMS.txt` before running it. You should
never need to disable Windows security software.

### macOS installation

Open the DMG, drag **HDRiris View** into **Applications**, and launch it from
there. Official macOS builds are signed with ASGARD Studio's Developer ID and
notarized by Apple.

## Optional local AI tagging

AI tagging is opt-in. When enabled, HDRiris View downloads an approximately
72 MB TinyCLIP vision model in the background. Normal library scanning and
preview generation continue while it downloads, and existing library items are
analyzed once the model is ready.

Image analysis happens locally. HDRIs, thumbnails, embeddings, generated tags,
and library metadata are not uploaded for AI processing. The model can be
disabled or removed later from the application settings.

The versioned model packages and their licenses are maintained separately in
[HDRiris-View-Models](https://github.com/ASGARD-Studio-pt/HDRiris-View-Models).

## Releases and updates

Release notes document new features, fixes, known issues, and model-compatibility
changes. HDRiris View installers are distributed exclusively through this
repository and the official HDRiris website.

For reproducible verification, every release includes:

- Stable installer filenames for macOS and Windows.
- `SHA256SUMS.txt` containing checksums for the published assets.
- `build-info.json` identifying the application version and build environment.

## Support, privacy, and legal

- For installation or product help, visit [HDRiris Support](https://hdriris.asgard-studio.pt/support/).
- For reproducible bugs and feature requests, open a [GitHub issue](https://github.com/ASGARD-Studio-pt/HDRiris-View/issues).
- Read the [Privacy Policy](https://hdriris.asgard-studio.pt/privacy/) and [Terms of Use](https://hdriris.asgard-studio.pt/terms/).

HDRiris View is proprietary software. This public repository is provided for
official binaries, release notes, checksums, and product support; it does not
grant permission to copy, modify, redistribute, reverse engineer, or create
derivative works from the application except where applicable law expressly
permits it.

Copyright © 2026 ASGARD Studio. All rights reserved.
