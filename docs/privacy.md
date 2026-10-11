# Privacy and local data

SpamChoppa has **no Internet permission**, account requirement, analytics, advertising, or billing. Rules and screening history are stored locally. The app does not upload them to a SpamChoppa service.

## Permissions and data

Android's caller ID/spam screening role lets the app handle eligible calls supplied by Android. Optional Contacts access lets saved contacts participate in screening and supports contact-based decisions. Without it, Android normally bypasses screening for saved contacts.

Local Activity retains up to 500 events with telephone numbers, actions, decision reasons, and timestamps. Up to 30 backup snapshots are stored privately on the device. Android controls daily-job timing.

## Exports and imports

JSON exports and exported snapshots can contain telephone numbers, rules/settings, and historical actions, reasons, and timestamps. Treat them as sensitive. The document picker lets you choose a destination, including a cloud-backed provider; that provider's handling is separate from SpamChoppa.

Import replaces rules/settings after confirmation, preserves current Activity, and does not merge imported history. Uninstalling removes private data and local backups, but does not delete copies exported elsewhere.

## App lock

The optional lock uses existing Android device credentials or strong biometrics. No separate app PIN is stored. Screening continues while the UI is locked. Protected screens use Android's secure-window flag to restrict screenshots and display capture; this does not encrypt or secure exported JSON.

## Support and screenshots

Public GitHub issues, comments, and attachments are visible to others. Remove personal numbers, contact names, real call history, notifications, and device identifiers before sharing. Use synthetic examples instead of uploading a full backup.

See [support](../SUPPORT.md) and [security reporting](../SECURITY.md) for the appropriate channel.

[Documentation index](README.md)
