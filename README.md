# D-Converter: FFmpeg source

This repository holds the source code that corresponds to the FFmpeg programs (`ffmpeg` and `ffprobe`) distributed with D-Converter.

FFmpeg is free software. The builds shipped with D-Converter are licensed under the GNU General Public License, version 3. This repository exists so that anyone who receives those programs can get their complete source code here, at no charge.

It holds nothing else: no code of D-Converter itself and no binaries.

## Releases

There is one release per FFmpeg build that is shipped. Each release carries the source archives, a `SHA256SUMS` file, a manifest (component, upstream, exact revision) and build notes.

| Platform | FFmpeg build | Release |
|---|---|---|
| Windows (x64) | `N-122685-g9bfa1635ae-20260209` | [`windows-N-122685-g9bfa1635ae-20260209`](https://github.com/movzed/d-converter-ffmpeg-source/releases/tag/windows-N-122685-g9bfa1635ae-20260209) |
| macOS (Apple silicon) | `N-122685-g9bfa1635ae-dconverter-mac-arm64` | [`macos-N-122685-g9bfa1635ae-20261012`](https://github.com/movzed/d-converter-ffmpeg-source/releases/tag/macos-N-122685-g9bfa1635ae-20261012) |

## Windows (x64)

Release `windows-N-122685-g9bfa1635ae-20260209`: source of the executables `ffmpeg.exe` and `ffprobe.exe` that D-Converter for Windows carries in its installation folder. One source archive per component (the FFmpeg tree and every library built into the executables), the scripts of the build they come from, and beside them `README.md`, `BUILD.md`, `MANIFEST.md`, `MANIFEST.json` and `SHA256SUMS`.

## macOS (Apple silicon)

Release `macos-N-122685-g9bfa1635ae-20261012`: source of the executables `ffmpeg` and `ffprobe`, version `N-122685-g9bfa1635ae-dconverter-mac-arm64`, that D-Converter for macOS carries inside its application bundle. One archive, `dconverter-ffmpeg-mac-arm64-source-9bfa1635ae.tar.gz`: the FFmpeg tree at commit `9bfa1635aef08e777deaeeae15ff9a5ade412188` with no local change, the source archive of every library built into the executables exactly as downloaded, the build script with the patch series applied to it, the build record and the licence files taken from the sources. Beside it: `README.md`, `MANIFEST.md`, `BUILD.md`, `SHA256SUMS`. These executables link neither libdvdread nor libdvdcss.

## Checking a download

Each release has a `SHA256SUMS` file. After downloading the files of a release into one folder:

```
sha256sum -c SHA256SUMS
```

On macOS:

```
shasum -a 256 -c SHA256SUMS
```

## Questions

Open an issue in this repository.
