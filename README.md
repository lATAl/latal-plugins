# latal-plugins

Claude Code plugins by [lATAl](https://github.com/lATAl).

## Plugins

### elixir-lsp

Elixir LSP support using [Expert](https://github.com/elixir-lang/expert) - the official Elixir Language Server.

**Features:**
- Instant diagnostics (errors/warnings after each edit)
- Go to definition, find references
- Hover information with type docs
- Support for `.ex`, `.exs`, `.heex`, `.eex`, `.leex`

## Installation

### 1. Install Expert binary

```bash
# Download latest release
gh release download --pattern 'expert_*' --repo elixir-lang/expert

# Or nightly build
gh release download nightly --pattern 'expert_*' --repo elixir-lang/expert

# Make executable and move to PATH
chmod +x expert_*
mv expert_* ~/.local/bin/expert
```

Verify: `expert --version`

### 2. Add marketplace

```
/plugin marketplace add lATAl/latal-plugins
```

### 3. Install plugin

```
/plugin install elixir-lsp@latal-plugins
```

## Requirements

- Claude Code
- Expert binary in `$PATH`
- Elixir >= 1.15.3, Erlang >= 25.0

## License

Apache-2.0
