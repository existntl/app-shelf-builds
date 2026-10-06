## Rental Deck 0.4.2

Adds58 gallery links across6 previously empty records.51 images downloaded/decoded; Brookswood7 load in the source browser but direct downloads return403, explicitly disclosed. Skyside contains2 shared rendering/promotion images, not verified #205 interiors; the unit and historical1595price are no longer visible in current inventory and are unconfirmed. Ezekiel ad deleted; Yorkson corrected to1650/street parking. Source galleries captured via normal public UI.

16 Android gallery/live-feed host checks and9 feed/export checks pass. Signed release/lint passes with original identity. Public feed and bundled214links match. Physical-phone verification pending. Refresh App Shelf -> Rental Deck -> Update0.4.2, then Sources -> Refresh. No uninstall.

# Codex App Shelf Builds

Public distribution catalog for personal Android builds published through Codex App Shelf.

- `catalog.json` is consumed by the App Shelf Android client.
- Versioned APKs are published in `release-assets/` and verified on-device by SHA-256 before Android opens its protected installer.
- Application source code and signing material are not stored in this repository.

Public APKs can be downloaded and inspected by anyone. Do not put credentials, customer records, signing keys, or other secrets in an APK or catalog entry.

## Rental Deck 0.4.1

Fixes a reproduced stale-detail bug: refreshing the feed while a listing was open left its gallery showing the old photo count. Read-only listing pages and full-screen viewers now adopt refreshed records; background updates are picked up on resume. Editable application/profile fields stay intact. Empty galleries offer Refresh listing & photos, and default-feed requests avoid stale CDN snapshots. The APK now bundles all five verified Solomon image links, allowing legacy records without a photos field to recover without a feed download. Explicit empty-gallery removals remain respected.

32 Android host tests passed, including live public-feed transport, stale Solomon detail regression, bundled gallery migration, resume, viewer preservation and unsaved application edits. Native empty-gallery renders inspected at 360dp and 320dp/enlarged text. Signed release/lint passed; original package/signer retained. Physical-phone verification remains pending. Refresh App Shelf -> Rental Deck -> Update to0.4.1; no uninstall needed.

## Folio 1.16.4

Schedule is now its own tab between Work hours and Expenses. Tap a tab or swipe between sections to see all configured company schedules. Your agenda scroll position is retained when switching tabs, and job details return to the coloured schedule. Tab labels scroll horizontally at enlarged text sizes. Choosing a job for clock-in still opens a confirmation form and never automatically records worked hours.

Clean debug/test build and lint passed; 25 focused API35 host tests passed at 320dp/150% text, with 16 schedule checks also passing at 360dp/100%. Native renders were inspected. Original package and signing identity are retained. Physical-phone verification remains pending. Refresh Codex App Shelf -> Folio -> Update, then confirm Android's installer. Publication does not install automatically.

### Previous Folio 1.16.3 update

Fixes the schedule losing company colour coding after opening a job and going Back. Both Back controls return to the combined agenda, including after screen recreation. Company-only schedule cards now use the same coloured dot, fill and border. Cancelled-job recovery returns to the correct schedule. Existing invoice send-and-archive improvements remain included.

Clean debug/test build and lint passed; 29 focused API35 host tests passed at 320dp/150% text, and schedule renders were inspected. The release APK retains the original package and signing identity. Physical-phone verification remains pending. Refresh Codex App Shelf -> Folio -> Update, then confirm Android's installer. Publication does not install automatically.

### Previous Folio 1.16.2 update

After returning from the email app, choose **Sent â€” add to list and archive shifts** to mark the invoice Sent, place it in the invoice list and archive its matching company/period shifts and billed expenses. **Not sent yet** leaves work active. The original PDF, invoice amount and archived records remain saved. Work changed since export requires review before archiving. Opening the email chooser does not imply delivery.

The invoice list also shows the latest saved invoice awaiting archive. Includes soft company-colour card highlights from 1.16.1. Clean build/lint, 18 focused API35 host tests and narrow-screen renders pass. Original package and signing identity are retained. Actual device verification of the finish-send flow remains pending. Refresh Codex App Shelf -> Folio -> Update, then confirm Android's installer; publication does not install automatically.

### Previous Folio 1.16.0 update

Adds one chronological agenda across the selected company calendars, with company names, source calendars, times and locations. Shared occurrences appear once and ask for a company when ambiguous. Calendar connections explain missing sources and setup; the app reads calendars already on the phone rather than logging into work providers. Provider calendar sharing determines what appears and how promptly changes arrive.

Company colour dots now appear in the selector, schedule and recent work history. Choose from eight named colours in Edit company and Save company. Defaults are assigned automatically; saved choices stay with a company through renaming. Names stay visible. Colours do not alter billing data or original PDFs.

Planned shifts never automatically become billed work. Use for clock-in opens confirmation for the selected active company and cannot replace a running timer. Clean build/lint, original-signed release and 23 focused API35 host checks pass at 320dp/150% font. Actual phone/provider sync and device verification remain pending. Refresh Codex App Shelf -> Folio -> Update, then confirm Android's installer. Publishing does not install automatically.

### Previous Folio 1.15.3 update

Tap the running shift card to edit its department, show/job description and start date/time in a native popup. The timer keeps running and retains its original company. Save validates the start time and persists changes; Cancel preserves the existing shift. Drafts survive screen recreation. Outward swipes at the first or last tab no longer trigger buttons underneath.

Clean Android build/lint, original-signed release and 28 API35 host checks pass at 320dp/150% font, including timer restoration and company ownership. Physical-phone touch, keyboard/insets and force-stop/logcat verification remain pending. Refresh Codex App Shelf -> Folio -> Update, then confirm Android's installer. Publishing does not install automatically.

### Previous Folio 1.15.2 update

Fixes the next-shift preview collapsing and reappearing when returning to Work hours. The existing preview remains in place while the same calendar selection refreshes; unchanged text is not rebound. Changed company/calendar/filter settings or lost permission clear old details immediately, and a finished refresh with no matches removes the preview normally.

A regression test reproduced the old collapse and passes with the fix. Clean build, original-signed release and 22 API35 host checks pass at 320dp/150% font. Before/during tab-return renders are identical. Physical-phone verification remains pending. Refresh Codex App Shelf -> Folio -> Update.

### Previous Folio 1.15.1 update

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
