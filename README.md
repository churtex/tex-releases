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
### Download Tex Suite 0.69.46

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.46.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.46/Tex-Suite-Setup-0.69.46.exe) | `403ef6d434bbcfad5c174e70e0e9f48107183838b01f7a6bbe06f6c33b1b19c9` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.46-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.46/tex-suite_0.69.46-1_amd64.deb) | `4467a00e3d0dda007d7fb8aaf8a677a7bb84ebce94ef41847e2be0c723c43a20` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.46-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.46/tex-suite-0.69.46-1.x86_64.rpm) | `1e6e45891029f9765e60badf4cf9174173b6ba5c80e8173c37874dffa11b62ba` |
| Any Linux | [tex-suite-0.69.46-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.46/tex-suite-0.69.46-linux-x86_64.tar.gz) | `15004e5cafd5672d19fd267ac0070ebc3f6cd5838fa4f7e10a5086350e663983` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.46.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.46-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.46/SHA256SUMS), signed with Churtex's release key
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
