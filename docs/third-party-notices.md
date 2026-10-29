# Third-party notices

StreamNyaa uses third-party software. The upstream projects retain their copyrights and licenses; this beta does not relicense them.

| Component | Included version / role | Upstream |
| --- | --- | --- |
| MPV | `v0.41.0-244-gaf9c81fa1`; local playback, GPL-enabled Windows x86-64-v3 build | [MPV](https://github.com/mpv-player/mpv), [reported source revision](https://github.com/mpv-player/mpv/tree/af9c81fa1), [copyright and licensing](https://github.com/mpv-player/mpv/blob/af9c81fa1/Copyright) |
| FFmpeg | `N-123099-g862338fe3`; media libraries inside MPV | [reported source revision](https://github.com/FFmpeg/FFmpeg/tree/862338fe3), [license information](https://ffmpeg.org/legal.html) |
| libplacebo | `v7.360.0-6-g905358e-dirty`, as reported by MPV | [source repository](https://github.com/haasn/libplacebo/tree/905358e) |
| rqbit | `8.1.1`; separate local torrent-engine process, Apache-2.0 | [v8.1.1 source](https://github.com/ikatson/rqbit/tree/v8.1.1), [license](https://github.com/ikatson/rqbit/blob/v8.1.1/LICENSE) |
| MPV Windows payload | `mpv.exe`, `mpv.com`, `d3dcompiler_43.dll`, font configuration | [Windows build project](https://github.com/shinchiro/mpv-winbuild-cmake), [MPV's Windows build guidance](https://mpv.io/installation/) |
| StreamNyaa player interface | Custom `streamnyaa-player.lua` | Packaged application resource; hash in the release manifest |
| Additional software notices | Applicable copyright and license notices | [Tauri](https://github.com/tauri-apps/tauri), [React](https://github.com/facebook/react), [SQLite](https://sqlite.org/copyright.html) |
| WebView2 | Microsoft runtime required by the Windows interface | [Microsoft WebView2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/) |

MPV's GPL-enabled build and linked libraries have their own redistribution obligations. The [licenses directory](../licenses/) carries upstream notices and license texts, and the linked upstream repositories provide source and build material. Those sources are not a new license grant for StreamNyaa's application code.

The versions above are reported by the bundled programs. Consult the linked upstream licenses, source, and build material when redistributing a component.

Release downloads do not include movie/episode media or personal account data.
