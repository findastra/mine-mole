# Rules for assistants working on Mine Mole (mine-mole)

*A pet app by Astra.* Public credit is always **Astra**. Keep work information out of this repo.

Started with Claude Opus 5.5 (`claude-opus-5-5`), 2026-10-09: research note, pet files, v0 calculator, handoff cards. Record your model name and version here when you change something substantial.

Draft sprite sheet and nine transparent mood frames added with OpenAI Codex (GPT-6), 2026-10-11, preserving the planned plum-purple mole, pink paws, teal hard hat, and silver pickaxe. Assets remain separate in `draft-art/mine-mole/` pending Astra's review; app behavior is unchanged.

## Rules
- **Research stage.** Do not add a miner, a miner download, or a wallet address until Astra has read the research and said yes.
- If mining goes ahead: it runs only on Astra's own PC, started by her, visible, and capped. Never hidden, never on anyone else's machine, never in a web page that visitors open.
- **Never commit** wallet seeds, private keys, pool passwords, API keys or `.env` files. A public wallet address is the most that may live in a local, git-ignored config.
- No dependencies. The web app works by double-click.
- Fetched or user text goes into the DOM with `textContent`, never `innerHTML`.
- Pet words follow `findastra/astras-pet-os` PET-WORDS.md. Art comes from the Cage's shared style (`scripts/generate-pets.mjs` there), never drawn ad hoc here.
- Work left for another assistant is a card in `handoffs/` (format: `astras-pet-os/skills/handoff/SKILL.md`).
- Say plainly what is not done. Numbers in the research are estimates with dates; recheck before relying on them.
