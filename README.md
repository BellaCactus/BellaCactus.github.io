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
