<div align="center">

# ♡ bella cactus (github pages)

terminal-core personal website.  
**static-only** (github pages), **no backend**, just **html / css / js**.

**black / white / pink** by default, with optional “evil” vibes depending on page 😈

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-ff78c8?style=for-the-badge)
![Static](https://img.shields.io/badge/Static--Only-no%20backend-0b0b0b?style=for-the-badge)
![Vibes](https://img.shields.io/badge/vibe-terminal--core-ff4db8?style=for-the-badge)

</div>

---

## what is this?

**bella cactus** is my personal **terminal-themed website playground**.  
it’s meant to feel like a fake OS / interactive terminal hub, not a normal portfolio.

it’s a place for:
- mini tools
- experiments
- weird little pages
- secret stuff
- “why did i add this” moments

live url (because this is a `*.github.io` repo):  
**https://bellacactus.github.io/**

---

## vibe

- fake-os / terminal playground aesthetic  
- black / white / pink default palette  
- cozy-chaotic, meant to be **explored**, not skimmed  
- subtle motion > loud motion  
- “alive” UI: shimmer text, floating sprites, scanlines, ambient nonsense

---

## repo layout

```txt
/
├─ index.html              # main hub
├─ links.html              # extra link hub / legacy-ish
├─ pages/                  # all subpages live here
├─ media/                  # images/gifs/video/favicon
└─ assets/
   └─ songs/               # mp3 soundtrack files
```

---

## highlights (main hub stuff)

- **intro gate**: autoplay video gate (click if browser blocks it)
- **music bar + waveform**: random track picker + waveform line
- **terminal script**: types commands + responses (doesn’t grow forever)
- **sticker wall**: background stickers sprinkled behind UI
- **command palette**: quick actions + navigation
- **easter eggs**: oneko + “yeah” button energy :3

---

## pages

### core “site world” pages
these match the main vibe / feel like part of the same universe:

- `index.html` : main hub (terminal + music + stickers + palette)
- `pages/limiter.html` : bella limiter deep-dive page
- `pages/os.html` : fake cli / fake os page
- `pages/ascii.html` : ascii zoo + local stash
- `pages/idle.html` : screensaver-style page (leave it open)
- `pages/glitch.html` : glitch / corruption playground
- `pages/dreams.html` : surreal dream log
- `pages/vault.html` : vault page (archive-y / stash vibes)
- `pages/shrines.html` : shrine page (lore / vibes)
- `pages/tamers.html` : tamers archive page

### tools / utilities
little practical side quests:

- `pages/encrypter.html`
- `pages/tab-crypt.html`
- `pages/epic-calc.html`
- `pages/audio-editor.html`
- `pages/ascii-art-maker-type-shit.html`
- `pages/keyb.html`
- `pages/pokecap.html`
- `pages/controllar-test.html`

### games / experiments
because of course:

- `pages/snkaegame.html`
- `pages/dungeoncrawler.html`
- `pages/shitty-ass-gamez-3d.html`
- `pages/lilgame.html`
- `pages/boucnignlolgo.html`
- `pages/sigmaness-basiclaly-epic.html`

### misc / legacy
- `pages/legacy-home.html`
- `links.html`

---

## controls (good to know)

### index.html (main hub)
- **ctrl + k** (or **/**): open command palette  
- **esc**: close palette / overlays

palette understands stuff like:
- `open dreams`
- `open idle`
- `open glitch`
- `theme pink` / `theme white` / `theme red` *(if the page supports it)*

### pages/idle.html (screensaver)
- **space**: pause/resume  
- **r**: reroll sprites/text  
- **t**: cycle theme  
- **esc**: back to `index.html`

### pages/glitch.html (glitch gallery)
- **drag & drop** an image onto the stage (local-only, not uploaded)
- **r**: reroll corruption
- **space**: freeze/unfreeze
- **esc**: back to home

### pages/ascii.html (ascii zoo)
- reroll creature button (and it cycles on its own)
- includes a **local stash** using **IndexedDB** (saved only in *your* browser)

---

## customization

### change the soundtrack
songs live in: `assets/songs/`

1) drop `.mp3` files into `assets/songs/`  
2) update the `tracks` list in `index.html` (search for `const tracks = [`)

**important:** filenames must match exactly (spaces/punctuation included)

### change stickers / media
images/gifs/video live in: `media/`

- stickers are referenced by filename in `index.html` (search `stickerFiles`)
- other pages may also have their own sticker lists

### theme persistence
some pages store theme in `localStorage` under:

- `bella_theme`  
  values: `pink`, `white`, `red`

so if you flip modes… it can stick until you change it again >:3

### “uploads” note (static site reality check)
github pages can’t accept uploads to the repo from the website itself.

- **glitch gallery** file input = local-only (in-memory)
- **ascii zoo stash** = local-only (IndexedDB), won’t sync across devices  
- if you want “real uploads”, you’d need a backend (not happening here by design)

---

## run locally

quick + dirty:
- double click `index.html` and it will *mostly* work

recommended (less browser weirdness with audio/video):

```bash
# from the repo folder
python -m http.server 8000
```

then open: `http://localhost:8000/`

---

## notes / gotchas

- autoplay is a liar: browsers often block audio/video until a click happens  
- if music “doesn’t play”, hit play once and you’re good
- if you move files between folders, update links in:
  - `index.html` (tracks + sticker list + page links)
  - and any page that references media directly

---

## status

this repo is a living art-tech project.  
it will keep mutating. that is the point. (:3)
