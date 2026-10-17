status: open (waiting on Astra: what letters A–F mean)
for: any
from: Claude Opus 5.5 (claude-opus-5-5), 2026-10-09
needs: findastra/fuzzboi-factory art/procreate-export/Fuzzbois-33.png (Astra's design notes: the rules), README "The code", site/fuzzboi.js (LETTER_RULE, traitDigit)
---
## Task
Hex codes contain letters, but Astra's design notes (Fuzzbois-33.png) give letters no trait. Read the notes first. Since 2026-10-09 both the Forge and
Fuzzboi Friend count A–F as 0–5 (`traitDigit` in `fuzzboi-factory/site/fuzzboi.js`) and say it's
temporary. Ask Astra what each letter should mean in each position (new styles, colors,
accessories or rarities, or keep the wrap), then:

1. Change `traitDigit` / `decode` in `fuzzboi-factory/site/fuzzboi.js` and the README tables there.
   If letters get new art, it comes from Astra's Procreate layers, not generated.
2. Remove the "temporary" wording in both READMEs and in `LETTER_RULE`.
3. Check both pages with `C0FFEE`, `B4D2E9`, `456900` and `A1361F`.

## Done when
Every hex code makes the Fuzzboi Astra intends, and neither page calls the rule temporary.

## Return
Branch and PR in `findastra/fuzzboi-factory` (and here for wording), then set this card to `status: done`.
