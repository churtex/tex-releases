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
### Download Tex Suite 0.69.2

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.2.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.2/Tex-Suite-Setup-0.69.2.exe) | `7676256b90d22bdaaff4dec6900bba555c325b3dc1d9d71eaf334aa35819d81f` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.2-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.2/tex-suite_0.69.2-1_amd64.deb) | `900b65623a1895c93bada7e175934ea43d0815aae74beccc1c7d671ce0cceb3a` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.2-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.2/tex-suite-0.69.2-1.x86_64.rpm) | `f79e2bd49490ac859026e4f9b4424a9d82c4c0d256ef008a6fe0e752ca78982b` |
| Any Linux | [tex-suite-0.69.2-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.2/tex-suite-0.69.2-linux-x86_64.tar.gz) | `996ce571610782afb8aec3d7cde62bbcbdc9bf19ba53f04588ef68866f4d097e` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.2.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.2-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.2/SHA256SUMS), signed with Churtex's release key
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
