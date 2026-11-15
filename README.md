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
### Download Tex Suite 0.73.3

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [TexMe-Setup-0.73.3.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.3/TexMe-Setup-0.73.3.msi) | `40a4ab4a2f01bf07fc9c238907ee6fafc7fb4f4251d1c3de531fd863d68362fa` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.73.3-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.3/tex-suite_0.73.3-1_amd64.deb) | `f14c5622fd2fd1bf8de6b1dc92fa304e78491aa5fdeddb0180d947a9be5ca2fa` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.73.3-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.3/tex-suite-0.73.3-1.x86_64.rpm) | `6b74b00855de7de7a210187688de003696f093df819e0f199bd1b57453209b5b` |
| Any Linux | [tex-suite-0.73.3-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.3/tex-suite-0.73.3-linux-x86_64.tar.gz) | `412edc978d075175b395c69fa622de9b9642faf1cdf7570d76b1250b1ac49533` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile TexMe-Setup-0.73.3.msi SHA256`
- Linux: `sha256sum tex-suite_0.73.3-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.3/SHA256SUMS), signed with Churtex's release key
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
