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
### Download Tex Suite 0.69.42

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.42.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.42/Tex-Suite-Setup-0.69.42.exe) | `d0d53feb91b9a861d7f15b992fb48a18551b5db35648fcefcbe984f7461755f0` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.42-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.42/tex-suite_0.69.42-1_amd64.deb) | `83aa4559ab7cfcd93360bc5e69ac579eb27bce542275f0b45a548e848a02469f` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.42-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.42/tex-suite-0.69.42-1.x86_64.rpm) | `1c1ab1bde1756dd5cdfe1ff1bf9b0aa3edb258813864ffb004f69fdf186ab074` |
| Any Linux | [tex-suite-0.69.42-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.42/tex-suite-0.69.42-linux-x86_64.tar.gz) | `a3632fd00ed4fc55f29b7d516400a58d7af4ea63fd9673a302854f4ff81b1b45` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.42.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.42-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.42/SHA256SUMS), signed with Churtex's release key
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
