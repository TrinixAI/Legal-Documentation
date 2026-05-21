# Third-Party Notices

**Trinix File Toolbox**
A desktop product of Srdjan Lopez LLC dba Trinix AI
Effective Date: 2026-05-21
Version: 1.1

Trinix File Toolbox includes or interoperates with the following third-party
components. We are grateful to the maintainers and contributors of each
project.

> **Change history:** Version 1.1 (2026-05-21) replaces the PyMuPDF (`fitz`)
> entry with the new permissive PDF stack (`pikepdf` + QPDF, `pypdfium2` +
> PDFium, ReportLab). PyMuPDF is no longer part of the runtime distribution.

This document does not modify the licenses below. In the event of conflict,
the upstream license text controls.

---

## 1. PySide6 / Qt for Python

- Project: <https://doc.qt.io/qtforpython/>
- License: GNU Lesser General Public License v3.0 (LGPL-3.0) or commercial.
- Use in Software: GUI framework, dynamically linked.
- Obligations satisfied by: dynamic linking, ability to relink with a
  modified PySide6 build, inclusion of this attribution and the LGPL-3.0
  notice.

## 2. Qt (underlying C++ libraries)

- Project: <https://www.qt.io/>
- License: GNU Lesser General Public License v3.0 (LGPL-3.0) or commercial.
- Use in Software: native GUI runtime under PySide6.
- Obligations satisfied by: same as PySide6 above.

## 3. pikepdf (and QPDF)

- Project: <https://pikepdf.readthedocs.io/>
- Upstream library: QPDF (<https://qpdf.sourceforge.io/>).
- License: **Mozilla Public License 2.0 (MPL-2.0)** for pikepdf, over
  **Apache License 2.0** for the QPDF C++ library that pikepdf statically
  links into its wheel.
- Use in Software: structural PDF operations (merge, split, extract,
  delete, reorder, range-split, page count, encryption status), lossless
  compression, metadata read/write, XMP read/write/delete, annotation
  removal, embedded-file removal, and document-level JavaScript / named
  action removal. All calls are routed through
  `trinix_toolbox/core/pdf_backend.py`.
- Obligations satisfied by: dynamic redistribution of the upstream
  pikepdf wheel without modification. MPL-2.0 file-level copyleft does
  not propagate to the rest of the application; Apache-2.0 obligations
  for QPDF are satisfied by retaining the upstream NOTICE file as
  shipped inside the pikepdf wheel.

## 4. pypdfium2 (and PDFium)

- Project: <https://pypdfium2.readthedocs.io/>
- Upstream library: PDFium (<https://pdfium.googlesource.com/pdfium/>),
  the same renderer used by Google Chrome and Microsoft Edge.
- License: **Apache License 2.0 OR BSD 3-Clause** for the pypdfium2
  Python wrapper, over **BSD 3-Clause** for the PDFium engine binary
  shipped inside the wheel.
- Use in Software: PDF rasterization (PDF to PNG/JPG) and per-page text
  extraction (PDF to TXT). Read-only.
- Obligations satisfied by: dynamic redistribution of the upstream
  pypdfium2 wheel without modification, including the bundled
  `pdfium.dll` and the upstream LICENSE/NOTICE files.

## 5. ReportLab (open-source edition)

- Project: <https://www.reportlab.com/opensource/>
- License: **BSD 3-Clause**.
- Use in Software: PDF synthesis from text input (TXT to PDF, Merge
  Text to PDF). The bundled font files (Type 1 cores) ship inside the
  ReportLab wheel under the same BSD-3-Clause grant.
- Obligations satisfied by: dynamic redistribution of the upstream
  ReportLab wheel without modification, including its LICENSE file.

## 6. Pillow

- Project: <https://python-pillow.org/>
- License: Historical Permission Notice and Disclaimer (HPND).
- Use in Software: image handling for the Images-to-PDF and PDF-to-Image
  paths and for in-memory raster handoff between pypdfium2 and disk.

## 7. psutil

- Project: <https://github.com/giampaolo/psutil>
- License: BSD 3-Clause.
- Use in Software: local process and system metrics displayed in Settings.
  Readings are not stored or transmitted.

## 8. PyInstaller

- Project: <https://pyinstaller.org/>
- License: GPL with a runtime exception that allows distribution of the
  resulting frozen application under the application's own license terms.
- Use in Software: build tool that produces the distributable Trinix File
  Toolbox executable. Not part of the runtime distribution itself except
  for its bootloader.

## 9. FFmpeg (optional, user-installed)

- Project: <https://ffmpeg.org/>
- License: LGPL-2.1+ or GPL-2.0+ depending on the build.
- Use in Software: invoked as a separate process **only if** the user
  installs FFmpeg themselves and makes it available on `PATH`. Trinix File
  Toolbox does not ship, bundle, or download FFmpeg in this version. If
  bundling is introduced in a future version, full attribution and the
  appropriate license text will be included with the distribution.

## 10. Python

- Project: <https://www.python.org/>
- License: Python Software Foundation License (PSFL).
- Use in Software: runtime, bundled by PyInstaller.

---

## Trademark Notices

"Trinix," "Trinix AI," and "Trinix File Toolbox" are unregistered or
registered trademarks of Srdjan Lopez LLC. "Microsoft," "Windows,"
"Microsoft Store," "Partner Center," and related names are trademarks of
Microsoft Corporation. All other product names, logos, and brands are
property of their respective owners.

---

© 2025 – 2026 Srdjan Lopez LLC dba Trinix AI. All Rights Reserved.
