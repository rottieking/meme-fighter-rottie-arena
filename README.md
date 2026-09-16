# Meme Fighter — $ROTTIE Arena

A meme-fighting arcade game built around the $ROTTIE coin — pick your fighter, battle through the story, grind Arcade Mode for endless rounds, and collect cards along the way.

**Play it now:** https://t.me/Meme_fighterbot/rottie
**Website:** https://rottieking.github.io/meme-fighter-rottie-arena/

---

## Features

- **Story Mode** — 10 arenas, Wolf/Croc/Bear enforcers guarding the path, Bearzilla waiting at the top
- **Arcade Mode** — no fixed levels, just endless rounds that get harder the longer you survive. Health drops appear more often as the difficulty climbs. Best streak is saved; a loss resets you to Round 1
- **Difficulty picker** — Easy (default), Medium, and Hard, each with a bigger coin/XP payout
- **6 playable heroes** — King, Sir, Bull, Frog, Doge, and Cat, each with their own stats and special move
- **Gesture controls** — swipe to move and jump, tap to punch, hold to kick/block, charge up your special
- **Coin economy** — earn coins from every win in either mode
- **42-card collection** — unlock cards by playing as each hero, defeating specific villains, or beating the game — or buy your way in early with coins
- **360° hero previews** — tap the 🔄 icon on Character Select or in your card collection for a spinning look at a hero
- **Installable** — add it to your home screen and play offline like a normal app

---

## What's in this repo

| File | What it does |
|---|---|
| `index.html` | The entire game — code and art in one file. This is the only file that needs to load for the game to run. |
| `manifest.json` | Makes the game installable as an app on your phone/desktop |
| `service-worker.js` | Lets the game load and play without an internet connection once installed |
| `*.mp4` | 360° rotation clips for the card/character previews. **These must stay in the same folder as `index.html`** — the game looks for them right next to it, not in a subfolder |

---

## Updating this repo — read this before you paste a new index.html

`index.html` is large (20+ MB, since every image in the game is embedded directly inside it). GitHub's own in-browser text editor is not reliable at that size — pasting a file this big into it can silently fail, hang, or save a truncated copy, which looks exactly like "the game broke as soon as I updated it."

**Use file upload instead of the text editor:**
1. On the repo's main page, click **Add file → Upload files**
2. Drag `index.html` (and any `.mp4` files you're updating) into the upload box
3. When prompted that the file already exists, confirm you want to replace it
4. Commit

This uploads the file as-is rather than routing it through the editable text box, and avoids the size problem entirely.

**After updating:** test through the actual Telegram bot link, not by opening the file directly on your phone — opening a local file in a preview pane (Files app, Edge's file preview, etc.) does not run the game's code and will look broken even when it isn't. If Telegram still shows the old version after a confirmed successful upload, fully close and reopen the Telegram app — it caches Mini Apps aggressively.

---

## Credits

$ROTTIE Meme Fighter Arena — built for the $ROTTIE community.
