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
### Download Tex Suite 0.69.48

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.48.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.48/Tex-Suite-Setup-0.69.48.exe) | `a1d37863cea79a0057793483e46e2d826ea20cbf66ddda65ec01cc35506501e2` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.48-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.48/tex-suite_0.69.48-1_amd64.deb) | `3555c57a4b2c08637a93bebc40c7309b021f1e3132f3b6dd5525ea0450bdfeba` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.48-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.48/tex-suite-0.69.48-1.x86_64.rpm) | `0cd50e2a759909e14e6947b1bf2da1dbc2cf5fe9a471efe3ace7b0d69bc9d19c` |
| Any Linux | [tex-suite-0.69.48-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.48/tex-suite-0.69.48-linux-x86_64.tar.gz) | `c7b62bf396186d1ba3f9d45f7299155f569697308424790e08df5fbc9c011e42` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.48.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.48-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.48/SHA256SUMS), signed with Churtex's release key
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
