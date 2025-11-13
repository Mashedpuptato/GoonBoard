# Goonboard (Packaged Release)

This ZIP contains everything required to run the compiled Goonboard desktop assistant on Windows.

## Contents

- `Goonboard.exe` – the single-file executable (includes Python + Qt runtimes).
- `assets/` – placeholder folders for your media (`images`, `gifs`, `overlay`, `sfx`). Drop your own files here; keep the `.keep` marker so empty folders remain.
- `messages.txt` – text prompts, one per line.
- `settings.json` – saved options from the configuration window.
- `stats-state.json` – runtime counters.
- `LOGO/` – icons used by the tray and the executable.

Keep all of these items together in the same directory as `Goonboard.exe`.

## Quick Start

1. Extract the ZIP into a writable folder.
2. Populate `assets/` with your media and edit `messages.txt` if desired.
3. Double-click `Goonboard.exe`.
   - The first launch shows the options window for configuration.
   - Use the tray icon to pause/resume overlays, toggle audio, or reopen settings.

Settings are saved back to `settings.json`; messages are written to `messages.txt`.

## Updating Content

- Add or remove media files inside the `assets` subfolders while the app is running.
- Use the tray menu’s **Reload assets** option to refresh without restarting.
- Modify `messages.txt` and choose **Reload assets** to pull in new lines.

## Support

If the executable fails to start, ensure antivirus is not blocking the unsigned binary and that the ZIP was fully extracted (it cannot run in-place from inside the archive). For further issues, rerun the executable from PowerShell to view console output.

---

*This app was made with partial to full support with Cursor AI.*¹

¹Cursor AI assisted with feature implementation, packaging automation, and documentation updates.

