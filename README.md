# latal-plugins

Claude Code plugins by [lATAl](https://github.com/lATAl).

## Quick Start

```bash
# 1. Add marketplace
/plugin marketplace add lATAl/latal-plugins

# 2. Install plugin(s)
/plugin install elixir-lsp@latal-plugins
/plugin install pancake@latal-plugins
```

---

## Plugins

### elixir-lsp

Elixir LSP support via [Expert](https://github.com/elixir-lang/expert) — the official Elixir Language Server.

**Skills:** none (LSP only)

**Features:**
- Instant diagnostics after each edit
- Go to definition, find references
- Hover with type docs
- Supports `.ex`, `.exs`, `.heex`, `.eex`, `.leex`

**Requirements:** Expert binary in `$PATH`, Elixir >= 1.15.3, Erlang >= 25.0

**Install Expert:**

```bash
# macOS ARM64
gh release download nightly --pattern 'expert_darwin_arm64' --repo elixir-lang/expert --clobber

# macOS Intel
gh release download nightly --pattern 'expert_darwin_amd64' --repo elixir-lang/expert --clobber

# Linux x64
gh release download nightly --pattern 'expert_linux_amd64' --repo elixir-lang/expert --clobber

chmod +x expert_* && mv expert_* ~/.local/bin/expert
```

---

### pancake

PR review automation skills for GitHub workflows.

**Skills:**
- `/pancake:check-pr` — Analyze a PR's review comments, unresolved threads, and CI status
- `/pancake:review-loop` — Iterative review loop: push → trigger `/review` bot → fix → repeat until approved

**Requirements:** `gh` CLI authenticated, GitHub Actions bot configured for `/review` command

---

## License

Apache-2.0
