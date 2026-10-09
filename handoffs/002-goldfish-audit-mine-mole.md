status: open
for: goldfish (any assistant working on github-goldfish)
from: Claude Opus 5.5 (claude-opus-5-5), 2026-10-09
needs: findastra/github-goldfish AGENTS.md, astras-pet-apps PET-WORDS.md
---
## Task
A new pet app repo exists: **findastra/mine-mole** (public). Audit it:
1. Pet files: `pet.json`, the web app `mine-mole-20261009.html`, and the `pet-app` topic.
2. Expected gaps (not errors yet): no sprite or art until card 001 is done, and no registry entry on astras-pet-apps `main` until Astra OKs the commit. Report them as notes.
3. Mining-specific: check that no wallet seed, private key, pool password or `.env` is committed, now or later. Consider adding this as a standing Goldfish rule for this repo.

## Done when
Findings are in `handoffs/results/002-goldfish-mine-mole.md` here, with the model name and version at the top.

## Return
Commit on a branch and set `status: done`.
