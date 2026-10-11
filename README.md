# SpamChoppa

**Local call screening for Android, by PhaZe Logic Studios.**

SpamChoppa brings block rules, trusted callers, schedules, and local Activity together in a comic-inspired interface. It has no ads, purchases, accounts, analytics, or Internet permission.

**0.2.10 is a testing prerelease:** the APK is development-signed and debuggable. It requires **Android 10 or newer**. Read the [release notes](docs/releases/0.2.10.md) before installing.

[Download APK](https://github.com/phaze-logic/SpamChoppa-Releases/releases/download/v0.2.10/spamchoppa-0.2.10.apk) · [SHA-256 file](https://github.com/phaze-logic/SpamChoppa-Releases/releases/download/v0.2.10/spamchoppa-0.2.10.apk.sha256) · [All releases](https://github.com/phaze-logic/SpamChoppa-Releases/releases)

<img src="docs/assets/screenshots/overview.png" width="280" alt="SpamChoppa Protection screen before Android screening setup is completed, with no rules configured">

## Features

- Block or allow exact numbers, prefixes, and contained number patterns. Allow rules take priority.
- Organize rules in colored folders and pause a folder as a group.
- Apply weekly schedules, multiple windows, and overnight windows.
- Reject, drop, or silence eligible calls, including broad blocking of noncontacts or all eligible callers.
- Review local Activity, test a hypothetical number, and export or restore JSON backups.
- Use light/dark appearance and an optional lock backed by your device credentials.

## Get started

1. Download the APK and [verify its checksum](docs/installation.md#verify-the-download).
2. Install it using Android's permission for the download source.
3. Open SpamChoppa and choose **Default screening app**. Approve Android's caller ID/spam screening role.
4. Grant optional Contacts access if saved contacts should participate in screening.
5. Add rules and use **Settings → Test a number** to check their effect.

Android delivers only eligible calls to the default screening app. SpamChoppa does not filter SMS, show the full system call log, or guarantee call-log removal or voicemail behavior. Read [Android limits](docs/usage.md#android-limits) before relying on broad rules.

## Documentation and support

[Installation](docs/installation.md) · [Usage](docs/usage.md) · [Privacy](docs/privacy.md) · [Troubleshooting](docs/troubleshooting.md) · [Screenshots](docs/screenshots.md) · [Documentation index](docs/README.md)

For help or a reproducible bug, see [SUPPORT.md](SUPPORT.md). Report vulnerabilities privately using [SECURITY.md](SECURITY.md).

This repository contains public documentation, screenshots, and release configuration. Completed install APKs are distributed as GitHub Release assets. Application source and source archives are not published here; GitHub's automatic source downloads contain this public repository's documentation and configuration only.

SpamChoppa is proprietary. See [LICENSE](LICENSE), [NOTICE](NOTICE), and [licensing](docs/licensing.md).
