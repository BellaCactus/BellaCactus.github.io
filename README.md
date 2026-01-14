# bella cactus (github pages)

terminal-core personal website. black/white/pink by default, optional red “evil” palette. **static-only** (github pages), **no backend**, just html/css/js.

## vibe

- fake-os / terminal playground aesthetic
- black / white / pink (and a red mode when you want it spicy)
- cozy-chaotic, meant to be **explored**, not skimmed
- subtle motion > loud motion

## highlights

- **intro gate**: auto-playing video if the browser allows it (otherwise click once).
- **music bar + waveform**: random track picker + lil waveform line.
- **terminal script**: types out little commands and responses.
- **sticker wall**: random image stickers sprinkled behind the UI.
- **command palette**: quick actions + navigation.
- **easter eggs**: oneko, secrets, and a few “why did i add this” moments.

## pages

main pages that match the “site world” vibe:

- `index.html` : main hub (terminal + music + stickers + palette)
- `limiter.html` : bella limiter page
- `os.html` : fake cli / fake os page
- `ascii.html` : ascii zoo
- `idle.html` : screensaver-style page (leave it open)
- `glitch.html` : glitch / corruption playground
- `dreams.html` : surreal dream log

extra mini-tools / experiments:

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

## controls (good to know)

### index

- **ctrl+k** (or **/**) opens the command palette.
- **esc** closes palette / overlays.

the palette understands stuff like:

- `open dreams`, `open idle`, `open glitch`, etc.
- `theme pink` / `theme white` / `theme red`

### idle screensaver

- **space**: pause/resume
- **r**: reroll sprites/text
- **t**: cycle theme
- **esc**: back to `index.html`

## customization

you can reskin the whole thing without touching any backend stuff.

### change the soundtrack

the music list lives in `index.html` (search for `const tracks = [`).

- drop `.mp3` files in the repo root (same folder as `index.html`)
- add them to the tracks list
- keep filenames exact (spaces + punctuation matter)

### change stickers

the sticker filenames are also listed in `index.html` (search `stickerFiles`).

- add images (`.png/.jpg/.gif`) to the repo root
- update the list

### theme persistence

theme is saved in `localStorage` under:

- `bella_theme`  (values: `pink`, `white`, `red`)

so if you flip to red mode once, it sticks until you change it.

## run locally

quick and dirty:

- just double-click `index.html` and it will mostly work.

recommended (avoids some browser weirdness with media):

```bash
# from the repo folder
python -m http.server 8000
