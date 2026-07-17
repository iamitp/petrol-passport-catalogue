# My Petrol Passport — vehicle catalogue (data only)

Over-the-air catalogue for the My Petrol Passport iOS app. Served via GitHub Pages:

- `v2/vehicles.json` — the source-backed vehicle evidence catalogue
- `v2/MANIFEST.json` — integrity manifest (sha256, record count, sources-checked date)

Every record cites its sources (issuer, date, URL, scope, caveats). The app verifies
the manifest hash before accepting any update and falls back to its bundled catalogue
otherwise. No user data flows through this repo — it is a one-way data feed.

Data licence: the catalogue compiles facts from cited public sources; the compilation
is provided as-is, with no warranty. It is not a vehicle certification.
