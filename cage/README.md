# Cage registration, ready to apply

`cage-registration-20261009.patch` is the Farmer's card 006 work for `findastra/astras-pet-apps`, prepared on 2026-10-09 with Claude Opus 5.5 (`claude-opus-5-5`). Astra asked to keep it out of `astras-pet-apps` for now, so it waits here. It was checked to apply cleanly to that repo's `main` at the time.

What it adds there:

- `pets.json`: the Fuzzboi Friend entry (kind `fuzzboi`, `says` lines, live link), a new `fuzzboi` kind in `cage_life` (ground, hops like the Forge's parade), and an up-to-date Fuzzbois candidate line.
- `scripts/generate-pets.mjs`: the Fuzzboi Friend prompt, generated **from a reference** so the pet keeps Astra's design.
- `art/refs/fuzzboi-friend-ref-20261009.png`: that reference, composited only from Astra's own Fuzzboi layers (code `043001`: fuzzy black outline, ice-blue body, birthday hat) on plain grey. A copy is in this repo's `art/`.
- `apps/fuzzboi-friend-20261009.html`: a copy of this app.

**Not done:** the mood sheet. Generating it failed on 2026-10-09 because the OpenAI account had no credits left ("You have no credits remaining", error 429). Nothing was billed.

To finish, in an `astras-pet-apps` checkout on a branch:

```
git apply path/to/cage-registration-20261009.patch
node scripts/generate-pets.mjs fuzzboi-friend
npm run build && npm run check && npm test
```

Then look at the roster sheet, copy the nine frames into this repo's `art/`, list them in `sprite-20261009.json`, and set Cage card 006 to done.
