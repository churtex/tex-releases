# Tex releases

Downloads of the **Tex** apps by **Churtex**: offline-first, private by design.

Each app has its own releases here, tagged with its name and version
(for example `tex-suite-v0.41.0`). The apps check this page for updates
only when you allow them to.

## Tex Suite

Your films, music, books, files and private life in one app that works
without the internet: Media, Books, Pedia, Tools, Edu, Anivo and the Vault
(contacts, 2FA codes, passwords), always encrypted.

- Releases: tags `tex-suite-v*`
- Systems: Windows and Linux (Android coming)

<!-- downloads -->
### Download Tex Suite 0.69.43

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.43.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.43/Tex-Suite-Setup-0.69.43.exe) | `e89393bd4ce6817e4bc6333606653ee97f413c93c57b75ddcdcc2025ca22bf10` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.43-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.43/tex-suite_0.69.43-1_amd64.deb) | `e57fe41f918f87dc076dbf633ab74b8c037edce05357fb0c1ec530610771dd5d` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.43-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.43/tex-suite-0.69.43-1.x86_64.rpm) | `d47531cfd9cc1012142bbc13b48d9e5b0057bd62a35c668b0c1dcbca5db047db` |
| Any Linux | [tex-suite-0.69.43-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.43/tex-suite-0.69.43-linux-x86_64.tar.gz) | `eaa7853e1ec6ea6ffabd9d49bfc2bf756705258d450adcba96ecc008ad202dcf` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.43.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.43-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.43/SHA256SUMS), signed with Churtex's release key
(its public key: `91bb465c0e903b6b5638682723e511ab7e83171aea40e2a358b424556c5b9e13`).
Once installed, Tex Suite checks its own signature at every start, and a
changed copy refuses to create a library. Windows may show "Windows
protected your PC" the first time: choose **More info → Run anyway** (the
installer is not yet signed with a Microsoft certificate).
<!-- /downloads -->

## More Tex apps

Coming.

---

Support: support@churtex.org · https://churtex.org
