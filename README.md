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
### Download Tex Suite 0.73.0

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [TexMe-Setup-0.73.0.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.0/TexMe-Setup-0.73.0.msi) | `83cc75c51770dd0fc88fc5d9bad77cc9b7a74ea276d600962872cda9304779cc` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.73.0-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.0/tex-suite_0.73.0-1_amd64.deb) | `3a4f6c4ed8c4c5410e2f315f7d43c83ce1561a10b8899fa66ba4016ffdae2c44` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.73.0-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.0/tex-suite-0.73.0-1.x86_64.rpm) | `0b90612fa4c471463b187c09cfa875707871d720b198b18e7c18eb149caa1f15` |
| Any Linux | [tex-suite-0.73.0-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.0/tex-suite-0.73.0-linux-x86_64.tar.gz) | `ccd85897ea2a0d470b5fb8311c07be1f638e5ee0b5393f87e97c2af32dd97dc1` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile TexMe-Setup-0.73.0.msi SHA256`
- Linux: `sha256sum tex-suite_0.73.0-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.0/SHA256SUMS), signed with Churtex's release key
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
