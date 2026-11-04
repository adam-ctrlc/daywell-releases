# Daywell for Android

Daywell is a calm, simple medication companion: a daily schedule of your medicines, reminders at the
times you set, your streak and adherence, and a Medical ID with your allergies, blood type and
emergency contact.

This repository only hosts the **Android app downloads and updates**. The source code is private.

## Download

| | |
|---|---|
| **Newest app version (APK)** | [daywell-v1.0.6.apk](https://github.com/adam-ctrlc/daywell-releases/releases/download/v1.0.6/daywell-v1.0.6.apk) |
| **Newest release page** | [Latest release](https://github.com/adam-ctrlc/daywell-releases/releases/latest) |
| **All releases** | [Releases](https://github.com/adam-ctrlc/daywell-releases/releases) |
| **Requirements** | Android 7.0 or newer, about 5 MB |

Not every release contains an APK: small updates are delivered inside the app (see
[Updates](#updates)). To install Daywell for the first time, use the newest release that lists a
`daywell-vX.Y.Z.apk` file under **Assets**.

## Install

1. On your Android phone, open the **Newest app version (APK)** link above.
2. When the download finishes, tap the file to open it.
3. The first time, Android asks to allow installs from your browser. Tap **Settings**, switch on
   **Allow from this source**, then go back and tap **Install**.
4. Open Daywell and create an account. Your account and data are stored on your phone.

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

From version 1.0.9 your account is online: install Daywell on the new phone and sign in with the same
username and password. Everything is there.

Still on the old phone with data from before 1.0.9 (it was saved on that phone only)? Before
updating, go to **Profile → Your data → Export data** and keep the file. After updating, sign in or
create an account, then **Profile → Your data → Import backup** and pick the file.

Backup files contain your health information. Keep them private.

## Release history

| Version | Type | Highlights |
|---|---|---|
| [1.0.17](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.17) | In-app update | The dispenser connects through Daywell, so your phone and dispenser don't need the same Wi-Fi; 6-character dispenser codes; compartments named by angle; Test mode |
| [1.0.16](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.16) | In-app update | Fixes photos that couldn't be read on some Android phones |
| [1.0.15](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.15) | In-app update | Photos open more reliably |
| [1.0.14](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.14) | In-app update | iPhone and high-efficiency (HEIC) photos can be used |
| [1.0.13](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.13) | In-app update | Medication colors show correctly again |
| [1.0.12](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.12) | In-app update | Tidier dispenser buttons |
| [1.0.11](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.11) | In-app update | An updated Guide |
| [1.0.10](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.10) | In-app update | Sign in with a username (old emails still work); Dispenser in the bottom bar; better fit on small screens |
| [1.0.9](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.9) | In-app update | Online account on every device; pill dispenser; notifications; medication photos and colours; dark theme |
| [1.0.8](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.8) | In-app update | Optional reason when skipping a dose; overdue message names the dose and time |
| [1.0.7](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.7) | In-app update | Export from any page as a backup file, a printable PDF report, or a spreadsheet |
| [1.0.6](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.6) | App (APK) | Export and import your data to move to a new phone; clearer time and date fields |
| [1.0.5](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.5) | In-app update | The Guide's topic list highlights the section you're reading |
| [1.0.4](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.4) | App (APK) | Updates download inside the app; no more permission to install apps |
| [1.0.3](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.3) | App (APK) | Search, a built-in Guide, a roomier phone layout, show/hide password |
| [1.0.2](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.2) | App (APK) | Update downloads inside the app |
| [1.0.1](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.1) | App (APK) | New app icon and launch screens |
| [1.0.0](https://github.com/adam-ctrlc/daywell-releases/releases/tag/v1.0.0) | App (APK) | First release |

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
