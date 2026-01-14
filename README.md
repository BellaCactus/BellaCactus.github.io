<div align="center">

# 🖤 bella cactus (github pages)

terminal-core personal website.  
**static-only** (github pages), **no backend**, just **html / css / js**.

**black / white / pink** by default  
+ optional **red “evil” palette** when you want it spicy 🔥

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-live-ff78c8?style=for-the-badge)
![Static](https://img.shields.io/badge/Static--Only-no%20backend-0b0b0b?style=for-the-badge)
![Vibes](https://img.shields.io/badge/vibe-terminal--core-ff4db8?style=for-the-badge)

</div>

---

## 🌙 what is this?

**bella cactus** is my personal **terminal-themed website playground**.  
it’s made to feel like a fake OS / interactive terminal hub rather than a normal portfolio.

it’s a place for:
- mini tools
- experiments
- weird little pages
- secret stuff
- and “why did i add this” moments

---

## 🖤 vibe

- fake-os / terminal playground aesthetic  
- black / white / pink default palette  
- optional **red “evil” mode**  
- cozy-chaotic and meant to be **explored**, not skimmed  
- subtle motion > loud motion  

---

## ✨ highlights

- **intro gate**: auto-playing video (if browser allows)  
- **music bar + waveform**: random track picker + lil waveform line  
- **terminal script**: types out commands + responses  
- **sticker wall**: random stickers sprinkled behind the UI  
- **command palette**: quick actions + navigation  
- **easter eggs**: oneko, secrets, and assorted nonsense  

---

## 🗺️ pages

### main pages
core pages that match the “site world” vibe:

- `index.html` : main hub (terminal + music + stickers + palette)
- `limiter.html` : bella limiter page
- `os.html` : fake cli / fake os page
- `ascii.html` : ascii zoo
- `idle.html` : screensaver-style page (leave it open)
- `glitch.html` : glitch / corruption playground
- `dreams.html` : surreal dream log

### extra mini-tools / experiments
little side quests:

- `encrypter.html`
- `ascii-art-maker-type-shit.html`
- `keyb.html`
- `snkaegame.html`
- `dungeoncrawler.html`
- `shitty-ass-gamez-3d.html`
- `controllar-test.html`
- `boucnignlolgo.html`
- `sigmaness-basiclaly-epic.html`
- `legacy-home.html`
- `shrines.html`
- `vault.html`

---

## 🎮 controls (good to know)

### index.html
- **ctrl + k** (or **/**) opens the command palette  
- **esc** closes palette / overlays  

the palette understands stuff like:
- `open dreams`
- `open idle`
- `open glitch`
- `theme pink` / `theme white` / `theme red`

### idle.html screensaver
- **space**: pause/resume  
- **r**: reroll sprites/text  
- **t**: cycle theme  
- **esc**: back to `index.html`  

---

## 🧪 customization

this site is built to be reskinned + remixed without needing any backend stuff.

### change the soundtrack
the music list lives in `index.html`  
(search for `const tracks = [`)

- drop `.mp3` files in the repo root (same folder as `index.html`)
- add them to the tracks list
- keep filenames exact (spaces + punctuation matter)

### change stickers
sticker filenames are also listed in `index.html`  
(search `stickerFiles`)

- add images (`.png / .jpg / .gif`) to the repo root
- update the list

### theme persistence
theme saves in `localStorage` under:

- `bella_theme`  
  values: `pink`, `white`, `red`

so if you flip into red mode once… it sticks until you change it 😈

---

## 🖥️ run locally

quick + dirty:
- double click `index.html` and it will *mostly* work

recommended (less browser weirdness with audio/video):

```bash
# from the repo folder
python -m http.server 8000
