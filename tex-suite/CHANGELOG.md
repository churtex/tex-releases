# Changelog

## 0.50.0 (2026-10-30) - Landscape in halves, reading progress, Anivo on white sheets

- **Landscape reading: one page in two halves** (founder: "one page, but split
  in half so that it becomes landscape"): the page's upper half first, a turn,
  then its lower half; "Page 3 of 10 · upper half". The cut always falls
  between lines (a test checks every line at several sizes); a PDF page is cut
  at a blank row near its middle, never through a line. The two-column sheet
  of 0.49 is gone.
- **Reader arrows click at once** (founder: they would not click while the
  mouse was on them): the page's frame lay over them; they are now on top. The
  page also sits clear of the "Page N of M" label.
- **Books show how much has been read**: a bar on the cover and "42% read" or
  "Finished" under the title.
- **Anivo reads like a document** (founder): a tinted page (#F4F4F4) with
  each reading on a white sheet, half an inch of margin on all sides; verses
  at **18 pt** (24 px, line height 1.5) and lines held to about 68 characters,
  as book typography advises (45-75; Bringhurst; WCAG asks no more than 80).
  The Bible and the daily readings share one look.
- **Anivo: Prayer points in the menu** (a Pray section): today's ticks, add
  and remove, and how many of the last 30 days each point was prayed for.
- **Tex Suite Preview** (`tools/preview.sh`): the next version installed beside
  the real app, to try before a release; it never updates itself and will not
  open while Tex Suite is open (one app at a time on a library).
- Engine: tex-engine 0.30.3 (texts). Dependencies: `cargo update` brought no
  changes beyond the engine.
- Security review: the new code reads only the app's own saved state (reading
  progress, prayer points) and a PDF page's own pixels; it opens no network
  connection and adds no dependency. The preview launcher refuses to open a
  library the real app has open.

## 0.49.0 (2026-10-30) - Sharp text in the reader, a two-column sheet in landscape, prayer points

- **Reader text is sharp** (founder: the text looked fuzzy): pages are no
  longer pictures; the text is drawn live like the rest of Tex Suite, sharp at
  any zoom. Words are measured exactly as they are drawn (a test keeps it so).
- **Landscape: one page as a sheet in two columns** (founder: "split into two
  pieces … the cut is clean"): the text keeps its true size and runs down the
  left column and on at the top of the right; the split is always between
  lines.
- **The page turn is a light paper fold** (founder: too much shadow): the
  folded paper shows its plain back, the next page appears behind the fold,
  and the shading is faint; the text stays sharp throughout.
- **Anivo: prayer points** (founder): write what you pray for and tick each
  point when prayed for; ticks start fresh each day.
- **Anivo: verses** a little larger, in a softer ink (not bold), **justified**,
  with a little letter spacing.
- Engine: tex-engine 0.30.2.

## 0.48.0 (2026-10-30) - The reader, one page at a time; updates found at once

- **The reader, as the founder asked after trying 0.46**: always **one page**
  (no two-page view), opening **on the cover** (with "Continue from page …" for
  a book read before), **‹ and › beside the page** that turn it with a quick,
  clean flip round its edge (no ‹ on the cover, no › on the last page), and
  **zoom** (− +, Fit page, Fit width, Ctrl + wheel, a pinch): zoomed in, the
  page scrolls up and down. Text laid out at the size it is shown, so it reads
  at its true size. Paper, Sepia, Night, text size; kept for every book.
- **Updates found at once** (founder: "update should check instantly and
  reflect in the app"): Tex Suite looks on opening, and again when Settings >
  Updates or the bell is opened (if the last look is over a minute old); it
  always asks for the fresh update file (GitHub kept copies for minutes).
- **Settings > Updates is the one place for updates** (founder): "Update to
  vX" downloads and installs right there, with what is new and the steps in the
  same card; the bell's update notice leads there.
- **No more "timeout: global"**: a download had two minutes in all, too short
  for 21 MB on a slow line. Now connecting must succeed within 20 s and a slow
  download has half an hour; problems are said in plain words.
- **The bell** is an icon alone at the right of the Tex Suite box, level with
  the name (founder: "its more visible"); in the top bar only on narrow windows.
- Knowledge base: "Reading books" rewritten for the new reader.
- Engine: tex-engine 0.30.1.

## 0.47.0 (2026-10-29) - Contacts import, numbers with their country, duplicates; a simpler update button

- **Import contacts** (founder: his Google Contacts file would not import):
  Google Contacts (CSV), Outlook (CSV) or a phone's vCard (.vcf). Numbers
  written without a country get Tanzania's.
- **Possible duplicates** after an import: the same number (even written
  differently), the same email, or names alike; **Merge** keeps every number
  and email once, **Keep both** leaves them apart.
- **Several numbers and emails per person**, each number with its **country**
  (Tanzania, the United States, then A to Z), kept in full: "+255 712 345 678".
- **Settings > Updates: one button** that says what it will do: Check for
  updates, Checking…, Update to vX. The answer shows at once (founder: Check
  now had to be pressed twice).
- **The top bar fits small windows** (founder: Import and search overlapped).
- Engine: tex-engine 0.30.0.

## 0.46.0 (2026-10-29) - The book reader

- **Books open inside Tex Suite** (founder's top priority: "we need one thing
  to be right"), with **one click** on the cover, as the best reading apps do.
  EPUB, PDF, Word (.docx), OpenDocument (.odt), text and Markdown; your own
  writing reads like a book (headings become chapters). Books are read from
  memory: nothing decrypted is written to disk.
- **Set like printed books**: EB Garamond, justified, first-line indents,
  chapters on new pages, the chapter at the top and the page number at the
  foot. PDF pages drawn by hayro (pure Rust).
- **Pages turn like paper**: hold any point of a page's edge and drag; the
  page curls from there and follows, showing its back; let go past the middle
  and it turns, otherwise it falls back. Click or the arrow keys turn it too.
- **Auto** (two pages in landscape, one in portrait), **1 page** or **2 pages**,
  kept for every book; **Paper**, **Sepia**, **Night**; text size; turning as
  paper or instant (readers asked to be able to switch animation off).
- **Every book reopens where you stopped.**
- The reader is its own module, **tex-reader** (crates/tex-reader), tested:
  typesetting, the curl's geometry (the held point follows the pointer, paper
  keeps its length, the page cannot tear), hostile files.
- Knowledge base: new article "Reading books".
- Dependencies: hayro 0.8 (Apache-2.0 OR MIT, forbids unsafe code), ab_glyph.

## 0.45.0 (2026-10-29) - Integrity check, Trust report, Anivo study, book covers

- **Tex Suite checks itself at every start** (founder: "not a single
  modification"): each release program is signed with Churtex's release key;
  a program changed by one byte, or unsigned, opens in protected mode: only
  Export Suite and a genuine update. Proven on a real build (one byte changed:
  protected mode). Rollback and updates carry the signatures.
- **About > Trust report**: tex-testkit's report of this version and of its
  engine, shown as a short paper: verdict, key figures, abstract, results,
  standards (NIST SSDF, OWASP ASVS), limitations, how to reproduce. Every
  number comes from a real run; what could not run is shown as a gap.
- **Anivo**: tap a verse for five highlight colours, a bookmark, a note or a
  copy; **My study** lists Bookmarks, Highlights and Notes. Every reading has
  a **title** (all 366 days). **Section headings inside Genesis**, written in
  Anivo's own words from reading the text verse by verse (more books follow).
  Verses in **EB Garamond**, the reading face.
- **Books** stand as books: 2:3 covers, the book's own cover when it has one
  in a book's shape (EPUB, comics, FB2), otherwise a designed cloth cover.
- **The Vault's PIN screen scrolls** (founder: with Forgot PIN open the words
  did not all show).
- Security: zstd vulnerabilities fixed in the engine (0.28); the book cover
  reader and the integrity check are tested with hostile input.
- Engine: tex-engine 0.29.0.
- Coming next: the book reader inside Tex Suite (tex-reader, in progress).

## 0.44.0 (2026-10-29) - Off-grid control, rollback, Anivo's daily flow, Vault upload

- **Go fully off-grid** (founder): Settings, **Scheduled tasks** lists
  everything Tex Suite does by itself (update checks, announcements, Space
  Saver, auto-lock, calendar and Anivo reminders), each tagged Online or
  On this device, each with its own switch. **Off-grid mode** stops every
  internet contact; everything else keeps working.
- **Off-grid report** in the Dashboard's menu: no account, no trackers,
  encryption, the Vault's PIN, auto-lock, the clipboard, where your data
  lives, and **every time Tex Suite went online** (when, where, why).
- **Go back to an earlier version** (founder): before each update the
  version you had is kept (the last two); Settings, Updates offers to go
  back, and the version you leave is not offered again until a newer one.
- **Settings in sections**: Appearance, Language, Updates (now with
  **Download and install**, founder: the update showed but could not be
  installed from there), Notifications, Scheduled tasks.
- **Anivo's daily flow** (founder): **Prayer**, then the **main
  reading**, then the **further reading**, shown as steps. Further
  reading is one continuous passage ("Genesis 1:1 – 3:7"). Leaving it for
  later counts as half a day (½ in the streak, a gold tick in the
  calendar). Verses in a lighter font, easier to read. About Anivo
  rewritten for readers.
- **The Dashboard** (founder): Anivo as the big tile on the left, the
  six other apps in a 3 × 2 grid on the right.
- **Projects is a tool of its own** (founder): Projects and Tasks; Code
  keeps the Editor and Repositories. New Projects icon.
- **Edu**: the menu shows **All courses** and each category. The course
  "How to use Tex Suite" has a 12th lesson, Off-grid.
- **What's new, guided** (founder): after an update a small green dot
  marks each app with something new, and the new item in its menu;
  opening it clears the dot. A fresh install shows none.
- **Vault: adding files made easy** (founder: "currently so hard for
  someone to use and upload"): My Photos, My Videos, Voice notes and
  Documents open with a big drop zone ("Drop files into My Photos here")
  that lights up while files are dragged over the window, with a **Choose
  files** button. Files added there land on that shelf, but only files of
  that sort (a film dropped in My Photos stays a film; a test proves it).
- French: labels that ran past the menu's edge shortened.
- Knowledge base: new article **Off-grid**; Settings, Updates (rollback,
  green dots), Anivo, Find your way, Edu and Vault files updated; every
  screenshot taken again.
- Engine: tex-engine 0.27.1 (the texts above, the Projects icon).
- Security review of this release: the off-grid switch is checked before
  every internet contact (updates, announcements) and each contact is
  logged; rollback only restores copies this device made of its own earlier
  version, from its own folder, never anything downloaded; the drop zone adds files through
  the same review and encryption as every import. The test that fails on
  any unknown internet address still passes.
- Package: still .tar.gz, so 0.42 can install it; .tar.xz from 0.45.

## 0.43.0 (2026-10-29) - Anivo, Edu, Tools, notifications, the Vault's PIN reset

- **Anivo is here** (founder): Bible reading, a world of its own like the
  Vault. **Today's reading** from the founder's Anivo Bible Reading Plan:
  the New Testament main reading and the Old Testament further reading, in
  the King James Version, "Day N of 365" (366 in leap years), the streak
  of days read in a row, **Mark as read**. **Reading calendar**: read days
  ticked, missed days (since you started) marked, today ringed; click a day
  to read it. **Bible (KJV)**: all 66 books. **About Anivo** in its
  author's words, with the open-use policy for churches. While today's
  reading waits, the Dashboard reminds you.
- **Edu: the course "How to use Tex Suite"**: 11 lessons made from the
  knowledge base, each with a 3-question quiz marked at once; best marks
  and progress kept.
- **Tools as menu categories** (founder): Calendar, Maps, Code (Projects,
  Editor), Lang (Translate, Learn), Comm (Messages, Radio); pages still to
  come say so in place.
- **Notifications** (founder): a bell in the top bar, with a red dot and
  a small shake when something is new; its own menu (All, Updates,
  Announcements); select and delete, Delete all; Settings can switch them
  off. An update is always first, and installing shows each step as a
  timeline (downloading, checking the signature, installing, restarting).
  The version line under the name stays as it was.
- **The Vault's PIN**: 3 wrong tries lock it for an hour, then longer
  each time, at most a day. **Forgot PIN?**: with Tex Suite's password, a
  reset empties the Vault's own things 72 hours later, then a new PIN is
  set; the right PIN in between cancels it. **The Vault hides its
  contents** whenever Tex Suite is not the window in front.
- **Passwords**: after an import, Tex Suite offers to delete the export
  file for good (overwritten, then removed).
- **Every clickable control shows the hand** (founder: Import and Export
  did not): a test now reads the code and fails if any does not.
- Knowledge base: new articles Anivo, Edu, Notifications; Vault,
  Passwords and Find your way updated; every screenshot taken again.
- **Smaller downloads from 0.44**: the updater now also reads .tar.xz
  packages, measured 10.7 MB instead of 15.4 MB (gzip) for this release.
  0.43 itself still ships as gzip so 0.42 can install it. A test also
  proves a hostile package cannot write outside its folder.
- Dependencies: tex-engine 0.27.0; new xz2 0.1 (static liblzma, public
  domain/MIT) for .tar.xz; `cargo update`.

## 0.42.1 (2026-10-29) - when Tex Suite last looked for updates

- Settings > Updates shows when Tex Suite last looked for a newer version
  ("Last checked at 06:12").
- The first version delivered by the updater itself: if you are reading
  this in the update notice, updates work.
- Dependencies: tex-engine 0.26.4.

## 0.42.0 (2026-10-29) - updates from the Tex releases page

- **Updates** (founder): while the device is online, Tex Suite looks at the
  Tex releases page every 15 minutes (and once soon after opening). A newer
  version shows **Update to v… available** under the name; click it to
  read what's new, then **Download and install**: it downloads, checks
  Churtex's signature, installs and restarts. Nothing is downloaded before
  you agree; a changed or fake update is refused and your version keeps
  working.
- Settings has an **Updates** card: look automatically (on), Check now.
- **The Vault**: an **Exit** button at the top beside "Vault" (founder:
  the one at the bottom was easy to miss); the menu says My Finances, My
  Vehicles, My Supplies, My Contacts, My Photos, My Videos, My Journal.
- The small uppercase headings in every menu have more space between
  their letters (founder: "too thin").
- **About** is its own menu (founder): Founder, Churtex, Features, FAQs.
  Features: "No account, no internet" first, "Videos 50 to 70% smaller",
  and the Free and Pro boxes the same height.
- **What's new** shows the ten latest versions, without dates, and a button
  to the full changelog on the Tex releases page (published with every
  release); the update notice has no date either.
- **Menu labels never pass the menu's edge** ("Sync with my devices" did):
  shorter "Sync devices", and any label too long ends with "…" with the
  whole text on hover. Screenshot runs now list every label that does not
  fit, checked at each release (it caught three French ones, shortened).
- Knowledge base: a new article, Updates; the Vault article follows the
  new names; every screenshot taken again.
- Dependencies: tex-engine 0.26.3; new ureq 3.5 (HTTPS, rustls),
  ed25519-dalek 3 (signatures), sha2, hex, flate2 and tar (the package),
  getrandom (the release key), all MIT/Apache; `cargo update`.

## 0.41.0 (2026-10-29) - knowledge base, What's new, crisp icons, Support menu

- **Knowledge base** (Support > Knowledge base; founder): 19 articles in 8
  categories, from creating your library to Passwords, backups and Free
  and Pro, each with screenshots of the real screens (from the sample
  library), searchable, with related articles. Written in kb/en; updated
  with every change to Tex Suite, like the Edu course will be.
- **What's new** (Support > For developers > Changelog): every version's
  changes since the very first, newest first, yours marked; **Releases**
  points to the Tex releases page.
- **Support menu** in sections (founder): Support (Get help: a person at
  Churtex, a paid service of its own, not part of Pro, coming), Feedback,
  Knowledge base, For developers (Changelog, Releases, Bug report). The
  headset opens the knowledge base.
- **Crisp icons** (founder: "they look blurred, the colour is not popping"):
  every app icon and the Tex Suite logo are now drawn from their drawings
  at the exact size on screen, on whole pixels, instead of shrunk from big
  pictures.
- **Coming-soon apps** (Anivo, Edu, ...): a soft screen with the app's
  icon and "Coming soon", never the page opened before.
- **The Vault**: a **Household** section first (Smart Home, Finances,
  Vehicles, Supplies; coming, entered by hand). **TexCoin removed** for
  good.
- **Sync** has a laptop and a phone for its icon.
- **The unlock screen** keeps inside the window's rounded corners (its
  square corners stuck out).
- About: a short note that Tex Suite is built with AI-assisted
  development, every release reviewed and tested.
- Heavy jobs (builds, tests, screenshots) now run inside a memory limit
  (tools/capped.sh): tests had pushed the 8 GB computer out of memory.
- Dependencies: tex-engine 0.25.0; `cargo update`.

## 0.40.0 (2026-10-29) - Passwords

- **Passwords** (Vault, Security; founder: "allow import and export ...
  compatible with others"):
  - your logins, searchable, the selected one on the right: user name,
    password (dots until Show), strength, the site's 2FA code when the
    login carries it, folder, notes; copy any of them;
  - a **copied password leaves the clipboard after 30 seconds** (unless
    something else was copied since);
  - **New password** makes a strong one at once; length 8 to 64, A-Z,
    0-9 and symbols to choose; changing them makes a new one;
  - **Import** from Chrome, Edge, Brave, Firefox, Safari, Bitwarden
    (CSV or JSON), 1Password, LastPass, Proton Pass or KeePass: shows what
    it found, adds it with one click, skips what is already here, and
    reminds you to delete the export file;
  - **Export** for browsers or for Bitwarden-compatible managers, after a
    warning that the file is not encrypted;
  - a website opens only when clicked, and only a plain http(s) address:
    one from an imported file can never run a command (tested).
- **Checked in English, French and Swahili** on a hidden screen; fixed what
  French showed: labels running into values, "Supprimer" over "Modifier"
  (2FA codes and Passwords: Delete on its own line), the Support toggle
  (segments now fit the longest label), the version line ("gagnés").
- Dependencies: tex-engine 0.24.0 (adds csv 1.4); `cargo update`: nothing
  newer.

## 0.39.0 (2026-10-29) - centred text, Support, 2FA by QR code

- **Text centred** (founder: "the text is slightly below"): the search
  bar placed its text by hand, 2.5 px low; it is now centred by the
  layout. Poppins also sat 1 px high in every field and button: one nudge
  for all text. Measured with the new `tools/align-check.py` on the
  search bars, password, Unlock, Import, Add account, Rename and the menu,
  light and dark: icons at 0 px, text within half a pixel.
- **Window buttons**: the x, - and + now sit on a pixel's centre, exactly
  in the middle of their circles (measured 0.0 px).
- **2FA by QR code** (founder): paste a screenshot of the website's QR
  code, choose a picture of it, or drop one on the window: the account is
  added at once. Each account can show its own QR code to move it to a
  phone (with a warning). Checked end to end: the code drawn on screen was
  read back from a full screenshot as the exact link.
- **Support** (headset icon where the star was): one form with a toggle
  like the theme's: Feedback, Bug report, Support (Support comes with
  Pro). A report adds only versions and system; copy it or save it as a
  file. Sending it straight to Churtex waits for the founder's choice.
- **Menu**: the Dashboard back at the top (Chat stays below it); the
  "Offline", "Churtex Foundation" and storage boxes are gone: under the
  name now "v0.39.0 · 456 GB (58%) saved". Settings, About, Support,
  Chat and Tex show only their own item, never the Dashboard's.
- **About** shows the Free and Pro features below the founder's word (the
  Features page and its star are gone).
- **Export Suite / Import Suite** (were Export/Import Vault: they move all
  of Tex Suite). Including the Vault's private things asks for its PIN.
- **"Unlock TexSuite"**, with Suite in your colour.
- **Checkboxes** in the app's look (filled with your colour when ticked);
  **Save** buttons show a plain tick (it vanished white on white).
- Screenshots now run on a hidden screen (`tools/headless-shots.sh`), so
  they never appear on, or stall behind, the founder's own windows.
- Dependencies: tex-engine 0.23.0; new rqrr 0.11 (reads QR codes), qrcode
  0.14 (draws them), arboard 3.7 (pictures on the clipboard), all
  MIT/Apache; `cargo update`: nothing newer.

## 0.38.0 (2026-10-29) - 2FA codes, auto-lock, full backups, Free and Pro

- **2FA codes, our own Authenticator** (founder; Vault, Security): add a
  website's setup key or its otpauth:// link, then see its six-digit code
  with a ring counting down the seconds; click a code to copy it. Rename or
  delete (asked first: without the codes you may be locked out of the
  site). Works with no internet; secrets are never shown again once saved.
- **Auto-lock**: after 5 minutes without a touch, Tex Suite locks itself
  (it waits for an import or export to finish; Space Saver keeps making
  files smaller while it is locked).
- **Full backups**: Export Vault with "Private" ticked now also carries
  contacts, calendar, 2FA codes, profile, picture and PIN, and every
  item's thumbnail and licence. Before, a backup restored on a new device
  came back without them. Import (merge) adds the contacts, events and
  accounts you don't have yet.
- **Menu rail** (founder): Anivo first, then a line; Home and Coin moved
  into the Vault (Personal: Home; a new Wallet section: Coin, coming); the
  Dashboard icon sits in the middle of the apps, three above and three
  below; "Cal" is now "Calendar".
- **Features** in two halves: Free (everything for one person) and Pro
  ($16 once, coming): the Tex Store (buy online, download, yours to keep),
  sync, share, several users, shared storage, cloud backup.
- The Vault's menu scrolls on a short window.
- Dependencies: tex-engine 0.22.0 (adds hmac, sha1, sha2 for the codes);
  `cargo update`: nothing newer.

## 0.37.0 (2026-10-29) - private by default, a calmer menu, snapping, your colour

- **Private by default** (founder): every Vault file and contact is
  private unless made public. "Select" on the Vault's shelves and in
  Contacts picks several to make public or private at once; each item
  shows its visibility. Only public contacts can go on calendar events;
  making attached contacts private warns first, then takes them off those
  events (tex-engine 0.21.0).
- **The menu rail**: Dashboard, **Chat** and **Tex** at the top; the apps
  centred in the middle (the Vault last, after a line); Features, Settings
  and About at the bottom. Chat has its page (coming).
- **Snaps to half the screen**: the window can now be as small as 760 x
  560 (it was 980 x 640, wider than half a 1920-px screen); below 1000 px
  the menu keeps only its icon rail.
- **The Tex Suite icon follows your colour** (founder): the logo in the app
  and the icon in the applications menu are drawn in the colour chosen in
  Settings (only Tex Suite's; the apps keep their own colours).
- Dependencies: resvg 0.45 added (draws the icon's SVG in any colour);
  `cargo update`.

## 0.36.0 (2026-10-29) - the Vault, a place of its own

- Opening the Vault blurs the whole app behind the PIN card, with "Back"
  to leave (founder: entering a different place). Inside, only the Vault's
  own menu: People (Contacts), Files (Photos, Videos, Voice notes,
  Documents), Personal (Journal, Family tree: coming), Security (2FA
  codes, Passwords: coming), Vault settings (change the PIN) and Exit
  Vault, which locks it again. The top bar shows only the window buttons
  and the language.
- In the main menu the Vault is the last app, set apart by a thin line.
- The door animation plays across the whole window.

## 0.35.0 (2026-10-28) - the Vault's PIN and its door, Tex

- **Vault PIN** (founder): the private room (Photos, Videos, Voice notes,
  Documents, Contacts) asks for a 4-digit PIN; the first time it is set up
  (typed twice). A number pad and the keyboard; a wrong PIN shakes the
  dots; five wrong tries make it wait (tex-engine 0.19.0). Locking Tex
  Suite closes the room again.
- **The vault door opens**, drawn live from lines: the wheel turns, the
  bolts slide back, light runs round the rim, the door swings open on its
  hinges with rays behind it (founder: "a cool complex animation, lines,
  not a video").
- **Tex**, the assistant (Tex AI): a robot head in the menu above the star;
  its page says what it will do (chat, answers from Pedia and your data,
  offline). Coming.
- Settings: "Custom colour", a round swatch like the others; its picker
  opens in our padded popup.

## 0.34.0 (2026-10-28) - contacts, people, rights at import, Sync, Features

- **Contacts** in the Vault: a searchable list, each person's card (phone,
  email, address to copy; notes) and the same form style as every form.
- **People on events** in Cal: add contacts to an event; opening it shows
  each person with every way to reach them, even with no network. Event
  reminders also show as desktop notifications.
- **Rights at import** (founder): "These are my files, or I have the
  rights to store and use them", or attach a licence, which is kept
  encrypted with each item; Add stays off until one is done. The item's
  details show "Yours" or "With a licence".
- **Sync** button between Import and Share, and its page: what will sync
  first (2FA, account, settings, analytics, then the library); coming.
- **What Tex Suite can do** (star icon above Settings): measured
  strengths, and what is coming (cloud backup per GB, a film store).
- About: its cards have the banner's 28 px padding on both sides
  (founder: less padding on the left than the right).

## 0.33.0 (2026-10-28) - Cal, the calendar

- **Cal** in Tools (founder: "innovate the complex looking calendar"):
  "Up next" across the top (the next three events with a countdown), the
  month as day cards with coloured event pills ("+2 more"), today in the
  accent, and the chosen day on the right with its events and "Add event".
  Double-click a day to add. The form: title, date, all day or start/end,
  reminder (none, 10 min, 30 min, 1 h, 1 day), colour, notes. Events are
  encrypted in the Vault (tex-engine 0.17.0); reminders show while Tex
  Suite is open.
- "Search" in the menu opens the Dashboard with the cursor in its search
  box (founder: one page, not two).
- The menu's name and version are centred on the logo.
- Dependencies: chrono 0.4 added (the device's local date, time and time
  zone, for "today" and reminders); `cargo update`.

## 0.32.0 (2026-10-28) - sharp icons, version shown, Edu

- App icons are shrunk smoothly (mipmaps) to every size: no more rough,
  pixelated edges in the menu (founder: "the icons look pixelated").
- The version shows under "Tex Suite" in the menu (founder: people should
  know which version they have). An "Update available" badge comes with
  the update system.
- Edu is one of the nine apps (out of Pedia); AI leaves the app list: it
  will be built into every app instead.
- Getting started on the Dashboard is collapsed; its arrow opens the steps.

## 0.31.0 (2026-10-28) - Tex Suite

- **Tex Suite** is the app's name (founder): window, applications menu,
  icon (a seven-point hub with a T, drawn from scratch like the Tex Vault
  icon), programs `tex-suite` and `texsuite`; the installer removes the
  old Tex Vault entry. GitHub: churtex/tex-suite. Your library stays where
  it is (the internal data folder keeps its name on purpose).
- Nine apps, named without "Tex" inside the suite: Home, Media, Books,
  Vault, Pedia (Aid, Farm, Stead, Edu), Tools (Maps, Code, Lang, Cal,
  Comm), Coin, Manna, AI. Icons redrawn as real objects in one bold colour
  each; apps to come keep their colour and say "Soon".
- **Dashboard** (was Home): large icons, five to a row, the search box
  exactly as wide as the icons; Getting started under it. Its menu:
  **Search**, **Analytics** (activity calendar and storage), Import Vault,
  Export Vault.
- Menu: "Tex" + "Suite" (accent) with the logo across the top; the line
  under it meets the top bar's line.
- **Thumbnails load at once**: each is made once and kept encrypted in the
  Vault (tex-engine 0.16.0); before, every film's picture was made again
  each time the app opened (founder: "take too long to load").
- Activity calendar: month names never overlap.
- Dependencies: `cargo update`.

## 0.30.0 (2026-10-28) - two-column menu, profile form, TexComm, TexCode

- **Two-column menu** (founder): a rail of app icons (names on hover, Home
  at the top, Settings and About at the bottom, apps to come faded) and
  the open app's items beside it: TexSuite (Home, Import, Export), Tex
  Media (Home, Movies, Series, Music, Podcasts), TexBooks (Ebooks), Tex
  Vault (Photos, Videos, Voice notes, Documents). Apps to come say so.
- **Profile form** rebuilt like Settings (founder: "in sync with how I
  want things"): one label column, full-width fields of the same style
  and height, picture with its buttons beside it, Save on the right that
  lights up only when something changed. `theme::form_row` / `big_area`
  for every form to come.
- Apps: TexComm (messages; radio with hardware) replaces TexChat; TexCode
  (code editor that builds and runs) added: 20 apps.
- Any new page shows its own app in the menu.

## 0.29.0 (2026-10-28) - TexSuite app home

- After unlock: **one big search box** and **every Tex app as a tile**
  (founder): TexHome, Tex Media, TexBooks, Tex Vault, TexPedia, TexMaps,
  Tex Calendar, Tex Keys, TexContacts, TexMoney, TexComm, Tex Share,
  TexEdu, TexAid, TexFarm, TexStead, TexLang, Tex Manna, TexAI. Working
  apps open; the others are faded with "Soon". Icons from tex-engine.
- The library's own home (featured, explore) is now "Tex Media".
- A slim typing line in the password and search fields (the founder found
  egui's full-height line "too long").
- Sidebar rows 28 px so everything still fits; the founder's Kiswahili
  (tex-engine 0.15.0). GitHub repository renamed to churtex/tex-suite.
- Dependencies: `cargo update`.

## 0.28.0 (2026-10-28) - locked screen, Getting started, light menu

- **Locked screen** (founder's "Dona" inspiration): while the Vault is
  locked nothing of the library shows. Soft colour clouds drift behind a
  card with the logo in a white tile, a gentle gradient and the password;
  only the window buttons and the language flag stay at the top. Import
  Vault still opens from there, with a way back.
- **Getting started** on Home: add your first files, set up your profile,
  let Space Saver make a film smaller, keep a backup with Export Vault;
  each crossed out when done, "Open ›" for the next, "Hide" to remove it.
- **Menu in Poppins Light** (the open page in Regular): lighter, calmer.
  Poppins Light added (SIL OFL, THIRD_PARTY.md).
- Dependencies: `cargo update`.

## 0.27.0 (2026-10-28) - your profile, activity calendar, Share button

- One person per Tex Vault (founder): the avatar opens **your profile**:
  picture (made square and small, encrypted), name and a few words. The
  avatar shows the picture, else the initials. Home says "Welcome back,
  {name}".
- **Activity calendar** on Home, GitHub-style: one square per day for as
  many weeks as fit, deeper colour on days the library was used more
  (opened, watched or read, added); hover a day for its numbers. Counted
  on this device only, encrypted (tex-engine 0.13.0).
- **Share** button beside Import (icon only, light like the padlock):
  shows what Tex Share will do (nearby devices over Wi-Fi, like Xender /
  AirDrop). Not working yet; marked "Coming soon".
- "device" instead of "computer" in every text (mobile is coming).
- Screenshot tool: also the profile and Share pages.
- Dependencies: `cargo update`.

## 0.26.0 (2026-10-28) - Podcasts, Voice notes, choose the shelf on import

- New shelves (tex-engine 0.12.0): **Podcasts** under Library (sermons,
  talks, podcasts, audiobooks) and **Voice notes** under Private. Both are
  speech: Space Saver makes them Opus 64k (half of music).
- Import shows the picked or dropped files first, each on the shelf it
  seems to belong to (already selected); change any of them, remove some,
  then "Add" (founder: "automatically selected to the one the system
  thinks it is, but the user can change").
- Details panel: "Shelf: Movies" opens the same menu to move an item later.
- Sidebar rows 30 px (macOS size) so the nine shelves and the boxes fit an
  860-px window; a drawn × (Poppins has no "✕"); new mic and wave icons.
- The screenshot tool also captures the import review with a menu open.
- Dependencies: `cargo update` (rustix 1.1.6). Newer major versions to
  plan: eframe 0.37, rfd 0.17.

## 0.25.0 (2026-10-28) - every video at 576p

- tex-engine 0.11.0, recipe 6: every video is made at most 576 px tall,
  same shape (founder, after watching 720p and 576p side by side: "this
  is the one we have been searching for"). Fast X (1080p) -70%, See -61%,
  The Last Ship (x265) -26%. The 720p/480p trial of 0.24 is gone.
- The quality badge knows 576p ("1080p → 576p" in the details).

## 0.24.0 (2026-10-28) - 480p for files that barely shrink, real quality badges

- Space Saver uses tex-engine 0.10.0 recipe 5: a 720p trial piece first;
  if it saves less than 25% (files like The Last Ship, x265: 7% at 720p,
  36% at 480p) the film is made at 480p (founder's decision).
- Converted videos show their real stored quality ("720p" or "480p", and
  AV1) instead of what the file name says, and the details panel says
  "Picture: 1080p → 720p" (founder: people should see why one film looks
  softer than another). Items converted before this version show AV1 only.

## 0.23.0 (2026-10-28) - menus inside the window, library in the app folder

- Every menu (language, Sort) is one padded popup that opens towards the
  window and keeps 12 px from every edge; the language list touched the
  screen edge (founder). The screenshot tool now also captures both menus
  open, so their edges are checked at every release.
- The library now lives in the system's place for app data:
  ~/.local/share/tex-vault/Library (Linux), %LOCALAPPDATA%\tex-vault\Library
  (Windows), ~/Library/Application Support/tex-vault/Library (macOS). A
  library left by earlier versions in the home folder (~/MediaVault or
  ~/TexVault) is moved there once, in one rename, only when no other Tex
  Vault is open; a place the person chose (a flash disk) is never moved.
  Test `an_old_library_in_home_moves_once_and_whole`.
- Unlock screen: "Open location" opens the library folder (the path shows
  on hover); its texts are translated ("Fungua Maktaba Yako").
- Kiswahili for Space Saver (tex-engine 0.9.1): Maktaba inakandamizwa,
  Imewekwa, Simamisha, Imesimamishwa, Endelea.
- The flag and the chosen language follow the language on screen.
- Welcome and unlock cards are centred on their measured height and never
  run off the bottom of the window; toasts wrap within the window.
- Settings: the outdated "English for now" line replaced; About: "Founder,
  Churtex Foundation".

## 0.22.0 (2026-10-28) - 720p, simpler Space Saver, tidy sidebar

- tex-engine 0.9.0: recipe v4, the founder's choice: up to 720p, preset
  10, CRF 42, H400 grain, Opus 128k. One recipe for every film (stronger
  settings for HEVC files were rejected by the founder). Time estimate:
  about 40% of the film's length (a 2-hour film in ~48 min).
- Space Saver panel shows only "Compressing your library", the item with
  one bar that never starts over (the check stage now moves it too), the
  time left, and "Saved X". The time left uses the speed measured in this
  session, so a resumed item is no longer shown as nearly done.
- Sidebar: no tagline; the three boxes always fit inside the menu (long
  text is cut with "…"); "Offline · Encrypted"; storage on separate lines
  (size, items, % saved, a bar with a track); the active menu item has
  only its soft red background, no red bar (founder).

## 0.21.2 (2026-10-28)

- Compressing runs at low priority (tex-engine 0.8.3), so the app and the
  desktop stay quick while it works (the Import file chooser took ~3 s to
  open during compression).

## 0.21.1 (2026-10-28)

- Kiswahili menu complete (tex-engine 0.8.2): "Sio mubashara ·
  imesimbwa", Nyingine, Akaunti.
- The padlock sits in the centre of its button (icon-only buttons are
  square now), and the person in the avatar is centred in its circle
  (founder: "not centred from all sides").

## 0.21.0 (2026-10-28) - languages begin; padlock and avatar

- The menu (sidebar, top bar, shelf names) now follows the chosen
  language through tex-engine's new `lang` module (0.8.1): Kiswahili from
  the founder (22 texts so far), French complete for the menu. Texts not
  translated yet show in English. Choosing a language says how much is
  translated. Other screens follow screen by screen.
- Top bar: Lock is a padlock only (its name on hover); a round account
  avatar sits between the padlock and the flag (a person icon until
  accounts have pictures). The tagline under the logo is smaller so longer
  languages fit on two lines.
- `TEX_LANG=sw|fr|en` shows another language without saving it (for
  screenshots and checks).

## 0.20.0 (2026-10-28) - Space Saver 3.5x faster (recipe v3)

- tex-engine 0.7.0: 480p, AV1 preset 10, CRF 42, film grain from a ready
  photon-noise table (ISO 400, the founder's pick: "H400 seems closest ...
  the red colour on the car was clearest"). A 2-hour film converts in
  about 33 minutes on the dev laptop (was ~1 h 52 min) and comes out
  ~54% smaller. Needs the svt-av1 package (SvtAv1EncApp) besides ffmpeg.
- Time estimates in the panel follow the new speed (~0.35x the length,
  including the check).
- An item that was half-way with an older recipe starts over with this
  one; items already converted stay as they are.

## 0.19.0 (2026-10-28) - the 480p recipe, retries

- Space Saver uses the founder's new recipe (tex-engine 0.6.2): at most
  480 px tall (wide films 1146x480, 16:9 854x480), AV1 preset 8, CRF 45,
  film grain; sound Opus 128k. Measured on a 2-minute Spy clip: 28 MB ->
  11.0 MB (-62%), converted in 0.95x its length (a 2-hour film in under
  2 hours). Items converted earlier with the 720p recipe stay as they are
  (converting again would only lose quality); an item that was half-way
  starts over with the new recipe.
- A failed conversion is tried again later (up to 3 times) instead of
  being set aside at once; then the panel says so with a "Try again" link.
  Items set aside by 0.18.0 are retried on opening. (One of the founder's
  episodes failed because a test script stopped every encoder.)
- Error messages no longer show the encoder's "Svt[info]" lines.
- Test `a_failed_item_is_tried_again_then_set_aside`.

## 0.18.0 (2026-10-27) - Space Saver: videos and music about half the size

- **Space Saver** (tex-engine 0.5.0, record in tex-engine
  docs/16_MEDIA_COMPRESSION.md): every movie, series episode, video and
  song is converted in the background with the founder's approved recipe
  (AV1 preset 6, CRF 45, 10-bit, film grain, at most 720p; Opus 128k).
  Measured on 2-minute clips: 58-71% smaller on the founder's H.264 films,
  27% on an HEVC series; about 1.5x the running time to convert.
- One item at a time; the waiting list is saved next to the Vault
  (space-saver.json), so it continues after closing the app or turning
  the computer off, from the last finished 2-minute piece. Existing items
  are queued too.
- A result is used only if it plays cleanly, has the same length and
  frames, passes picture spot checks and is smaller; otherwise the item
  stays as it was. The stored copy is replaced crash-safely.
- Panel on Home and the shelves: current item, stage, %, time left for it
  and for everything, items waiting, space saved so far, Pause/Continue,
  and the advice to keep the laptop plugged in.
- Closing the window stops the encoder (no stray ffmpeg); it continues
  next time. Converted items open as .mkv; thumbnails are remade.
- Needs ffmpeg with libsvtav1, libopus and libvmaf (RPM Fusion ffmpeg);
  without it the panel says so and nothing is converted.
- Tests: `queue_takes_media_once_and_is_saved`,
  `a_video_in_the_vault_is_made_smaller` (real conversion inside a Vault).

## 0.17.0 (2026-10-27) - privacy of screenshots, search, sort, filter, rename

- **Screenshots never show a real library.** `tools/make-sample-library.sh`
  builds a sample library from generated clips, tones, pictures and books
  with invented titles; every screenshot in docs/ now comes from it. The
  earlier ones (taken from the founder's files) were removed; the history
  is being rebuilt from old versions with the sample library.
- **Search works with several words**: dots, underscores and dashes in
  file names count as spaces, and the words may come in any order. Before,
  any title of two words found nothing ("operation fortune" vs
  "Operation.Fortune..."). Test `search_ignores_dots_and_word_order`.
- **Sort** on every shelf: newest, name A-Z, name Z-A, largest, year. Names
  are the ones people see, not raw file names. Test
  `sorting_uses_the_names_people_see`.
- **Filter chips** on every shelf from what is there: 4K, 1080p, 720p, HDR,
  HEVC, H.264, MKV, MP4, PDF, EPUB, MP3...
- **Rename**: "Rename..." in the details panel gives an item a name of its
  own; the file name stays (shown small underneath). Clean titles are shown
  everywhere ("Spy" for "Spy.2015.720p.BluRay.x264.mp4"). Engine 0.4.0.
- Fix: text on coloured chips (Season 1, filters) was black instead of
  white; the same mistake in the language list and the import stages.
- Fix: the logo inside the app had jagged edges (drawn from shapes); it is
  now the icon PNG at the right size, smoothly scaled.
- "1 seasons" -> "1 season".

## 0.16.1 (2026-10-27) - vault icon, languages, fixes

- **New icon**, drawn from scratch: a vault door (ring, hinges, bolts and
  handle wheel) on the blue-violet squircle of the first Tex icon. Used for
  the menu, the window and the logo inside the app.
- Fix: the menu and desktop showed a generic icon. The installer now
  refreshes the desktop's icon cache.
- **Languages**: a flag in the top bar and a Language card in Settings:
  English (United Kingdom flag), Kiswahili (Tanzania flag), Français
  (France flag), saved in settings.json. Texts are not translated yet;
  choosing Kiswahili or Français says so. Plan in src/gui/i18n.rs. Test
  `language_codes_round_trip`.
- Fix: the sidebar shared its scroll state with the page, so scrolling the
  page (e.g. About) scrolled the menu, and the menu's hover areas drifted
  half an item off ("I have to point between two items"). Each now has its
  own scroll id.
- Sidebar: a **Churtex Foundation** box under "Offline · encrypted" (opens
  churtex.org when clicked); storage box on two lines so all fits.

## 0.16.0 (2026-10-27) - the sidebar redesign

From the founder's dark mockup; the right panel stays as it was.

- **Left sidebar**: TexVault logo and "Your library · offline · forever",
  Home; LIBRARY (Movies, Series, Music, Ebooks); PRIVATE (Photos, Videos,
  Documents); VAULT (Import Vault, Export Vault, Settings, About); library
  storage and "Offline · encrypted" at the bottom. Replaces the top
  navigation and the Tools menu.
- **Top bar**: one wide search field for the whole library (Escape clears),
  Import, Lock and the window buttons.
- **Home**: a Featured banner (newest movies and shows, a frame from the
  video fading into navy, clean title and year, quality tags, Play and
  Details, carousel arrows), Explore with filter chips and poster cards,
  then Latest in Movies, Latest Series, Your Music and Your Books. The old
  category cards are gone. Searching on Home shows results as posters.
- **Poster cards** everywhere (Home, shelves, Series shows): picture,
  title, year or episode, size, quality tags; a play mark on hover.
- Titles and tags are read from file names ("Spy.2015.720p.BluRay.x264" ->
  "Spy", 2015, 720p, H.264). Tests: `titles_from_real_file_names`,
  `badges_from_file_names`.
- New icons: Play, Gear (Settings), Upload (Export).
- Screenshots of every version's Home are kept in
  docs/screenshots/history/ (recovered back to 0.5.0).

## 0.15.3 (2026-10-27) - Poppins only

- The app uses one font, Poppins: Regular for text and Medium for titles
  (SemiBold looked too heavy next to regular text). Inter, Montserrat,
  Rajdhani, Lato, the font chooser and "Add your own font" are removed.
- Fix: "→" showed as a box (Poppins has no arrow); "›" is used instead.

## 0.15.2 (2026-10-27) - password field width

- Fix: the password fields still stretched across the whole card (the
  frame around the text filled the centred layout; 0.15.1 only narrowed the
  text inside). They now sit in an exact box as wide as the Unlock button.

## 0.15.1 (2026-10-27) - founder's UI fixes

- Home category cards: Movies and Series on top, then Videos · Music ·
  Photos, then Ebooks · Documents. Series shows "N shows" and "N episodes"
  on separate lines (never split mid-text).
- Home never previews personal items: no photos, personal videos or
  documents in the banner, the category pictures, Recently Added or Recent
  Additions (counts only). The banner shows a frame of the newest movie.
- Export Vault: Photos, Videos and Documents are one **Private** choice,
  unticked by default.
- Series episodes: each row has a frame from that episode with its number
  on it. Fix: the row's Open button did nothing (the row's click area sat on
  top of it).
- Import panel: stages of the current file (Compress, Check, Encrypt), what
  is happening in plain words, files, elapsed, speed, space saved, time
  left, a bar for all files and one for this file, and the last files done.
- Thumbnails: photos have their own worker, so they no longer wait behind
  video frames (several seconds each).
- Unlock/create password fields are as wide as the button below them.
- Title in the top bar reads "TexVault" (Vault in the accent colour).
- Terminal tool: no stale version number in its help.

## 0.15.0 (2026-10-27) - Import Vault, Export Vault, About

- **Tools menu** is now: Import Vault, Export Vault, Settings, About. The
  single-file Compress, Restore, Encrypt, Decrypt and History screens are
  gone (Tex Vault is a library; the `texvault` terminal tool keeps them).
- **Export Vault**: the whole library, or chosen shelves, in one
  `.texvault` file. Stays encrypted; opens with the same password.
- **Import Vault**: choose a `.texvault`, type its password, then **Merge**
  (its items join your library, duplicates skipped) or **Replace** (it
  becomes your Vault; the old Vault folder is kept aside, never deleted).
  Works on a new computer with no Vault yet, from the welcome screen, and
  by dropping or double-clicking a `.texvault` file.
- **About**: a welcome from the founder, Aniwene Madolomani ("Welcome
  off-grid."), what Churtex is, and a **Visit churtex.org** button.
- No more "Export…" of single items (founder's rule: no recovery of
  originals; items are enjoyed inside Tex Vault).
- Default library folder for new users: `~/TexVault`.
- The `.texvault` file type replaces `.utx` in the menu entry.
- Engine: tex-engine 0.3.0 (bundles and merge). Tests:
  `replace_keeps_the_old_vault_aside`, `import_on_a_new_computer_and_merge`,
  `export_name_gets_its_extension`.

## 0.14.1 (2026-10-27) - settings carried over

- Fix: settings and the library location stayed behind in an older data
  folder when the new `tex-vault` folder already existed. Missing files are
  now copied over from older folders (never overwriting newer ones).
  Regression test `old_settings_reach_an_existing_new_folder`.

## 0.14.0 (2026-10-27) - Tex Vault, shared engine, documents, real thumbnails

- Renamed **Tex Vault** (app `tex-vault`, terminal `texvault`, repository
  churtex/tex-vault). Settings, history and the library location move over
  from earlier names; the installer removes earlier menu entries.
- The engine moved to its own repository, **churtex/tex-engine** (v0.2.0),
  shared by all Tex apps; this app depends on it by tag. Engine docs moved
  there too.
- **Documents** are accepted (Word, Excel, PowerPoint, OpenDocument, RTF,
  text, Markdown, CSV) with their own section; programs and archives are
  refused. Wording: "library" instead of "Vault" inside the app.
- **Welcome screen** on first start with the five key points (encrypted,
  much smaller, enjoyed inside the app, media/books/documents, offline),
  then the create form with **big password fields** (44 pt, rounded).
- **Real thumbnails for movies, series and videos**: a frame about 75 s in,
  dark frames skipped; only the start of the file is decrypted, into a
  private temporary file removed at once. Needs an ffmpeg that can decode
  H.264/H.265 (RPM Fusion; `ffmpeg-free` cannot). Series cards show a
  frame from the first episode.
- Home: 7 category cards (4 + 3); big counts shortened (1.2K, 444K, 1.2M)
  so they always fit.
- Removed: the "move originals to the Trash" prompt (users keep their
  originals outside Tex Vault).

## 0.13.0 (2026-10-27) - Tex MediaVault, Settings

- Renamed **Tex MediaVault** (Tex = product brand, Churtex = company):
  app `tex-mediavault`, menu entry, new icon (Navy squircle, white T,
  Cerise bar), repository `mrweneonline/tex-mediavault`. Settings, history
  and Vault location move over from the 0.12 data folder automatically;
  the installer removes the 0.12 menu entry.
- **Settings** (Tools menu): accent colour (8 swatches or any colour),
  font (Inter, Montserrat, Poppins, Rajdhani, Lato, all embedded with their
  SIL OFL licences, or your own .ttf/.otf), Light/Dark/System. Applied at
  once and remembered.
- Home: category cards in 3 columns x 2 rows (name and count on the left,
  newest picture on the right), so text always fits; long names in cards
  are cut to the card width with "…".
- After an import: offer to move the originals (verified in the Vault) to
  the Trash, showing the space it frees. Trash, not delete, so it can be
  undone.
- Fix: the welcome banner's gradient had square corners poking out of
  its rounded border.
- HANDOFF.md: how to continue on another computer (setup, state,
  decisions, ordered next work including user accounts and kids accounts).

## 0.12.1 (2026-10-27) - Series by show and season; Import fixed

- Series: one card per show; inside, Season tabs and episodes in order
  (E01, E02...), with titles read from the names. Recognised: S01E02,
  S01 E02, sees01e02 (name glued on, two-digit numbers), Season 1 Episode 2,
  season01 ep02, 1x02; case and a trailing year are ignored, so "See",
  "see." and "See (2019)" are one show. Look-alikes such as "Glass1E2" or
  "Mission 2x4 Movie" are not episodes. 2 new tests.
- Fix: the file chooser could slip behind the window, and Import then
  seemed dead. Choosers are now attached to the window (kept on top); a
  second click says the chooser is open; a failed chooser no longer blocks
  Import; Import works during an import (files join the queue).

## 0.12.0 (2026-10-27) - Churtex MediaVault

The app is now **Churtex MediaVault**: an offline vault for media.

- Renamed everywhere: app `churtex-mediavault`, terminal `mediavault`, menu
  entry, icons, installer (which removes the old Urtex Compressor entry).
  `.utx` files and the Urtex engine keep their names.
- New screens, from the founder's light mockup (2.png) in the Mac look:
  top navigation (Home, Movies, Series, Videos, Music, Photos, Ebooks),
  welcome banner, six category cards with the newest photo, Recently
  Added, and Storage / Offline / Recent Additions on the right. Light,
  dark and system.
- Create / unlock screen (password strength required on create); Import
  button and drag and drop; library shelves with a Mac inspector (sizes,
  saved, method, fingerprint, Open, Export, Remove); search; Lock.
- Media only: series detected from names like S01E02, personal videos
  from camera names (VID_, PXL_...) and .mov; non-media files are politely
  refused (documents will get their own Churtex app). Compress, Restore,
  Encrypt and Decrypt remain in the Tools menu for any file.
- Photo thumbnails decrypted and decoded on a background thread; imports
  run in the background with progress and Stop; Open decrypts a private
  copy (owner-only folder in ~/.cache) that is wiped on Lock and on exit.
- Engine: the Vault can be shared by the screens and background imports
  (`Arc<Vault>`, index behind a lock); `Vault::bytes`; media kinds.
- Test: media kinds from names. 38 tests.

## 0.11.0 (2026-10-27) - big files 2.5x faster to compress, 4x to restore

- New method 8: files of 8 MiB or more run the Urtex engine on 4 independent
  blocks in parallel (fixed by size, so archives stay identical on every
  machine; not in Max mode, which would need about 5 GB). Measured on an
  11.8 MB file: compress 218.4 s -> 86.8 s, restore 110.6 s -> 26.7 s, for
  2.7% more size; still 23% smaller than xz -9e. Restored bit-identical.
- Progress: the four blocks' progress is added up for the one progress
  bar, and Cancel reaches all of them.
- App: results the list did not expect (the 4-core engine, the document
  safety net) appear in the method list as they finish.
- Fix (found by the new test): an empty input made zero blocks, which the
  decoder refuses; it is now one empty block.
- 2 new tests (round trip, determinism, bad headers, frozen format). 37 tests.

## 0.10.0 (2026-10-27) - documents and PDFs unpacked, then compressed

- New method 7: the deflate streams inside Word/Excel/PowerPoint/
  OpenDocument files, zip, EPUB, PDF and PNG are undone with preflate-rs
  0.7.6 (Microsoft, Apache-2.0), which records the corrections needed to
  rebuild each stream bit for bit; the content is then compressed by our
  methods. Measured on 39 real documents (9.4 MB): **19.2% saved, up from
  5.8%**; text-heavy ones 35-67%; 39/39 restored identical.
- Safety net: zstd on the file as it is is always a candidate too, so
  unpacking never makes a file bigger.
- Zip bombs: the unpacked size is capped (32x, at most 1 GiB) before any
  memory is used; beyond it the file is compressed normally.
- Hostile files: preflate panics become errors, all recipe lengths are
  checked, output never exceeds the stored size. 4 new tests (1,500
  corrupted recipes, 1,500 damaged files, oversized recipe, frozen
  fixture). 35 tests in total.
- Known limits: PNGs split over several IDAT chunks or written by fdeflate
  are not unpacked yet. The full engine on unpacked content is slow (about
  11 KB/s for compress + restore on this laptop); speed work is next.

## 0.9.0 (2026-10-27) - JPEG photos one third smaller, losslessly

- New method 6: lossless JPEG recompression (lepton_jpeg 0.5.8, Apache-2.0),
  tried automatically on files that start like a JPEG, in every mode and in
  the Vault. The exact original photo comes back, bit for bit.
  Measured on 18 real JPEGs (4.9 MB): 33.1% saved vs 16.0% for zstd -19;
  18/18 identical after compress/restore; in a Vault 33.02% saved.
- JPEGs a library cannot handle (rare variants) fall back to the other
  methods instead of failing.
- Hostile input: decoding capped at the stored size; library panics become
  errors. 4 new tests incl. 1,500 corrupted payloads and a frozen fixture
  (tests/data/). Old files are unaffected (new method id).
- App: JPEGs are described as "recompressed losslessly, usually 10 to 25%
  smaller" instead of "will barely shrink"; the progress list shows the
  JPEG method.
- THIRD_PARTY.md now lists every component, including those added in 0.7
  and 0.8 (RustCrypto, zeroize, zxcvbn, rpassword, serde) and egui/eframe.

## 0.8.0 (2026-10-27) - Vault core

First step towards Churtex MediaVault (plan agreed 2026-10-26).

- **Vault** (`src/vault.rs`, docs/15_VAULT.md): a folder where every file
  is compressed when that helps and always encrypted, unlocked by one
  password. Random Vault key sealed by the password; a random key per
  item, sealed by the Vault key; password change re-seals only the key file.
  Duplicates (same BLAKE3 fingerprint) are stored once. File names and
  contents are unreadable on disk. Every item is verified before it is
  listed; exports are checked against the fingerprint and never overwrite.
- **Chunked encryption** (`src/stream.rs`, `UTXC`): STREAM construction over
  XChaCha20-Poly1305 in 1 MiB chunks. Any size with little memory, random
  access for playback (`Read` + `Seek`), detects changed, dropped, swapped
  and cut-off chunks.
- Terminal: `urtex-compress vault init|add|ls|get|rm|passwd`.
  Measured: 3 files, 1,201,721 bytes stored in 60,288 bytes (94.98% saved).
- 6 new tests, including a frozen format and a scan of the Vault folder for
  leaked names or content. Total: 27 tests.

## 0.7.0 (2026-10-26) - encryption

- Password protection: **Encrypt** and **Decrypt** in a new "Security"
  section of the sidebar, and a "Protect with a password" switch on
  Compress. Files are compressed, then encrypted with XChaCha20-Poly1305;
  the key comes from the password through Argon2id (256 MiB, 3 passes,
  0.92 s per try on the dev laptop). Proven ciphers only, see
  docs/14_ENCRYPTION.md for why and for the measurements.
- New `UTXE` envelope around a whole `.utx` (docs/05_FILE_FORMAT.md):
  method, size and fingerprint are hidden; the header is authenticated;
  hostile Argon2 settings are refused. Old `UTX1` files are unchanged.
- Encrypted files are decrypted again and compared before they are written.
- Password strength meter (zxcvbn); "Strong" is required. Warning that a
  forgotten password cannot be recovered.
- Terminal: `urtex-compress c file --encrypt` (asks twice, hidden);
  `d`/`t`/`i` ask for the password on encrypted files; `URTEX_PASSWORD`
  for scripts.
- 6 new tests, including every single-bit flip and every truncation of an
  encrypted file, and a frozen-format test.
- `examples/crypto_bench.rs` compares XChaCha20-Poly1305, ChaCha20-Poly1305
  and AES-256-GCM and times Argon2id settings.
- Fix: the folder name was blank for a file opened by a relative path.

## 0.6.0 (2026-10-26) - one-button app, already-compressed files

- Redesigned Compress and Restore screens: the content is centred and grows
  with the window (a maximised window is no longer half empty), the chosen
  file is shown large, and one big Compress / Restore button replaces the
  small one.
- No mode options in the app: it always uses the best compression.
- Already-compressed files (video, photos, audio, PDF, Office, archives) are
  recognised by their first bytes (extension as fallback) and packed quickly
  with Zstandard, with a note saying why: a 33.9 MB mp4 used to take 3 minutes
  for 0.2%. The terminal tool prints a note suggesting `--fast`.
- Fix: the quick path showed no percentage or remaining time. Zstandard now
  reports progress in 1 MiB steps (output proven byte-identical,
  `zstd_chunked_output_is_identical`); verification and restore of standard
  methods also show progress and can be cancelled. Regression test
  `fast_path_reports_progress` fails on the old code.
- Screenshot mode no longer writes to the real History, and can capture a
  maximised window (`URTEX_SHOT_MAXIMIZED=1`).

## 0.5.0 (2026-10-26) - macOS-style design

- Desktop app redesigned to look like a macOS (Sequoia) app: own title bar
  with red/yellow/green window buttons at the top right, rounded borderless
  window (drag by the title bar, resize from the edges, double-click to
  maximise), floating sidebar with sections and SF Symbols-style line
  icons, segmented controls, grouped boxes, Mac push buttons.
- Inter font embedded (SIL OFL), so the app looks the same offline.
- Colours: Mac neutrals plus the Churtex palette: Cerise Red for actions and
  selection, Deep Emerald for verified/saved, Executive Gold for the best
  result, Navy Depth for the app icon. Light/dark follow the system.
- File location shown as the folder name (full path on hover).
- Developer screenshot mode (`URTEX_SCREENSHOTS`): saves every screen in
  light and dark, for reviewing the design.

## 0.4.1 (2026-10-26) - file dialog fix

- Fix: choosing a file a second time (after "Compress another file", on
  Restore, or "Change...") did nothing. The dialog library keeps one
  desktop-portal connection for the whole process, but each dialog ran on a
  new async runtime that was thrown away afterwards, killing that
  connection. The app now keeps one runtime for all dialogs. Regression test
  `background_task_survives_into_next_dialog` fails on the old code.

## 0.4.0 (2026-10-26) - desktop app

- Desktop app `urtex-compressor`: drag and drop or file dialog; live
  progress per method; result screen with saved location, Open folder,
  chart of all methods; Restore screen with archive details; persistent
  History; light/dark/system appearance.
- App menu entry, icon, `.utx` file association (double-click to restore).
- Never overwrites: picks `name (2).ext`.
- Engine reports progress and supports cancel (output unchanged).
- Fixes found in app testing: fake result after cancel; file dialog crash.
- Code split into a library plus two programs.
- Full Silesia benchmark: smaller than zstd/xz/brotli/bzip2 on all 12 files.

## 0.3.0 (2026-10-26) - first Urtex Compressor release

- New context-mixing engine (Urtex CM): 19 contexts + match model, bit
  histories, 2-layer mixer, 3 SSE stages, x86 filter, record and column models.
- Best-of selection with zstd-22, LZMA-9e, brotli-11, bzip2-9.
- `.utx` format v1 (magic `UTX1`) with BLAKE3-256 integrity.
- Verify-before-write, atomic writes, decompression-bomb limits.
- Deterministic math for cross-machine decoding.
- Test suite: round-trips, single-bit-flip detection, fuzzing.
- Linux .rpm / .deb / .tar.gz; GitHub Actions for Windows, macOS, ARM, Android.

## 0.2 (prototype, "Churtex Compress")

- Six simple methods (RLE, LZ77, delta, pattern+exceptions). See `audit/`.
