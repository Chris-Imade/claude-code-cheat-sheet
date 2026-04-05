# Claude Code CLI — Cheat Sheet

> A comprehensive, interactive cheat sheet for **Claude Code CLI** users. 100+ commands, shortcuts, flags, config references, hooks, MCP setup, and pro tips — all in a single, searchable HTML page with a terminal-inspired dark UI.

![Claude Code](https://img.shields.io/badge/Claude_Code-v2.1.92-d97706?style=for-the-badge&labelColor=1a1120)
![HTML](https://img.shields.io/badge/HTML-CSS-a78bfa?style=for-the-badge&labelColor=1a1120)
![License](https://img.shields.io/badge/License-MIT-34d399?style=for-the-badge&labelColor=1a1120)

---

## Features

- **100+ commands** across 13 categorized sections
- **Instant fuzzy search** — press `/` to focus, `Esc` to clear
- **Category filter tabs** — Slash, Keys, CLI, Config, Hooks, Env, MCP, Agents, Tips
- **Expandable descriptions** — click any card to reveal detailed docs with code examples
- **Terminal aesthetic** — dark purple/orange Claude Code palette, scanline overlay, monospace typography
- **Zero dependencies** — single self-contained HTML file (only external: Google Fonts)
- **Fully responsive** — works on desktop, tablet, and mobile

## Sections Covered

| Section | Count | What's Inside |
|---------|-------|---------------|
| 📦 Installation | 4 | Native install, Homebrew, doctor, auth |
| ⚡ Slash Commands | 30+ | `/init`, `/compact`, `/model`, `/plan`, `/voice`, `/security-review`, and more |
| ⌨️ Keyboard Shortcuts | 15 | Ctrl combos, navigation, history, autocomplete |
| ⟫ Quick Prefixes | 5 | `#` memory, `/` slash, `!` shell, `@` file, `&` background |
| $ CLI Flags | 14 | `-p`, `-c`, `-r`, `--model`, `--max-turns`, `--output-format` |
| ⚙️ Configuration | 9 | settings.json, CLAUDE.md, custom commands, skills, agents, .mcp.json |
| 🔒 Permission Modes | 5 | default, acceptEdits, auto, plan, cycling |
| ⟁ Hooks | 8 | PreToolUse, PostToolUse, Stop, SessionStart, FileChanged |
| ◈ Environment Variables | 10 | Auth, model config, cloud providers, timeouts |
| ⬡ MCP | 7 | Setup commands, Context7, Playwright, Memory, Filesystem |
| ◎ Subagents | 5 | Explore agent, background tasks, custom agent definitions |
| ★ Pro Tips | 8 | Pipe workflows, PR review, OpenRouter, CI/CD integration |
| 📁 Key File Locations | 8 | Every config path at a glance |

## Quick Start

```bash
# Clone the repo
git clone https://github.com/your-username/claude-code-cheatsheet.git
cd claude-code-cheatsheet

# Open directly in your browser
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Or serve it locally:

```bash
python3 -m http.server 8080
# Visit http://localhost:8080
```

## Usage

| Action | How |
|--------|-----|
| **Search** | Type in the search bar or press `/` |
| **Clear search** | Press `Esc` |
| **Filter by category** | Click a tab (Slash, Keys, CLI, etc.) |
| **Expand a command** | Click any card to reveal description + code examples |
| **Collapse a command** | Click the card header again |

## Design

- **Color palette** — Claude Code's signature dark purples (`#1a1120`, `#231730`) with warm orange accents (`#d97706`)
- **Typography** — JetBrains Mono for that terminal feel, Inter for headings
- **Scanline overlay** — subtle CRT-style effect for extra dev ambiance
- **Terminal chrome** — red/yellow/green dots, prompt cursor, version badge

## Data Sources

- [Official Claude Code documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Blake Crosley's Claude Code Cheat Sheet](https://blakecrosley.com/guides/claude-code-cheatsheet)
- [Shipyard Claude Code Cheatsheet](https://shipyard.build/blog/claude-code-cheat-sheet/)
- [OpenRouter Claude Code Integration Guide](https://openrouter.ai/docs/guides/coding-agents/claude-code-integration)

## Contributing

Contributions are welcome! To add or update commands:

1. Fork the repo
2. Edit the `DATA` array in `index.html` (search for `const DATA =`)
3. Follow the existing object format:
   ```js
   {
     cmd: "command name",
     tag: "slash",          // slash | keyboard | cli | config | hook | env | mcp | agent | tip | prefix | perm
     tagLabel: "Slash",     // Display label for the tag
     short: "Brief desc",   // Shown inline on the card
     desc: "Full HTML description with <code>examples</code>"
   }
   ```
4. Submit a PR

## License

MIT — use it, share it, put it on your wall.

---

<p align="center">
  <b>Built for developers who live in the terminal.</b><br>
  <sub>▐▛█▜▌ Claude Code CLI Cheat Sheet</sub>
</p>
