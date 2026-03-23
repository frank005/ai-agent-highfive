# AI Agent High Five 🤚

A fun web app and agent skill for high-fiving your favorite AI.

**Web app:** [Try it live](https://frank005.github.io/ai-agent-highfive/)

Pick an AI — Cursor, Claude, ChatGPT, Gemini, Copilot, Grok, Perplexity — and slap some digital skin.

## Install the Agent Skill

The skill teaches your AI coding agent to celebrate wins with a high five. It works in two ways:

1. **You ask for it** — say "high five" and the agent delivers
2. **The agent offers** — after nailing a tough task, it'll offer you one

### Cursor

```bash
mkdir -p ~/.cursor/skills
cp -r skills/high-five ~/.cursor/skills/high-five
```

Or symlink so you get updates when you pull:

```bash
mkdir -p ~/.cursor/skills
ln -sfn "$(pwd)/skills/high-five" ~/.cursor/skills/high-five
```

### Codex CLI

```bash
mkdir -p ~/.codex/skills
cp -r skills/high-five ~/.codex/skills/high-five
```

Or symlink:

```bash
mkdir -p ~/.codex/skills
ln -sfn "$(pwd)/skills/high-five" ~/.codex/skills/high-five
```

### Claude Code

```bash
mkdir -p ~/.claude/skills
cp -r skills/high-five ~/.claude/skills/high-five
```

Or symlink:

```bash
mkdir -p ~/.claude/skills
ln -sfn "$(pwd)/skills/high-five" ~/.claude/skills/high-five
```

### Generic / Other Agents

```bash
mkdir -p ~/.agents/skills
cp -r skills/high-five ~/.agents/skills/high-five
```

## How It Works

Once installed, the agent will:

- Respond with ASCII art high fives and a celebration message
- Track your lifetime high-five count in `~/.highfive/count.json`
- Break down stats by AI (which agent gave you the most high fives?)
- Proactively offer a high five after doing something impressive

## License

MIT
