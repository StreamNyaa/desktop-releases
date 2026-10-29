# Install the Windows beta

## Requirements

- Windows 10 or 11 on a 64-bit Intel/AMD PC.
- Microsoft Edge WebView2 Runtime. Many Windows installations already include it; if the app cannot open its interface, use [Microsoft's official WebView2 Runtime download](https://developer.microsoft.com/en-us/microsoft-edge/webview2/).
- An x86-64-v3 compatible processor. An older CPU may open the app but fail when the player starts. This download is for Windows x64, not 32-bit Windows or ARM64.
- Internet access for metadata, sources, sign-in/sync, and peer playback. Temporary playback and full downloads use disk space and bandwidth; a 40.56 MiB installer is not the total space the app will use.

The player is included. You do not need to install a separate player or torrent client.

## Download and verify

1. Open the [Public Beta 1 release](https://github.com/StreamNyaa/desktop-releases/releases/tag/v0.1.15-beta.1).
2. Download `StreamNyaa_0.1.15_x64-setup.exe` and `SHA256SUMS.txt` from that release's Assets section. Do not use a reposted installer or an advertisement's download button.
3. In PowerShell, run this from the folder containing the installer:

   ```powershell
   Get-FileHash -LiteralPath '.\StreamNyaa_0.1.15_x64-setup.exe' -Algorithm SHA256
   ```

4. The expected SHA-256 is:

   ```text
   10F6D3CBD2B12AEBEF68B279089E727230C8DFC80B5E3A4629EDDD46BD5D3011
   ```

   If it differs, stop and download the file again from the release. A matching hash confirms that the file matches the published artifact; it does not certify its safety.

5. Scan the file with your security software. The published installer is **not code signed**. Windows may show an unknown-publisher or reputation warning. Review that warning yourself and install only if you accept the beta's risks. Do not turn off protection or override an organization's restrictions.
6. Open the installer and follow its prompts. Review the install location and any runtime or permission prompts. Open StreamNyaa from the shortcut afterward.

## First run

Start with browsing and the schedule before trying playback. Guest use is available; sign in only if you want account features. Select a title and its intended episode, then open Sources. **Use** begins preparation and playback; when a batch needs a file choice, select the correct episode file. Some sources may have no responding peers even when a listing reports seeders.

Choose a download folder deliberately. Temporary streaming pieces and a saved full release are different things. Allow for the size of the selected media, especially with batches. Review [privacy and network behavior](privacy.md) before torrent playback.

If a window appears to close but the app is still in the notification area, use **Quit StreamNyaa** from its tray menu when you want it fully stopped.

## Upgrade an existing installation

1. In StreamNyaa Settings, choose **Export personal backup** and save the file somewhere outside the app's folders. Check that the backup exists. It excludes account credentials and downloaded media; keep your downloaded files separately.
2. Finish or pause transfers and quit StreamNyaa, including its tray icon and player.
3. Verify the new installer's checksum, then run it and review the prompts.
4. Check that the app reports version 0.1.15 and that your library and history are present before continuing normal use.

Keep your backup until you are happy with the new version. If you encounter a data or installation error, save the message and report it rather than deleting your history or app data.

## Uninstall

Quit the player and StreamNyaa first. Use Windows **Settings → Apps → Installed apps → StreamNyaa → Uninstall** (the name varies slightly by Windows version).

Do not assume that uninstalling erases cloud records, downloaded media, backups, or every local preference. Clear or remove those deliberately after saving anything you need. Never delete a shared Downloads folder just to remove the app.

## When installation or startup fails

Record the Windows version, processor model, app version, and exact error. Check WebView2 and available disk space. Report an antivirus detection privately with its detection name and file hash; do not disable your antivirus. For a playback-only problem, include whether the player opens, whether video advances, and whether another permitted source works. See [Reporting feedback](feedback.md) and [Security](../SECURITY.md).
