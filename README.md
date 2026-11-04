# LANCOM — Official Releases

Official release downloads and version information for **LANCOM**, the local-network messenger from TwoFish Studios.

> This repository is dedicated to public release information and downloadable build assets. LANCOM's development source repository remains private.

## Latest release

### LANCOM V5 RC86 — Windows Release Candidate

- **Version:** 5.0.0-rc.86
- **File version:** 5.0.0.86
- **Platform:** Windows x64
- **Installer:** `LANCOM-Setup-5.0.0-rc86-x64.exe`
- **Installer size:** 65,232,896 bytes (approximately 62.22 MiB)
- **SHA-256:** `23DF8698B99E78CB32991929DA5A8E66CC6490B2F2821E438D27D0A76806C2EB`
- **Source revision:** `ad702aa02040a288440ba6ea90390b80635193ad`

**Release status:** Release Candidate. This is not a production, security, or scale certification.

The installer asset will be linked here when the GitHub Release is published.

## Other platform builds

| Platform | Build | Status |
|---|---|---|
| Windows x64 | 5.0.0-rc.86 | Release Candidate |
| Android | 1.2.4-preview (code 8) | Preview build |
| Ubuntu | — | Coming soon |
| macOS | — | Coming soon |

The Android preview is a separate version line; it is not Android version 5.0.0-rc.86. Its APK has not yet been published as a release asset.

## Validation and known limitations

For Windows RC86:

- 34 existing Windows title, profile, and settings checks passed.
- Installer payload verification passed.
- Isolated packaged-app launch passed.
- The previous Alpha85 full-suite report recorded 1,618 passed tests.
- The full test suite was not rerun for RC86; this revision contains credits and title presentation changes.
- The Windows installer is currently unsigned.
- No host installation or peer-send testing was performed for this revision.

For Android 1.2.4-preview:

- Build and lint completed with 0 errors and 30 existing warnings.
- The APK uses the existing development preview signing key.
- No phone installation or Android unit/instrumentation test rerun was performed for this copy-only change.

See [CHANGELOG.md](CHANGELOG.md) for the release notes.

## Verify your download

After downloading the Windows installer, calculate its SHA-256 hash and compare it with the value above.

PowerShell:

```powershell
Get-FileHash .\LANCOM-Setup-5.0.0-rc86-x64.exe -Algorithm SHA256
```

Only install software obtained from the official LANCOM website or this official release repository.

## Official links

- Website: https://www.lancom.uk/
- Releases: https://github.com/raw-tech-IT/LanCom-Releases/releases
- Publisher: TwoFish Studios

---

Copyright © TwoFish Studios. All rights reserved.
