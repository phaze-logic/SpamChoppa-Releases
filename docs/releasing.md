# Release maintenance

This repository holds public documentation, screenshots, and release configuration. Build and validate the app privately. Publish only completed install APKs and checksums as release assets. Never upload application source, source ZIPs, test APKs, signing credentials, backups, or device evidence.

## Release contract

| Item | Convention |
| --- | --- |
| Tag | `vX.Y.Z` |
| Title | `SpamChoppa X.Y.Z` with testing status when applicable |
| APK | `spamchoppa-X.Y.Z.apk` |
| Checksum | `spamchoppa-X.Y.Z.apk.sha256` |
| Notes | Changes, requirements, signing/debug status, validation, and limits |

The checksum file identifies the final APK bytes and exact filename:

```text
<64 hexadecimal SHA-256 characters> *spamchoppa-X.Y.Z.apk
```

`v0.2.10` uses the existing development-signed, debuggable build 12 and must remain a **prerelease**. Record the verified certificate fingerprint; never publish its private key.

## Publishing checklist

1. Verify actual APK version/code, UTC build date, package, minimum/target API, byte size, signer, and debug status.
2. Validate installation, launch, compatible updates, screening role, rules, and important UI behavior. Distinguish recorded results from newly executed tests and device/carrier limits.
3. Review licensing and third-party notices. Preserve proprietary terms.
4. Hash the final APK and produce its checksum asset. Repeat verification if bytes change afterward.
5. Prepare notes using the [template](release-notes-template.md). Mark testing builds as prereleases.
6. Require passing GitHub repository checks. Inspect public files for source, secrets, personal data, and broken links; review rendered pages and screenshots. Repository checks do not test the Android app.
7. Publish the APK and checksum only. GitHub's automatic source ZIP/tarball contains this public documentation repository, not the app source.
8. Download both public assets and verify size/hash, release status, and links.
9. Update overview, installation, changelog, security policy, notes, and screenshots to match publication.

Never silently replace a published APK or checksum. Use a new version for changed binary bytes. Downloads are manual; there is no app network-update feed.

[Documentation index](README.md)
