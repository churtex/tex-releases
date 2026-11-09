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
### Download Tex Suite 0.69.44

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.44.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.44/Tex-Suite-Setup-0.69.44.exe) | `e732c2e690c04f7de2d1eb6b0fa1220715aa861b3e02fead27b9ecaf7630b25b` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.44-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.44/tex-suite_0.69.44-1_amd64.deb) | `a93695b6f0c58c995f9851a168d17a643c1649adc05e942f06134d25c941c7f5` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.44-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.44/tex-suite-0.69.44-1.x86_64.rpm) | `aa9d8cc918ef73e9eb88a74808f5f7ced3e4fd729b85b81ef5cf84e95db4051e` |
| Any Linux | [tex-suite-0.69.44-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.44/tex-suite-0.69.44-linux-x86_64.tar.gz) | `1b24f20fdf80d247a9607949b27af7d78d435d07bee9c530bf9af7142b4e5c1f` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.44.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.44-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.44/SHA256SUMS), signed with Churtex's release key
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
