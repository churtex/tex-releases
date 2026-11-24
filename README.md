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
### Download Tex Suite 0.77.0

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-0.77.0.msi](https://churtex.org/download/0.77.0/Churtex-Setup-0.77.0.msi) | `03497eb3699342f981d75a9b587333fed2dc4ea532b74892bf6692218ee343b0` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.77.0-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.77.0/tex-suite_0.77.0-1_amd64.deb) | `bf160b05fe6f1a8a2b892be3a0ef10ea764c298def836d3d869a9ac5b5836e87` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.77.0-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.77.0/tex-suite-0.77.0-1.x86_64.rpm) | `8d7518a5d30df805707412aae6dacffcfee63b197b14ee9005399113baac7b0d` |
| Any Linux | [tex-suite-0.77.0-linux-x86_64.tar.xz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.77.0/tex-suite-0.77.0-linux-x86_64.tar.xz) | `7a9ba2abc842c06044e45aa1211884805fa51948619d5696d07e4ad74ec6b857` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-0.77.0.msi SHA256`
- Linux: `sha256sum tex-suite_0.77.0-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.77.0/SHA256SUMS), signed with Churtex's release key
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
