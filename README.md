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
### Download Tex Suite 1.0.4

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-1.0.4.msi](https://churtex.org/download/1.0.4/Churtex-Setup-1.0.4.msi) | `8975ffc7d9a71f8855171432cdd28ebff68251f79f2cf13a30e495a89670e421` |
| Ubuntu, Linux Mint, Debian | [tex-suite_1.0.4-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.4/tex-suite_1.0.4-1_amd64.deb) | `5a7d1174e2f63fdaee15a035c2a5f38378cc79c40ab126c6d9c7f45ace65c5a8` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-1.0.4-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.4/tex-suite-1.0.4-1.x86_64.rpm) | `f074d9cf95658ea59583dd3a5e5ee2212c0eb1f34f727701395747a27c701c9a` |
| Any Linux | [tex-suite-1.0.4-linux-x86_64.tar.xz](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.4/tex-suite-1.0.4-linux-x86_64.tar.xz) | `fa9bf0f78a571ba2b5b10eaea6373fa90199b8949675eedbe46435d46acd1875` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-1.0.4.msi SHA256`
- Linux: `sha256sum tex-suite_1.0.4-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.4/SHA256SUMS), signed with Churtex's release key
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
