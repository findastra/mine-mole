status: open (art waits on OpenAI credits)
for: farmer (any assistant working on astras-pet-apps)
from: Claude Opus 5.5 (claude-opus-5-5), 2026-10-09
needs: astras-pet-apps PET-FILES.md "Adding a pet to the Cage", PET-WORDS.md, pets.json; this repo's README and pet.json
---
## Task
Welcome **Mine Mole** (`mine-mole`) to the Cage. The registry and prompt edits are ready as a patch in this repo, [001-cage-registration-20261009.patch](001-cage-registration-20261009.patch), made against astras-pet-apps `main` at 52637db. Apply it in astras-pet-apps with `git apply <path-to>/001-cage-registration-20261009.patch` (use `git apply -3` if `main` has moved). It adds:

- `pets.json`: the entry (`kind: "mole"`, `status: "hatching"`, `asset_date: "20261009"`, public, `says` lines), a new `cage_life.kinds.mole` (`zone: "ground"`), and friends `["mine-mole", "finance-finch"]`.
- `scripts/generate-pets.mjs`: its prompt. Plum-purple fur, hot pink nose and paws, electric teal hard hat with a white-hot lamp, silver pickaxe. No other pet uses this palette.

Still to do:
1. Once OpenAI credits are back: `node scripts/generate-pets.mjs mine-mole` (one paid image). On 2026-10-09 it failed with "no credits remaining" and nothing was billed.
2. Copy `mine-mole-20261009.html` from this repo to `apps/mine-mole-20261009.html` and set `interface_url` and `interface_local_url`.
3. `npm run build`, look at the roster sheet, `npm run check`, `npm test`. Copy the nine frames to this repo's `art/` and fill in `sprite`.

## Done when
Mine Mole shows in the Cage and ROSTER.md with nine draft moods, and the checks pass. The art stays a draft until Astra approves it.

## Return
Commit on the branch, open a PR once Astra says so, and set this card to `status: done`.
