# D-Converter: FFmpeg source

This repository holds the source code that corresponds to the FFmpeg programs (`ffmpeg` and `ffprobe`) distributed with D-Converter.

FFmpeg is free software. The builds shipped with D-Converter are licensed under the GNU General Public License, version 3. This repository exists so that anyone who receives those programs can get their complete source code here, at no charge.

It holds nothing else: no code of D-Converter itself and no binaries.

## Releases

There is one release per FFmpeg build that is shipped. Each release carries the source archives, a `SHA256SUMS` file, a manifest (component, upstream, exact revision) and build notes.

| Platform | FFmpeg build | Release |
|---|---|---|
| Windows (x64) | `N-122685-g9bfa1635ae-20260209` | `windows-N-122685-g9bfa1635ae-20260209` (in preparation) |
| macOS (Apple Silicon) | not built yet | none yet |

## Checking a download

Each release has a `SHA256SUMS` file. After downloading the archives into one folder:

```
sha256sum -c SHA256SUMS
```

## Questions

Open an issue in this repository.
