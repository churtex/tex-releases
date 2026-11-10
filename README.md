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
### Download Tex Suite 0.69.50

| System | File | Fingerprint (SHA-256) |
|---|---|---|
| Windows 10 / 11 | [Tex-Suite-Setup-0.69.50.exe](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.50/Tex-Suite-Setup-0.69.50.exe) | `6c2fdbb9cabd7a4023e3e079d00d4f46d8ef81070ad1a3113a34388b85dbf948` |
| Ubuntu, Linux Mint, Debian | [tex-suite_0.69.50-1_amd64.deb](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.50/tex-suite_0.69.50-1_amd64.deb) | `cd2c1ce0f4de17528ee1e7fdba7f93b7293991fb4383c51d5c2f3ca3ad0bb61d` |
| Fedora, AlmaLinux, openSUSE | [tex-suite-0.69.50-1.x86_64.rpm](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.50/tex-suite-0.69.50-1.x86_64.rpm) | `a2991f2fe5304afebbecc5c8770dd7c64a3f04853c5ab7b24bee36883a1ca782` |
| Any Linux | [tex-suite-0.69.50-linux-x86_64.tar.gz](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.50/tex-suite-0.69.50-linux-x86_64.tar.gz) | `61137abb8498cfe9ae5c80dc654d5c42f91383877ce2051f4396ffb2febe6fb2` |

**Check your file before you open it**, whether you downloaded it or got it
from someone on a flash disk; no internet is needed once you have this page:

- Windows: `certutil -hashfile Tex-Suite-Setup-0.69.50.exe SHA256`
- Linux: `sha256sum tex-suite_0.69.50-1_amd64.deb` (or the file you have)

The answer must be exactly the fingerprint above. If it differs, the file
was changed: delete it. Each file also has a `.sig` signature beside it and a
line in [SHA256SUMS](https://github.com/churtex/tex-releases/raw/main/tex-suite/0.69.50/SHA256SUMS), signed with Churtex's release key
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
