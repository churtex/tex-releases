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
### Download Tex Suite 1.0.2

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-1.0.2.msi](https://churtex.org/download/1.0.2/Churtex-Setup-1.0.2.msi) | `e2ee299deff4e7ee5090cbaf6c597176d560635e1b8d6f0086c5ab5815f866fa` |
| Ubuntu, Linux Mint, Debian | [tex-suite_1.0.2-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.2/tex-suite_1.0.2-1_amd64.deb) | `dae4372c7b81e211f384d25ea7c912b8d72dfb36030458ebcbb0dc636fab211e` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-1.0.2-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.2/tex-suite-1.0.2-1.x86_64.rpm) | `0c7d04d25d0a5cb9171be277999634611a2042495175ca8baa8fd28c318aa771` |
| Any Linux | [tex-suite-1.0.2-linux-x86_64.tar.xz](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.2/tex-suite-1.0.2-linux-x86_64.tar.xz) | `2bba4ffbb4608deca29f09f9894c3ca7026fbfa6a59e6f0c39be007df7cc12e6` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-1.0.2.msi SHA256`
- Linux: `sha256sum tex-suite_1.0.2-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.2/SHA256SUMS), signed with Churtex's release key
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
