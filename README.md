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
### Download Tex Suite 1.0.0

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-1.0.0.msi](https://churtex.org/download/1.0.0/Churtex-Setup-1.0.0.msi) | `5796ac25d4894937289a93eada2aca4e9a560cae4b17f7c5acf24bbbc2790f4e` |
| Ubuntu, Linux Mint, Debian | [tex-suite_1.0.0-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.0/tex-suite_1.0.0-1_amd64.deb) | `c63d3a3b15ea1f192eaa60437b1f4fd7712c9b48b372f1263d1d7955a4b700a2` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-1.0.0-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.0/tex-suite-1.0.0-1.x86_64.rpm) | `4ff7ea8e42d6c32649907d61ba90075aa07bd252fb5ca292c8443d29e6aa32ee` |
| Any Linux | [tex-suite-1.0.0-linux-x86_64.tar.xz](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.0/tex-suite-1.0.0-linux-x86_64.tar.xz) | `a6fe96ce6e845c73bb10d3c2c832315decb85aabbcd8b886169782ea4bb4c054` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-1.0.0.msi SHA256`
- Linux: `sha256sum tex-suite_1.0.0-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/1.0.0/SHA256SUMS), signed with Churtex's release key
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
