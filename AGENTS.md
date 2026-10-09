# Rules for assistants working on Fuzzboi Friend (fuzzboi-friend)

*A pet app by Astra.* Public credit is always **Astra**, never a legal name. Keep work
information (including any employer's name) out of this repo.

Hatched with Claude Opus 5.5 (`claude-opus-5-5`), 2026-10-09. Record your model name and
version here when you change something substantial.

## What this is
A pet app for sharing Fuzzbois: a friend types their six-digit hex code and gets that exact
Fuzzboi as a PNG. v0 is one web app file (`fuzzboi-friend-20261009.html`), live on GitHub Pages
at <https://findastra.github.io/fuzzboi-friend/> (`index.html` forwards there). Its host is the
Friendly Farmer in `findastra/astras-pet-apps`; the pet's registry entry and art live there.

## Rules
- **One copy of the Fuzzboi rules.** The trait tables, decoding and drawing are in
  `findastra/fuzzbois` `site/fuzzboi.js`, served at `https://findastra.github.io/fuzzbois/site/`.
  This app loads that file and the layers from there. Never copy the rules into this repo; change
  them in `fuzzbois` so the Forge and this app agree.
- **Fuzzbois are Astra's own drawings.** Don't add other art, and don't redraw or "improve" the
  layers here.
- **The letter rule is temporary** (A–F count as 0–5, set 2026-10-09). Say so wherever a code
  with letters is shown, until Astra decides what letters mean.
- Follow the Cage's [PET-FILES.md](https://github.com/findastra/astras-pet-apps/blob/main/PET-FILES.md)
  and use its [PET-WORDS.md](https://github.com/findastra/astras-pet-apps/blob/main/PET-WORDS.md):
  pet, app, desktop pet, bubble, quick chat, app icon, pet well.
- Text goes into the page with `textContent`, never `innerHTML`.
- The repo description starts with the website link, and the repo's Website field is set to it.
- Say plainly what is not done. Update README "Limits" with every change.
- No pushing to `main` and no new GitHub repos without Astra's OK; use a branch and a PR.

## Handoffs
When Astra's request is unclear or sounds like an assignment, check `handoffs/` here and in
`findastra/astras-pet-apps` first. Leave a card when work remains. Format: the Cage's
[skills/handoff/SKILL.md](https://github.com/findastra/astras-pet-apps/blob/main/skills/handoff/SKILL.md).
