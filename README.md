# Rasoi Master — public releases

This repository **does not contain application source code**. It exists so **GitHub Releases** can host:

- Windows installers (`.exe` / NSIS)
- macOS disk images (`.dmg`) — when you publish them
- `latest.yml` and related metadata used by **electron-updater**

Desktop app source stays private in [`rasoiMaster-pos`](https://github.com/deepakkraj/rasoiMaster-pos).

**Updates:** Installed POS clients check this repo’s **Releases** page for a newer semver than the build they have, then download the published installer.

**Publishing:** CI in the private app repo runs `electron-builder --publish always` with `GH_TOKEN` (use secret **`GH_RELEASES_TOKEN`** there if the code repo is private — a PAT with `repo` scope that can create releases on **this** repository).
