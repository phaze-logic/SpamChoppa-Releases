# Install SpamChoppa

## Requirements and testing status

Use **Android 10 or newer** (minimum API 29). Version 0.2.10 targets API 36 and uses package `com.phazelogic.spamchoppa`.

This is a **development-signed, debuggable testing prerelease**, not a store production build. Android's signature governs package identity and compatible updates; the checksum detects a file mismatch.

## Verify the download

Download [spamchoppa-0.2.10.apk](https://github.com/phaze-logic/SpamChoppa-Releases/releases/download/v0.2.10/spamchoppa-0.2.10.apk) and its [checksum file](https://github.com/phaze-logic/SpamChoppa-Releases/releases/download/v0.2.10/spamchoppa-0.2.10.apk.sha256) from the official release.

The APK must be **2,004,178 bytes**, with SHA-256:

```text
0ccfe08297523fa78a993579d2fb3c492e975e06f0cb83f18f9f87ad73f83f3c
```

On Windows, run this in the download folder:

```powershell
Get-FileHash -LiteralPath '.\spamchoppa-0.2.10.apk' -Algorithm SHA256
```

Compare the entire hash, ignoring letter case. Do not install a mismatch; download again from the official release. A matching checksum alone does not independently authenticate the publisher.

## Install and enable screening

1. Open the APK on your phone. If prompted, allow installation from that specific browser or file manager in Android settings.
2. Complete installation. You can turn that source's installation permission off afterward.
3. Open SpamChoppa. Tap **Default screening app** on Protection and approve Android's caller ID/spam screening role (`CALL_SCREENING`). Only one app holds this role.
4. Optionally grant Contacts access. Android normally bypasses screening for saved contacts without this permission.
5. Enable Protection, add a rule, and check it under **Settings → Test a number**.

System dialogs differ by device. Read any security warning before deciding whether to proceed.

## Update an existing installation

Install the newer APK over the existing app. Android requires the same package and signer for an in-place update. Export a backup first. A differently signed APK cannot update the installed package; export data you want to keep before considering uninstalling.

The verified development certificate for 0.2.10 has SHA-256 fingerprint:

```text
1d88666cbc564eae11814c4c109880709410e1473b1280f5328afa05a9b23e70
```

Downloads are manual; the app has no network updater.

## Backup and restore

Export your rules and settings through **SpamChoppa Settings → Backup & restore**. Importing a supported JSON backup replaces rules/settings after confirmation while preserving the receiving app's current Activity. Private daily snapshots stay local to the installation; export data you want to keep before uninstalling.

[Usage](usage.md) · [Troubleshooting](troubleshooting.md) · [Documentation index](README.md)
