# Daywell for Android

Daywell is a calm, simple medication companion: a daily schedule of your medicines, reminders at the
times you set, your streak and adherence, and a Medical ID with your allergies, blood type and
emergency contact.

This repository only hosts the **Android app downloads and updates**. The source code is private.

## Download

- **[Latest release](https://github.com/adam-ctrlc/daywell-releases/releases/latest)**
- **[All releases](https://github.com/adam-ctrlc/daywell-releases/releases)**

Daywell needs Android 7.0 or newer.

Most updates are delivered inside the app, so not every release has an APK (see [Updates](#updates)). To install Daywell for the first time, open **All releases** and use the newest one that has a `daywell-vX.Y.Z.apk` file under **Assets**.

## Install

1. On your Android phone, open **All releases** above and tap the newest `daywell-vX.Y.Z.apk`.
2. When the download finishes, tap the file to open it.
3. The first time, Android asks to allow installs from your browser. Tap **Settings**, switch on
   **Allow from this source**, then go back and tap **Install**.
4. Open Daywell and sign in, or create an account. Your account and data are online, so they're the same on every device.

Already have Daywell? Install the new APK over it the same way; your medications and history stay.

## Updates

Daywell checks for a new version every time you open it. Updates are required: when one is out, an
**Update required** screen lists what's new.

- **Most updates download inside the app.** Tap **Update now**, wait a few seconds, and Daywell
  restarts on the new version. Only the changed files are downloaded. No reinstall, and no
  permission prompts.
- **Occasionally a new app version (APK) is needed**, when Android-level parts of the app change.
  Tap **Download**, and your browser downloads the APK; open it to install over the current app.

If a new version ever fails to start, Daywell automatically goes back to the version that worked.

## Moving to a new phone

Install Daywell on the new phone and sign in with the same username and password. Everything is there.

Your data is also yours to keep: go to **Profile**, then **Your data**, then **Export data**, and to bring a backup in, use **Import backup** in the same place. Backup files contain your health information, so keep them private.

## Check that a download is genuine

Every Daywell APK is signed with the same key. Its SHA-256 certificate fingerprint is:

```
01:86:26:F6:F7:03:8C:2F:33:3B:9B:A4:65:F2:2D:91:CA:C3:12:C2:FD:AD:F7:3A:CB:48:18:35:9D:B5:42:EF
```

With the Android SDK build tools: `apksigner verify --print-certs daywell-vX.Y.Z.apk` and compare the
`SHA-256 digest` line. Android also refuses to install an update signed with a different key, so an
APK that doesn't come from here can't replace your installed Daywell.

## Privacy

- Your account, medications, history, photos and Medical ID are saved in your Daywell account on
  Daywell's server (in Tokyo), so they're the same on every device you sign in on. Your password is
  stored scrambled, so nobody can read it.
- If you connect a pill dispenser, your dose times and compartments are saved on the Daywell server
  so the dispenser can follow them.
- Daywell has no ads and no analytics.
- Permissions: internet (your account and update checks) and notifications with exact alarms
  (reminders on time, even after the phone restarts). Photos: Daywell only receives a photo you pick
  yourself. It can't read your other files, contacts, location or microphone, and never asks to
  install apps itself.

Daywell helps you keep track of your medicines. It isn't medical advice: always follow what your
doctor or pharmacist tells you.

## What's in a release (technical)

| File | What it is |
|---|---|
| `daywell-vX.Y.Z.apk` | The Android app, in releases that include a new app version |
| `latest.json` | The update manifest the app reads: version, release notes, the oldest app build that can run it, and every app file with its SHA-256 hash |
| `f-<sha256>` | App files for in-app updates, uploaded once and reused by later releases |

Installed apps read [`latest.json` from the latest release](https://github.com/adam-ctrlc/daywell-releases/releases/latest/download/latest.json).

## License

Apache License 2.0. See [LICENSE](LICENSE).
