
# bella cactus (github pages) 

a static, terminal-ish, fake-os-ish personal website with a black/white/pink palette, little interactive toys, and “this tab is alive” type shiii 

**stack:** pure html + css + client-side js  
**hosting:** github pages (no backend)

---

## what’s inside

### main hub
- **`index.html`**: the home “terminal hub”
  - intro gate video (`hello-everypony-mlp-dexter.mp4`)
  - soundtrack player + waveform viz (browser may block autoplay)
  - terminal typing script + rotating ascii critters
  - sticker wall background (clickable images)
  - “intel” panel (explicit buttons for permissions, no silent tracking)

### featured pages
- **`limiter.html`**: bella limiter project page (feature deep-dive / terminal vibes)
- **`os.html`**: fake os / cli playground (includes local storage + some indexeddb stuff)
- **`ascii.html`**: ascii zoo + **local stash** (IndexedDB for images/audio on *this browser only*)
- **`idle.html`**: screensaver-style page (canvas vibes, optional audio toggle)
- **`glitch.html`**: glitch gallery (drag/drop or load an image, all local-only)
- **`dreams.html`**: surreal dream log (uses localStorage)

### extra toybox pages (mini apps)
- `encrypter.html` (encrypt/decrypt tool)
- `ascii-art-maker-type-shit.html` (ascii converter)
- `keyb.html` (keyboard tester)
- `snkaegame.html` (snake)
- `dungeoncrawler.html` (dungeon crawler)
- `shitty-ass-gamez-3d.html` (3d-ish page)
- `controllar-test.html` (controller tester)
- `boucnignlolgo.html` (bouncing logo)
- `shrines.html` (directory of fixations)
- `vault.html` (vault page)
- `legacy-home.html`, `sigmaness-basiclaly-epic.html` (legacy / extra)

---

## assets + vibe ingredients

**music files currently included:**
- `530 0.mp3`
- `bipolar.mp3`
- `Tay-K - I Love My Choppa [Official Audio] 4.mp3`
- `Who I Smoke (Official Music Video).mp3`
- `lil-jon-yeah.mp3` (oneko click easter egg)

**images / stickers:**
- `twi looking.png`
- `twi and trixy.jpg`
- `ponies in bed.jpg`
- `yuri meme.png`

**oneko:**
- `oneko.gif` + a few extra oneko images

---

## running it locally (so it doesn’t get weird with files)

you *can* double click `index.html`, but some browsers get fussy about audio/canvas/files when opened as `file://`.

recommended tiny server:

### windows / mac / linux
```bash
# in the repo folder
python -m http.server 8000
````

then open:

* `http://localhost:8000/index.html`

---

## deploying (github pages)

this repo includes a github actions workflow:

* `.github/workflows/static.yml`

typical setup:

1. push to `main`
2. in github: **Settings → Pages**
3. set **Build and deployment** to **GitHub Actions**
4. your site publishes from the workflow automatically

---

## customization notes (quick hacks)

### change the sticker pool

search for `stickerFiles = [` in `index.html` / `ascii.html` and edit the filenames.

### add / change soundtrack tracks on the home page

in `index.html`, find the `tracks = [` array and:

* add `{ file: "yourfile.mp3", label: "your label" }`
* make sure the mp3 exists in the repo root (same folder as `index.html`)

### “uploads” on pages aren’t real uploads

some pages let you add files (glitch gallery, ascii stash), but:

* **glitch.html** uses local drag/drop (not uploaded anywhere)
* **ascii.html** saves to **IndexedDB** (local to *that browser/device* only)
* **dreams/shrines/vault/idle/index** use **localStorage** for certain bits

if you want files to be visible to everyone: commit them to the repo.

---

## browser reality checks (aka debuffs)

* **autoplay is usually blocked** until the user interacts (click/tap). this is normal.
* anything stored in localStorage/IndexedDB is **per-device/per-browser**, not global.

---

## license

no license file is included right now. if you want others to reuse/modify it, add a LICENSE (mit/apache-2.0/etc). if you *don’t*, that’s also valid for a personal art-tech project.

---

## credits / shoutouts

made by bella cactus 🖤
built as a living weird website, not a portfolio.

```

```
