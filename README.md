# Nublet — release feed

Public feed for [Nublet](https://nublet.app)'s in-app auto-updater (Sparkle).

- `appcast.xml` — the update feed the app polls.
- Each release's `Nublet-<version>.dmg` is attached as a **GitHub Release asset**.

Cut a release with `Scripts/package.sh` in the app repo: it signs + notarizes the DMG
and prints the `<item>` block to paste into `appcast.xml`. Then upload the DMG here.
