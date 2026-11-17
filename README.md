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
### Download Tex Suite 0.76.1

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-0.76.1.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.76.1/Churtex-Setup-0.76.1.msi) | `b69e22081a6e78e7566a37cce5ed1e2ad9fefc944d44c29c0f4a70bd544944fd` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.76.1-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.76.1/tex-suite_0.76.1-1_amd64.deb) | `9b7a63f0b448375f5877b46ce9193c4662dfd412d29ee0f4fdeab29fc4ef614b` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.76.1-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.76.1/tex-suite-0.76.1-1.x86_64.rpm) | `cfa8ca98d3bf5391b83108183fb3391716048631983dc5507b510e4cd7fb14a7` |
| Any Linux | [tex-suite-0.76.1-linux-x86_64.tar.xz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.76.1/tex-suite-0.76.1-linux-x86_64.tar.xz) | `33230befe461912008f149fccd960aa191e048cbf48e9241fdb47ee70f30dadb` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-0.76.1.msi SHA256`
- Linux: `sha256sum tex-suite_0.76.1-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.76.1/SHA256SUMS), signed with Churtex's release key
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
