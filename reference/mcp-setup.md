# DemoStance MCP — Setup

Connecting the MCP adds persistence, a character sheet, token economy, and a PPOV library to your DemoStance skill sessions. Without the MCP the skill still works fully — all coaching runs through conversation.

---

## Claude Code

Add to `~/.claude/settings.json`:

```json
{
  "mcpServers": {
    "demostance": {
      "command": "npx",
      "args": ["-y", "demostance-mcp@latest"]
    }
  }
}
```

Or via CLI (if available):
```bash
claude mcp add demostance -- npx -y demostance-mcp@latest
```

---

## Claude Desktop

Edit `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) or `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{
  "mcpServers": {
    "demostance": {
      "command": "npx",
      "args": ["-y", "demostance-mcp@latest"]
    }
  }
}
```

Restart Claude Desktop after saving.

---

## Add your User ID (for persistent profile)

1. Register at **demostance.com/signup** — free, takes 30 seconds. You get a User ID (`usr_xxxxxxxx`).
2. Add it to your MCP config:

```json
{
  "mcpServers": {
    "demostance": {
      "command": "npx",
      "args": ["-y", "demostance-mcp@latest"],
      "env": {
        "DEMOSTANCE_USER_ID": "usr_your-id-here"
      }
    }
  }
}
```

3. Restart your AI client. You'll be recognized automatically from now on — character sheet, tokens, and PPOV score persist across sessions.

---

## Verify the connection

After restarting, type `/demostance` — you should see your character sheet in the response. If you see the skill-only mode opening message instead, the MCP is not connected (check the config path and restart).
