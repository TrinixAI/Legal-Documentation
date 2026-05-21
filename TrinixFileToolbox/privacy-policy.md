# Privacy Policy

**Trinix File Toolbox**
A desktop product of Srdjan Lopez LLC dba Trinix AI ("SL LLC," "Trinix AI," "we," "us," "our")
Website: <https://trinix.gg>
Support: <support@trinix.gg>
Effective Date: 2026-05-20
Version: 1.0

---

## 1. Overview

Trinix File Toolbox is a local-first Windows productivity utility that
converts, merges, and processes documents and other files entirely on the
user's own device. This Privacy Policy explains what the Software does and
does not do with your information.

The short version: **no account, no telemetry, no cloud upload, no tracking.**
The detail follows.

## 2. Information We Do Not Collect

We do not collect, store on our servers, transmit, or share:

- Your name, email address, phone number, mailing address, or other identity data.
- Your file contents. Files you process remain on your device.
- File paths from your computer.
- Telemetry, usage analytics, crash reports, feature engagement, or session data,
  except as described in Section 4 ("Diagnostics Export"), which is strictly
  user-initiated.
- IP addresses, device identifiers, or advertising identifiers.
- Any data collected via cookies, tracking pixels, or third-party SDKs. The
  Software does not embed any third-party analytics or advertising SDKs.

We do not maintain user accounts. The Software does not require sign-in.

## 3. Local Data Stored on Your Device

The Software writes the following data to your device only. It is never
transmitted off your device by us.

- **Application settings.** A JSON settings file stored under
  `%APPDATA%\Trinix\FileToolbox` (PyInstaller builds) or under the per-package
  `LocalState` folder (future Microsoft Store MSIX build). Contains UI
  preferences such as theme, font scale, performance mode, output folder, and
  feature toggles.
- **Recent jobs list.** A short history of recent operations. Only file
  **basenames** are stored, never full file paths.
- **Optional thumbnail cache.** If a feature generates thumbnails, they are
  cached locally for performance and can be cleared from Settings.
- **Local performance readings.** While the app is running, it may read local
  process metrics (CPU, memory) via the `psutil` library to display in the
  Settings page. These readings are not stored persistently and are never
  transmitted.

You may delete any of this data at any time by clearing the relevant cache
from Settings, deleting the `%APPDATA%\Trinix\FileToolbox` folder, or
uninstalling the Software.

## 4. Diagnostics Export

The Software includes a diagnostics export feature intended to help us
resolve a problem you report to us. It is strictly **user-initiated**.

- You must click an explicit "Export Diagnostics" action.
- You choose the destination folder where the diagnostics file is saved.
- The file is saved locally only. The Software does not upload it.
- It is your decision whether to send the file to <support@trinix.gg>.

A diagnostics export may contain: application version, Windows version,
recent application log lines, last error trace, and non-identifying system
information such as CPU model and total RAM. It does not contain file paths
of files you processed, file contents, account identifiers, or any data the
Software does not already have access to in normal operation.

## 5. Third-Party Components

The Software is built on open-source components including Qt/PySide6,
pikepdf (with QPDF), pypdfium2 (with PDFium), ReportLab, Pillow, and
psutil. These components run locally inside the Software's own process
and do not transmit data on their own. A complete list of third-party
components and their licenses is in
[Third-Party Notices](third-party-notices.md).

Some features may use programs you install yourself (for example, **FFmpeg**
for audio conversion). When the Software invokes such a program, it does so
as a local subprocess on your machine. The Software does not send your files
to any external service.

## 6. Data Sharing and Disclosure

Because we do not collect personal data, we do not sell, rent, trade, or
share personal data. Aggregated, anonymous, or operational disclosures that
are technically possible could occur only in the following cases:

- When required to comply with applicable law, such as a valid subpoena.
- In connection with a business transaction such as a merger or asset sale,
  in which case we will provide notice where practicable.

In practice, we have no user data to disclose.

## 7. Children's Privacy

The Software is suitable for general audiences. It does not knowingly
collect data from any user, regardless of age, because it does not collect
data at all.

## 8. Security

The Software performs file operations locally using atomic writes to user-writable
folders and does not open network listeners. We make no representation that any
software is free from defects or vulnerabilities, and we cannot guarantee that
your device or operating system is secure. You are responsible for securing your
own device, including operating system updates and antivirus protection.

## 9. Your Rights

Because we do not collect or store personal data on our servers, there is no
server-side data to access, correct, port, or delete. You may at any time:

- Clear local caches from the Software's Settings page.
- Delete the local data folder described in Section 3.
- Uninstall the Software.

For questions about this Privacy Policy, contact <support@trinix.gg>.

## 10. Changes to This Privacy Policy

We may revise this Privacy Policy from time to time. Updated versions will
be published in this repository and at
<https://trinix.gg/legal/file-toolbox/privacy-policy>, with a revised effective
date. Continued use of the Software after the effective date constitutes
acceptance of the revised policy.

## 11. Contact

For privacy-related questions or requests, contact:
**<support@trinix.gg>**

---

© 2025-2026 Srdjan Lopez LLC dba Trinix AI. All Rights Reserved.
