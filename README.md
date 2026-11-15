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
### Download Tex Suite 0.75.1

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Churtex-Setup-0.75.1.msi](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.75.1/Churtex-Setup-0.75.1.msi) | `5f385405fe761ba08d1fd98292cab3acfd11189220c006207391a32313d22bcd` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.75.1-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.75.1/tex-suite_0.75.1-1_amd64.deb) | `e92238d94c4fd4ad1f92a49bac215d0145aa3c0eee020fab5070474025fe5dda` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.75.1-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.75.1/tex-suite-0.75.1-1.x86_64.rpm) | `80a6beb7558bf216a7d0e3e1eea5896f7fb030de164df56e1c955c997ecf44bd` |
| Any Linux | [tex-suite-0.75.1-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.75.1/tex-suite-0.75.1-linux-x86_64.tar.gz) | `88119dacb49716ec2df08e8ce6b411aee7ddf5742c25c7e4ef3d0f05d3ae43e1` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Churtex-Setup-0.75.1.msi SHA256`
- Linux: `sha256sum tex-suite_0.75.1-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.75.1/SHA256SUMS), signed with Churtex's release key
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
