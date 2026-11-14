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
### Download Tex Suite 0.73.2

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [TexMe-Setup-0.73.2.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.2/TexMe-Setup-0.73.2.msi) | `fdb61386685384584e2e6ffc2ae27c78e87f093e4192e863c2b7b1d54a00d42b` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.73.2-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.2/tex-suite_0.73.2-1_amd64.deb) | `9b566aa94d4250ec1996df5d1dc0e0120c751457b61856088b0a700590b6e4c2` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.73.2-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.2/tex-suite-0.73.2-1.x86_64.rpm) | `eeca62eadea5557e6361c5f8d339e5cf00e396d69b85608a46c029ee8d8b15e1` |
| Any Linux | [tex-suite-0.73.2-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.2/tex-suite-0.73.2-linux-x86_64.tar.gz) | `5b85e027188878c0a9c4a304cf83d064a0c2b7aae1ac3ecd8cc22d8b975538c3` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile TexMe-Setup-0.73.2.msi SHA256`
- Linux: `sha256sum tex-suite_0.73.2-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.73.2/SHA256SUMS), signed with Churtex's release key
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
