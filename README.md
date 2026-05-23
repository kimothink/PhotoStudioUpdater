# PhotoStudioUpdater

PhotoStudio reads `manifest.json` from this repository:

```text
https://raw.githubusercontent.com/kimothink/PhotoStudioUpdater/main/manifest.json
```

To publish an update, run the **Release PhotoStudio update package** workflow and enter a version higher than the installed app version, for example `1.0.2.0`.

The workflow creates a GitHub Release containing:

- `PhotoStudio.update.zip`
- `manifest.json`

`manifest.json` points PhotoStudio to the release asset URL and includes the SHA-256 hash that `Updater.exe` verifies before replacing files.
