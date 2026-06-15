# DemoStance Skill

Demo psychology coach for Sales Engineers (SE/AE/Presales) in B2B SaaS software sales. Turns generic feature tours into opinionated demos built around a Provocative Point of View (PPOV) that win deals and close opportunities.

**Tags:** `sales engineer` · `demo` · `SaaS` · `B2B` · `sales` · `pitch` · `software demo` · `opportunity` · `deal` · `PPOV` · `presales` · `demo script` · `SE coaching` · `AE` · `pipeline`

Works **with or without** the DemoStance MCP — skill-only mode gives you full PPOV coaching through conversation; MCP adds persistence, gamification, and a character sheet.

---

## Install

### Claude Code / Cursor / Windsurf

```bash
npx skills add demostance/demostance-skill -g -y
```

Then type `/demostance` in any Claude Code session.

### Claude Desktop (Project Instructions)

1. Open Claude Desktop → **New Project**
2. Go to **Project Instructions**
3. Paste the full contents of `SKILL.md` into the instructions field
4. Save — Claude now behaves as your DemoStance coach in every conversation in this project

No MCP required. All coaching happens through conversation.

---

## Usage

```
/demostance build    — Start from discovery notes → PPOV → Demo flow
/demostance analyze  — Score existing material (script, PPT, transcript)
/demostance check    — Quick traffic-light review of a draft outline
```

Also auto-activates on trigger phrases like:
- "Wie ist diese Demo?" / "How does this demo look?"
- "Ich habe morgen einen Demo-Termin" / "I have a demo tomorrow"
- "Ich brauche eine starke These für die Demo" / "I need a strong thesis for the demo"

---

## Connect the MCP (optional — for persistence & gamification)

The MCP unlocks: character sheet, token economy, PPOV library, demo export.

→ See [`reference/mcp-setup.md`](reference/mcp-setup.md) for setup instructions.

---

## Update

```bash
npx skills update demostance -g
```

---

## License

MIT — see `LICENSE.txt`
