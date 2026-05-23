# PhotoStudioUpdater

PhotoStudio reads `manifest.json` from this repository:

```text
https://raw.githubusercontent.com/kimothink/PhotoStudioUpdater/main/manifest.json
```

To publish an update, run the **Release PhotoStudio update package** workflow and enter a version higher than the installed app version, for example `1.0.2.0`.

The update ZIP is stored through Git LFS. `manifest.json` uses a `media.githubusercontent.com` URL so PhotoStudio downloads the actual ZIP instead of the LFS pointer file.
