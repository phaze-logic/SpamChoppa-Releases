# Use SpamChoppa

## Protection and rules

On **Protection**, enable protection and confirm SpamChoppa holds the default screening role. Add rules in **Blocklist** or **Allowlist**. Allow rules take priority over blocking rules.

| Match type | Meaning |
| --- | --- |
| Exact | Complete normalized number digits |
| Prefix | Numbers starting with the specified digits |
| Contains | Numbers containing the specified digit sequence |

Add country-code and national-number variants explicitly; exact matching does not automatically equate them. Short prefixes and contained patterns can affect many callers. Begin with narrow rules and test their effect.

Use colored folders to organize rules and pause a folder's rules together.

## Blocking and schedules

In **Settings → Blocking**, choose the action:

- **Reject:** decline the call.
- **Drop:** disconnect without explicit rejection.
- **Silence:** let it ring silently.

Broad options can block noncontacts or all eligible calls. Check allow rules and optional Contacts access before enabling them.

**Settings → Weekly schedule** supports multiple windows, weekday overrides, and overnight windows. Schedules follow device local time. Equal start/end times mean an all-day window.

## Test a number

Open **Settings → Test a number**, enter a number, and choose whether to treat it as a saved contact. The result shows the decision and reason under the current rules/settings and local time.

The saved-contact option is hypothetical. The tester does not place a call, prove Android will deliver that caller to screening, or guarantee a carrier's response.

## Activity

**Activity** records calls delivered to the screening service, including the number, time, action, and decision reason. You can add a number to a list from an event. Up to **500 events** are retained locally.

Activity is not Android's full call history. Missing events can mean Android did not send the call to the screening service.

## Backup and restore

Use **Settings → Backup & restore** to export or import JSON through Android's document picker. Exports can include telephone numbers and Activity actions, reasons, and timestamps, alongside rules/settings. Keep them private.

Import replaces rules and settings after confirmation. It preserves the importing app's **current Activity** and does not append Activity from the file. Export the current configuration before replacing it.

Local backup history retains up to **30 private snapshots**. Daily jobs run when Android schedules them and battery conditions permit; exact timing varies. Export snapshots to keep copies outside the app. Uninstalling removes app-private data and snapshots.

Validation limits are 1,000 rules and 1 MiB per state/backup; these are storage limits, not paid tiers.

## Appearance and lock

**Settings → Appearance & privacy** provides light/dark appearance and an optional lock using existing secure device credentials or strong biometrics. SpamChoppa stores no separate app PIN. Screening continues independently of the UI lock. Protected screens use Android's secure-window flag; see [privacy](privacy.md).

## Android limits

- Only eligible telephone calls reach the default screening service. Hidden/private, unavailable, payphone, emergency, and unsupported calls cannot be promised to pass through it.
- Saved contacts normally bypass screening until Contacts access is granted.
- SMS filtering is not implemented.
- Removal of blocked calls from Android's system call log is not guaranteed.
- Voicemail behavior depends on Android and your carrier.
- Unknown contact lookup or storage failures fail open, allowing calls through.

[Privacy](privacy.md) · [Troubleshooting](troubleshooting.md) · [Documentation index](README.md)
