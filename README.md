# LANCOM

**Next Gen LAN Messenger**

LANCOM brings conversations and file sharing to your local network. Connect Windows PCs and Android devices, discover nearby colleagues, and exchange messages and files directly—without a cloud messaging account or a central relay server.

Developed by **TwoFish Studios**. Lead developer: **Rohan Vasava**.

[Website](https://www.lancom.uk) · [TwoFish Studios](https://www.twofishstudios.com) · [Contact](mailto:contact@twofishstudios.com)

## Latest release

### LANCOM V5 RC86 — Windows & Android

This release combines the Windows V5 RC86 release candidate with the Android 1.2.4 release.

| Platform | Version | Package | Requirements |
| --- | --- | --- | --- |
| Windows | 5.0.0-rc.86 | `LANCOM-Setup-5.0.0-rc86-x64.exe` | Windows 10/11, x64 |
| Android | 1.2.4 | `LANCOM-Android-1.2.4.apk` | Android 8.0 or later |

Download the installers from the [GitHub Releases page](https://github.com/raw-tech-IT/LanCom-Releases/releases) or the [official LANCOM website](https://www.lancom.uk).

### SHA-256 checksums

| File | SHA-256 |
| --- | --- |
| `LANCOM-Setup-5.0.0-rc86-x64.exe` | `23DF8698B99E78CB32991929DA5A8E66CC6490B2F2821E438D27D0A76806C2EB` |
| `LANCOM-Android-1.2.4.apk` | `C2BC27C976D1A295991BAED328E3F1957341BAC83DEBC381AEEA7D9BAD7568C4` |

The checksum file is also available as [SHA256SUMS.txt](SHA256SUMS.txt).

## Features

- **Direct conversations:** Send messages between LANCOM users on the same reachable local network, with conversation history and delivery/read status.
- **Nearby users and presence:** Discover active devices and see availability, profile pictures and status notes.
- **Encrypted file sharing:** Send files directly between Windows and Android, review incoming requests and follow transfer progress inside conversations.
- **Transfer controls:** Accept, decline or cancel transfers, choose where received files are saved, and open completed downloads.
- **Personal profiles:** Set your display name, picture and presence. Windows also supports role badges, including uploaded PNG/JPG badges with optional titles.
- **Notifications:** Receive message and file alerts, with platform notification controls and sound preferences.
- **Local-first operation:** Messaging and transfers work without internet access when both devices can reach each other on the LAN.

## Windows features

- Drag files into a conversation to prepare a transfer, with a drop area that follows the selected theme.
- Send messages to an offline recipient; delivery is retried when the recipient returns and both apps are reachable.
- Prepare files for offline recipients, with Pending status in chat and Transfers. The receiver's acceptance preferences still apply when the request arrives.
- Receive duplicate filenames safely as `filename(1).ext`, `filename(2).ext` and so on, preserving existing files.
- View recent transfers and LANCOM's own upload/download activity, alongside the selected network link's reported speed.
- Choose themes, notification preferences and optional animations. Animations are off by default.
- Keep LANCOM available in the system tray and choose whether it starts with Windows.
- Back up and restore your profile, preferences, conversations and transfer records with a password-protected backup.
- Protect the local message and transfer database with encryption at rest.

## Platform availability

| Capability | Windows | Android |
| --- | --- | --- |
| Direct text messages and conversation history | Yes | Yes |
| Encrypted Windows–Android file transfers | Yes | Yes |
| Active users, presence and shared profile pictures | Yes | Yes |
| In-chat file requests and transfer progress | Yes | Yes |
| Offline outgoing message/file delivery | Yes | Receives when connected |
| Custom badge creation | Yes | Displays shared badges |
| Password-protected backup and restore | Yes | Not currently available |
| Application-level database encryption | Yes | Not currently available |

## Get started

1. Download the Windows installer or Android APK from this repository's **Releases** page or [lancom.uk](https://www.lancom.uk).
2. Install LANCOM on the devices you want to connect.
3. Connect the devices to the same local network and open the app.
4. Set your display name and profile, then choose someone from **Active Users** to start a conversation.
5. Use the attachment button to share a file. On Windows, you can also drag files into the conversation.

**Windows:** Use the x64 installer on Windows 10 or Windows 11. The download includes the required application runtime. The Windows installer is currently unsigned; download it only from the project's official distribution and compare the supplied SHA-256 checksum.

**Android:** Requires Android 8.0 or later. Install the signed APK using Android's installation flow. Allow notifications if you want message and file alerts. Android may keep an ongoing service notification while LANCOM is listening for peers.

Both devices must be able to communicate directly. Guest Wi-Fi, client isolation, VPN routing or firewall rules can prevent discovery. Internet access alone does not connect users on separate networks.

## Files, offline delivery and history

Offline delivery requires the sender and receiver to be online and reachable at the same time. For pending files, keep the original file in place and unchanged until it is sent. A file request does not bypass the receiver's acceptance settings.

Windows backups include settings, profile data, conversations and transfer records. They do not include the contents of files you sent or downloaded. Keep those files separately, and retain your backup password.

The network link rate is different from actual transfer speed. Wi-Fi conditions, the other device, storage performance and concurrent activity affect throughput.

## Security and privacy

Messages and file transfers use AES-256-GCM authenticated encryption. Session keys are established using P-256 ECDH and HKDF-SHA-256. Device identities are remembered after first contact, and unexpected identity changes are rejected. For sensitive use, independently verify the other device's identity; first-contact trust alone does not verify a person's identity.

Windows encrypts its local history database and supports password-protected backups. Android currently stores history in its application-private storage without a separate application-level database encryption layer. Files saved outside LANCOM follow the destination's operating-system protections.

LANCOM is designed for direct local communication. It does not provide cloud delivery when the sender is unavailable. Keep your devices and operating systems secured and updated.

## Help and feedback

- Website: [www.lancom.uk](https://www.lancom.uk)
- Studio: [www.twofishstudios.com](https://www.twofishstudios.com)
- Email: [contact@twofishstudios.com](mailto:contact@twofishstudios.com)

For bug reports, include your LANCOM version, operating system, the steps to reproduce the issue, and a screenshot if useful. Avoid sharing private conversations, passwords or identity keys. Contact TwoFish Studios for licensing and redistribution enquiries.

---

Copyright © TwoFish Studios. All rights reserved.
