# TraceMark v1.0 (Windows)

TraceMark is a desktop tool that issues invisibly fingerprinted copies of a PDF, one
per recipient, and later identifies which recipient a leaked copy came from. The text
of every copy stays selectable, copyable and searchable. It is a private academic
prototype built for the IE3092 Information Security Project and is shared here only
with invited testers.

This repository holds **only the ready-to-run application**. There is nothing to
build or install.

## Requirements

- Windows 11, 64-bit
- A local NTFS drive with at least 5 GB free for the workspace. Don't use OneDrive,
  Dropbox, Google Drive or network drives.
- No Python or other software is needed.

## Install and run

1. Open **Releases** (right-hand side of this page) → **v1.0** and download
   `TraceMark-v1.0-windows-x64.zip`.
2. Check the download in PowerShell. The value must match the one in the release notes:
   ```powershell
   (Get-FileHash .\TraceMark-v1.0-windows-x64.zip -Algorithm SHA256).Hash
   ```
3. Right-click the zip → **Extract All…** Put the extracted folder somewhere
   permanent, for example `C:\TraceMark\`. Keep the folder whole; `TraceMark.exe`
   will not run without the `_internal` folder next to it.
4. Double-click `TraceMark.exe`.
   - The app is not code-signed, so Windows SmartScreen may show *"Windows protected
     your PC"*. Click **More info** → **Run anyway**.

## Before using real documents

Read `OPERATIONS.md` inside the extracted folder. It covers the recommended
workstation setup (BitLocker / Device Encryption, a Windows Firewall outbound block
for `TraceMark.exe`, workspace placement) and what TraceMark does not protect against.
`SECURITY.md` in the same folder is the full security design.

## Integrity

The extracted folder contains `SHA256SUMS.txt` (one line per file) and
`BUILD-IDENTITY.json`. `OPERATIONS.md` §1a shows how to check every file from
PowerShell.

## License

All rights reserved. See [LICENSE](LICENSE). Third-party components are listed in
[THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
