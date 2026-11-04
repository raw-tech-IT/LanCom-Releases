# LANCOM Release Changelog

This file records public build changes based on the release information supplied for each version.

## [5.0.0-rc.86] — Windows Release Candidate

**Release type:** Release Candidate  
**Platform:** Windows x64  
**Source revision:** `ad702aa02040a288440ba6ea90390b80635193ad`

### Changed

- The About section now lists only Rohan Vasava as Lead Developer.
- Removed the two fictional developer names.
- Retained TwoFish Studios branding, website links, and contact details.
- Updated the Windows title bar to display LANCOM followed by lowercase `v5 rc86` in 12-point regular text beside the 15-point semibold app name.
- Retained all Alpha85 functionality, including safe numbered duplicate downloads.

### Validation

- 34 existing Windows title, profile, and settings checks passed.
- Installer payload verification passed.
- Isolated packaged-app launch passed.
- No new behavior tests or full-suite rerun were performed for this credits/title-only revision.
- The previous Alpha85 full-suite report remains 1,618 passed.
- No host installation or peer sends were performed.

### Known limitations

- The Windows installer is unsigned.
- RC is a release label, not a production, security, or scale certification.
- Prior physical-device, signing, and deployment validation limitations remain.

### Windows installer details

- **Filename:** `LANCOM-Setup-5.0.0-rc86-x64.exe`
- **Size:** 65,232,896 bytes
- **SHA-256:** `23DF8698B99E78CB32991929DA5A8E66CC6490B2F2821E438D27D0A76806C2EB`

## Android preview — 1.2.4-preview (code 8)

This is a separate Android preview build, not the Android equivalent of Windows 5.0.0-rc.86.

### Changed

- The About section now lists only Rohan Vasava.
- The About button remains at the bottom of Settings.

### Validation and limitations

- Build and lint passed with 0 errors and 30 existing warnings.
- APK signature matches the previous preview signer.
- No phone installation or Android unit/instrumentation rerun was performed for this copy-only change.
- Android continues to use the existing development preview key.

### Android APK details

- **Build path supplied:** `release/android-preview/LanCom-Android-1.2.4-preview.apk`
- **SHA-256:** `B17395688759792785236392EC3A8C6752EA72D63088B36FBFB4FD455C1B0BF9`

---

Older Alpha85 test results are included only as historical validation context; they are not a claim that the full suite was rerun for RC86.
