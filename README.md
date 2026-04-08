# vadash-plugins

Curated plugins for Claude Code by vadash.

## Add This Marketplace

From within Claude Code, run:

```
/plugin marketplace add vadash/claude-plugins
```

Or via the CLI:

```bash
claude plugin marketplace add vadash/claude-plugins
```

## Available Plugins

### claude-md-management

Tools to maintain and improve CLAUDE.md files - audit quality, capture session learnings, and keep project memory current.

**Install:**

```
/plugin install claude-md-management@vadash-plugins
```

**What's included:**

| Component | Type | Description |
|---|---|---|
| `claude-md-improver` | Skill | Audits CLAUDE.md files against current codebase state, outputs quality report, makes targeted updates |
| `/revise-claude-md` | Command | Captures learnings from the current session into CLAUDE.md |

## Manage Plugins

```shell
# List all plugins from this marketplace
/plugin list

# Uninstall a plugin
/plugin uninstall claude-md-management@vadash-plugins

# Update marketplace to get new plugins/versions
/plugin marketplace update vadash-plugins

# Remove marketplace entirely
/plugin marketplace remove vadash-plugins
```

## Structure

```
.
├── .claude-plugin/
│   └── marketplace.json      # Marketplace catalog
└── plugins/
    └── claude-md-management/
        ├── .claude-plugin/
        │   └── plugin.json   # Plugin manifest
        ├── commands/           # Slash commands
        ├── skills/             # Skills
        └── ...
```

## License

See individual plugin directories for license information.
