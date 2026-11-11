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
### Download Tex Suite 0.72.0

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [TexMe-Setup-0.72.0.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.72.0/TexMe-Setup-0.72.0.msi) | `f4adbb145a51e9ac1f4fee4e8f29a8e2c2f2983fde3b2077c8eb3138a170db37` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.72.0-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.72.0/tex-suite_0.72.0-1_amd64.deb) | `310ce07de653a574abc13b6efe9d6cfd6d79d406363a2d187770143e3178204e` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.72.0-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.72.0/tex-suite-0.72.0-1.x86_64.rpm) | `a48c9749bbf53b51b269ec4d455b6550f6095fc90f70453516f4d189cdc79739` |
| Any Linux | [tex-suite-0.72.0-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.72.0/tex-suite-0.72.0-linux-x86_64.tar.gz) | `117abca57257c765374489b6bf301c3337747d2323b0bc09edd8092ce12f7552` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile TexMe-Setup-0.72.0.msi SHA256`
- Linux: `sha256sum tex-suite_0.72.0-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.72.0/SHA256SUMS), signed with Churtex's release key
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
