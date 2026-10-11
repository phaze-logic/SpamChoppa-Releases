# Troubleshooting

## Installation or update fails

Confirm Android 10 or newer, download from [official releases](https://github.com/phaze-logic/SpamChoppa-Releases/releases), and [verify the checksum](installation.md#verify-the-download). Installation permission applies to the browser or file manager opening the APK. Version 0.2.10 is development-signed and debuggable; read Android's warnings.

Updates require the same package and signer. Export data you want to keep before uninstalling to address a signature mismatch. Older Call Harbor builds install separately; follow [migration guidance](installation.md#migrate-from-older-call-harbor-builds).

## A caller is not blocked

1. Confirm Protection is on and SpamChoppa is the default screening app.
2. Check allow rules, paused rules/folders, and schedule windows.
3. Use **Settings → Test a number** with the appropriate hypothetical saved-contact setting.
4. Check country-code versus national-number digits and match type.
5. For saved contacts, check optional Contacts permission.

The tester evaluates app rules, not Android call eligibility. Android may bypass the service for unsupported calls. Contact lookup/storage failures fail open. See [Android limits](usage.md#android-limits).

## A call appears in history or reaches voicemail

SpamChoppa cannot guarantee removal from Android's call log or control carrier voicemail. Reject, drop, and silence differ; confirm your action under **Settings → Blocking**.

## Activity is incomplete

Activity contains only calls delivered to the service, with a 500-event retention limit. It is not the full system call log. Imports preserve current Activity and do not add imported events.

## Schedule or daily backup timing differs

Schedules use local device time and timezone. Equal start/end times mean all day. Android schedules backup jobs subject to battery conditions; exact daily execution is not guaranteed. Use a manual backup/export for an immediate copy.

## A backup cannot be imported

Use a supported JSON export and read the displayed error. Validation limits include 1,000 rules, 500 history events, and 1 MiB per state/backup. Do not post the file publicly. Import replaces rules/settings after confirmation; export the current configuration first.

## Lock or screenshot capture behaves unexpectedly

The lock requires existing secure device credentials or supported strong biometrics. Protected screens restrict capture through Android's secure-window flag. Follow [screenshot guidance](screenshots.md#capture-guidance) using synthetic data.

For other problems, see [SUPPORT.md](../SUPPORT.md).

[Documentation index](README.md)
