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
### Download Tex Suite 1.0.3

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-1.0.3.msi](https://churtex.org/download/1.0.3/Churtex-Setup-1.0.3.msi) | `99951543c149a5e831f7088cfd5c6decac3482e4d55ce4a05ba602cc261f20a3` |
| Ubuntu, Linux Mint, Debian | [tex-suite_1.0.3-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.3/tex-suite_1.0.3-1_amd64.deb) | `d502fed2cdb12d88a52ec792c475054f2481bc274ad0ad58f51e4eedd615f20b` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-1.0.3-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.3/tex-suite-1.0.3-1.x86_64.rpm) | `a070bed04422c7528ee6e92a9df736031ecf9c94e222f6e536981b78d787384e` |
| Any Linux | [tex-suite-1.0.3-linux-x86_64.tar.xz](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.3/tex-suite-1.0.3-linux-x86_64.tar.xz) | `cfc35f806ac5ba8d7a9768082c37da2ae648c9f4785cae32d872ab0fbbae969f` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-1.0.3.msi SHA256`
- Linux: `sha256sum tex-suite_1.0.3-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.3/SHA256SUMS), signed with Churtex's release key
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
