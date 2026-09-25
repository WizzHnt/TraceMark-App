# Third-party notices

The TraceMark v1.0 bundle (`TraceMark-v1.0-windows-x64`) contains the components
below, each under its own license. Versions are the exact pins the bundle was built
from. Where a component ships its license text, that text is inside `_internal\`.

| Component | Version | License |
|---|---|---|
| Python runtime | 3.12.10 | PSF-2.0 |
| Qt 6 / PySide6 / Shiboken6 | 6.8.1 | LGPL-3.0 |
| pikepdf (with qpdf) | 9.5.2 | MPL-2.0 (qpdf: Apache-2.0) |
| pdfminer.six | 20260107 | MIT |
| pypdfium2 (with PDFium) | 5.12.1 | Apache-2.0 or BSD-3-Clause; PDFium: BSD-3-Clause |
| opencv-python-headless | 4.10.0.84 | Apache-2.0 |
| NumPy | 2.1.3 | BSD-3-Clause |
| SciPy | 1.14.1 | BSD-3-Clause |
| scikit-image | 0.24.0 | BSD-3-Clause |
| Pillow | 12.3.0 | MIT-CMU |
| lxml | 6.1.2 | BSD-3-Clause |
| cryptography | 50.0.0 | Apache-2.0 or BSD-3-Clause |
| argon2-cffi | 23.1.0 | MIT |
| SQLAlchemy | 2.0.36 | MIT |
| Alembic | 1.14.0 | MIT |
| Mako | 1.4.1 | MIT |
| MarkupSafe | 3.0.3 | BSD-3-Clause |
| greenlet | 3.5.5 | MIT and PSF-2.0 |
| charset-normalizer | 3.5.1 | MIT |
| PyYAML | 6.0.3 | MIT |
| Source Sans 3, Source Code Pro fonts (Adobe) | bundled | SIL Open Font License 1.1 |
| Microsoft Visual C++ runtime (`VCRUNTIME140*.dll`) and Universal CRT (`api-ms-win-*.dll`) | bundled | Microsoft redistributable |

## LGPL-3.0 (Qt / PySide6)

Qt and PySide6 are used unmodified and loaded as separate shared libraries
(`_internal\PySide6\*.dll`, `_internal\shiboken6\`). You may swap in your own
compatible build of these libraries. The Qt source code is available from
https://download.qt.io/official_releases/qt/ and the PySide6 source from
https://download.qt.io/official_releases/QtForPython/.

## MPL-2.0 (pikepdf)

pikepdf is used unmodified. Its source code is available from
https://github.com/pikepdf/pikepdf.

## Fonts

The full SIL Open Font License texts are in
`_internal\app\ui\assets\fonts\LICENSE-SourceSans3.md` and
`LICENSE-SourceCodePro.md`.
