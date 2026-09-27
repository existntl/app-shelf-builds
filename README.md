# Codex App Shelf Builds

Public distribution catalog for personal Android builds published through Codex App Shelf.

- `catalog.json` is consumed by the App Shelf Android client.
- Versioned APKs are published in `release-assets/` and verified on-device by SHA-256 before Android opens its protected installer.
- Application source code and signing material are not stored in this repository.

Public APKs can be downloaded and inspected by anyone. Do not put credentials, customer records, signing keys, or other secrets in an APK or catalog entry.

## Folio 1.14.1

Finalized app icon: near-white blue front page and soft-blue back page on a navy background. This is an icon update to 1.14.0, using the original package and signing identity to preserve existing records. Release build, signature and package identity verified; installation and hands-on verification on the owner's phone remain pending.

Refresh Codex App Shelf, select **Folio**, then **Update** and confirm Android's installer.

### Previous Folio 1.14.0 update

Folio is the new name for Work Hours Invoice, with one identity shared by the Android app and its Windows bookkeeping companion. Refresh Codex App Shelf and update the existing entry; the Android package and original signing identity are unchanged.

The update includes the slate-blue theme, page icon, company-scoped work and invoices, receipt capture and offline reading, expense guidance, equipment details and optional encrypted expense/receipt sync. Build, signature and 36 Android host test groups passed, including narrow screens and enlarged text. Final hands-on verification of this version on the owner's phone is pending. Publishing does not install the update automatically.
