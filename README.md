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
### Download Tex Suite 0.69.49

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.49.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.49/Tex-Suite-Setup-0.69.49.exe) | `4405818a4ef41d39f8be6beab674a5b2defa885dd95a68dff3234f2936544180` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.49-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.49/tex-suite_0.69.49-1_amd64.deb) | `f2f003fa8896b8c4674441f7827fbfa32f5f5e1ca6cfd7637213b4f01d8b239e` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.49-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.49/tex-suite-0.69.49-1.x86_64.rpm) | `0609e1215255b67687e6aa239f63b05c980cc5bc957ab4c3a28637bbec2fa327` |
| Any Linux | [tex-suite-0.69.49-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.49/tex-suite-0.69.49-linux-x86_64.tar.gz) | `0f2608cc6255c271e415a0ba725d24b7256aa9c5000c102f5cdf1241f31c6272` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.49.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.49-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.49/SHA256SUMS), signed with Churtex's release key
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
