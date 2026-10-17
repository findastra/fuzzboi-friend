# Fuzzboi Friend

## 👉 Make your Fuzzboi: **[findastra.github.io/fuzzboi-friend](https://findastra.github.io/fuzzboi-friend/)**

*A pet app by Astra.*

Fuzzboi Friend makes your very own Fuzzboi. Type your six-digit hex code (like `C0FFEE`), and it draws that exact Fuzzboi from Astra's hand-drawn layers, at full size (2048×2048), on your code's color. Save it as a PNG or copy a link that opens it.

The Fuzzbois themselves, their rules and the art live in [findastra/fuzzboi-factory](https://github.com/findastra/fuzzboi-factory). The pet lives in the Cage: [astras-pet-apps](https://github.com/findastra/astras-pet-apps).

## How to run it

- **Easiest:** open <https://findastra.github.io/fuzzboi-friend/>. A code in the address opens that Fuzzboi, e.g. `https://findastra.github.io/fuzzboi-friend/#C0FFEE`.
- **On your PC:** double-click [fuzzboi-friend-20261009.html](fuzzboi-friend-20261009.html). It needs the internet, because it loads the rules and drawings from the Fuzzboi Factory website.
- **Testing a change to the rules:** put this folder next to a `fuzzboi-factory` checkout and serve the parent folder (`python -m http.server`, then open `http://localhost:8000/fuzzboi-friend/`). On `localhost` the app reads `../fuzzbois/site/` instead of the website.

## What works

- **Any hex code:** type or paste six characters, with or without the `#`. The color chip shows your color as you type.
- **Your Fuzzboi:** the real art, stacked from the 32 layers the Fuzzboi Forge uses. Body style, color, accessories, rarity and background are listed under the code.
- **Save my Fuzzboi:** downloads `fuzzboi-<code>.png`. On a phone you can also long-press the picture.
- **Copy link:** a link that opens your Fuzzboi. **Surprise me** rolls a random code.
- **Bubbles:** the pet says what it is doing. Moods follow the Cage's meanings: `sleep` (no code yet), `curious` (drawings loading), `happy` (done), `worried` (the code breaks a Fuzzboi rule, such as two hats), `sick` (it can't reach the Fuzzboi Factory website), `sad` (drawings missing on our side).

## Limits

What is not done, plainly:

- **Letters A–F aren't on Astra's design notes yet.** The notes ([Fuzzbois-33.png](https://github.com/findastra/fuzzboi-factory/blob/main/art/procreate-export/Fuzzbois-33.png)) set every other rule. Until letters get traits, they count as 0–5 (A=0 … F=5), a stopgap chosen by Claude, not Astra. Your color is always exact; the traits may change later. The rules live in `fuzzboi-factory/site/fuzzboi.js`, so both pages change together.
- **The pet's art is a draft** until Astra approves it: nine moods generated on 2026-10-09 from a reference made from her own layers ([art/](art/), listed in `sprite-20261009.json`).
- **Not in the Cage yet.** The registration (with the generated sheet, so it needn't be paid for again) is a patch in [cage/](cage/README.md), kept out of `astras-pet-apps` for now at Astra's request.
- No desktop pet and no quick chat.
- It needs the internet: the rules and the drawings come from the Fuzzboi Factory website.
- Nothing is saved. Your code is only in the address bar.

## Words

Each part of a pet app has one name: the **pet** (Fuzzboi Friend), its **app** (this page), **bubbles**, the **app icon** and the **pet well**. The full list is the Cage's [PET-WORDS.md](https://github.com/findastra/astras-pet-apps/blob/main/PET-WORDS.md).

## Credits

Fuzzbois are drawn by Astra. Hatched with Claude Opus 5.5 (`claude-opus-5-5`) on 2026-10-09. MIT licensed.

Desktop appearance draft updated 2026-10-11: see [desktop details](desktop-pet-20261011.json). This changes the desktop pet, not application features.
