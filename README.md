# Codex App Shelf Builds

Public distribution catalog for personal Android builds published through Codex App Shelf.

- `catalog.json` is consumed by the App Shelf Android client.
- Versioned APKs are published in `release-assets/` and verified on-device by SHA-256 before Android opens its protected installer.
- Application source code and signing material are not stored in this repository.

Public APKs can be downloaded and inspected by anyone. Do not put credentials, customer records, signing keys, or other secrets in an APK or catalog entry.

## Folio 1.15.1

Replaces bulky back buttons with a simple arrow and consistently spaced page title. The shared header keeps a 48dp touch target, screen-reader label, keyboard focus feedback and right-to-left arrow support. Expense details, work forms, Schedule, connected devices and invoice imports use the same design. Existing Back actions and unsaved-draft protection are retained.

Clean Android build, signed release and 41 API35 host checks pass, including expense-draft Back navigation and enlarged-text native renders at 320dp width. The original signing certificate and package are preserved. Final physical-phone UI verification remains pending. Refresh Codex App Shelf, select **Folio**, then **Update**.

### Previous Folio 1.15.0 update

Adds optional read-only calendar access and a separate Schedule page. Select calendars already synced to the Android phone, choose a name filter per company, and see the next 90 days of planned shifts with times, locations and notes. Home shows just the next match. Calendar changes refresh the view; Google's calendar sync determines when remote edits reach the phone. Use for clock-in prefills the usual confirmation form; calendar hours never automatically become recorded or billed work. No calendar writing or calendar-content uploads are added.

After updating, open **Schedule**, grant calendar access and select work calendars. Build/lint, original signature and 33 API35 host checks pass, including recurring events, cancellations, permission handling, company isolation and timer preservation. These host checks use a test calendar provider; real Google calendar sync and permission UI on the owner's phone still need hands-on verification. Original package/signing identity and records are retained. Refresh Codex App Shelf, select **Folio**, then **Update** and confirm Android's installer.

### Previous Folio 1.14.1 update

Finalized app icon: near-white blue front page and soft-blue back page on a navy background. This is an icon update to 1.14.0, using the original package and signing identity to preserve existing records. Release build, signature and package identity verified; installation and hands-on verification on the owner's phone remain pending.

Refresh Codex App Shelf, select **Folio**, then **Update** and confirm Android's installer.

### Previous Folio 1.14.0 update

Folio is the new name for Work Hours Invoice, with one identity shared by the Android app and its Windows bookkeeping companion. Refresh Codex App Shelf and update the existing entry; the Android package and original signing identity are unchanged.

The update includes the slate-blue theme, page icon, company-scoped work and invoices, receipt capture and offline reading, expense guidance, equipment details and optional encrypted expense/receipt sync. Build, signature and 36 Android host test groups passed, including narrow screens and enlarged text. Final hands-on verification of this version on the owner's phone is pending. Publishing does not install the update automatically.
