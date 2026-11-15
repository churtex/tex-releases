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
### Download Tex Suite 0.74.0

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-0.74.0.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.74.0/Churtex-Setup-0.74.0.msi) | `678c294cd62fd607be261cf689ef4296465c2b910ae8d2c23d1cde1210b41ace` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.74.0-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.74.0/tex-suite_0.74.0-1_amd64.deb) | `291b2b2b2ab9b738b1947c69ecc788c12ac05fddbd482122e472e26c9ddf9ef5` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.74.0-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.74.0/tex-suite-0.74.0-1.x86_64.rpm) | `1d457516fd516869271a90e24d7cc3906cd34701fbcac09f9dda094203d11412` |
| Any Linux | [tex-suite-0.74.0-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.74.0/tex-suite-0.74.0-linux-x86_64.tar.gz) | `0a9f99e773fa35654a0646f77620c235153ad8a4af7f14fc6811e976639f4fb5` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-0.74.0.msi SHA256`
- Linux: `sha256sum tex-suite_0.74.0-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.74.0/SHA256SUMS), signed with Churtex's release key
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
