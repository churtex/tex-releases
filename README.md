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
### Download Tex Suite 0.69.47

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.47.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.47/Tex-Suite-Setup-0.69.47.exe) | `f2074b0802b7cab0cb4cc2d26cffbc99975848937d4efc5a43f57dc1f1790241` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.47-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.47/tex-suite_0.69.47-1_amd64.deb) | `50b70412140cb0f2790e44096b6bfd59e6b00c2ae80b952193612bb6319e3de9` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.47-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.47/tex-suite-0.69.47-1.x86_64.rpm) | `6efd575c5bcde52fd04253430ac5e4717513ae7993f53e30bd4939304fc44ffc` |
| Any Linux | [tex-suite-0.69.47-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.47/tex-suite-0.69.47-linux-x86_64.tar.gz) | `7e901ffdd4b4b56bf89f2194b1acd4ca100947e3f71baabf539ed4a01b54fe37` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.47.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.47-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.47/SHA256SUMS), signed with Churtex's release key
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
