# Cage registration, ready to apply

`cage-registration-20261009.patch` is the Farmer's card 006 work for `findastra/astras-pet-apps`, prepared on 2026-10-09 with Claude Opus 5.5 (`claude-opus-5-5`). Astra asked to keep it out of `astras-pet-apps` for now, so it waits here. It was checked to apply cleanly to that repo's `main` at the time.

What it adds there:

- `pets.json`: the Fuzzboi Friend entry (kind `fuzzboi`, `says` lines, live link), a new `fuzzboi` kind in `cage_life` (ground, hops like the Forge's parade), and an up-to-date Fuzzbois candidate line.
- `scripts/generate-pets.mjs`: the Fuzzboi Friend prompt, generated **from a reference** so the pet keeps Astra's design.
- `art/refs/fuzzboi-friend-ref-20261009.png`: that reference, composited only from Astra's own Fuzzboi layers (code `043001`: fuzzy black outline, ice-blue body, birthday hat) on plain grey. A copy is in this repo's `art/`.
- `apps/fuzzboi-friend-20261009.html`: a copy of this app (its pet well falls back to the Cage's frames).
- **The generated art:** `art/sheets/fuzzboi-friend-20261009.png` (the paid mood sheet, generated 2026-10-09 after Astra added credits) and the nine 256×256 frames in `art/frames/fuzzboi-friend/`, plus the rebuilt `ROSTER.md`, README table, `cage-data.js`, `art/frames/index.json` and `art/roster.png`. Draft until Astra approves it.

With it applied, `npm run check` says "Cage OK: 19 pet apps" and all 48 tests pass (checked 2026-10-09 against `main` at `52637db`).

To finish, in an `astras-pet-apps` checkout on a branch. **Don't run the generator again**: the sheet is in the patch, and a re-run would only cost money.

```
git apply path/to/cage-registration-20261009.patch
npm run build && npm run check && npm test
```

Then set Cage card 006 to done. If `main` has moved and the patch doesn't apply, apply it to `52637db` and merge, or re-run `npm run build` after resolving `pets.json`: the generated files are rebuilt from it.
