# PhotoStudioSetup

This repository publishes the PhotoStudio NSIS installer.

To publish a setup installer, run the **Release PhotoStudio setup installer** workflow and enter a version, for example `1.0.2.0`.

The workflow creates a GitHub Release containing:

- `PhotoStudioSetup-<version>.exe`

The installer uses per-user installation:

```text
%LOCALAPPDATA%\Programs\PhotoStudio
```

This keeps the app updater simple because `Updater.exe` can replace installed files without administrator permission.
