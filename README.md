# UltimaPhoenix Claude Code plugins

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) hosting
UltimaPhoenix's plugins. Add it once, then install any plugin from it.

```bash
/plugin marketplace add UltimaPhoenix/claude-plugins-marketplace
/plugin install <plugin>@ultimaphoenix
```

## Plugins

| Plugin | Description | Source |
|--------|-------------|--------|
| **devcoach** | Progressive technical coach — auto-delivers personalized lessons as you work, tracks your knowledge map. Bundles the MCP server, Stop hooks, and coaching skill. Local only (Claude Code / Claude Desktop). | [UltimaPhoenix/dev-coach](https://github.com/UltimaPhoenix/dev-coach) (`plugin/`) |

```bash
/plugin install devcoach@ultimaphoenix
```

## Beta channel

Want what is coming next? [claude-plugins-marketplace-beta](https://github.com/UltimaPhoenix/claude-plugins-marketplace-beta)
carries the same plugins pinned to their latest canary build (`/plugin install devcoach@ultimaphoenix-beta`).
Enable one channel at a time: both ship the same hooks.

## Maintenance

`.claude-plugin/marketplace.json` is the catalog. Each plugin's own repo CI keeps its entry pinned to
the latest release tag (a surgical merge that never touches other entries). To add a plugin, append an
entry pointing at its repo (`github` or `git-subdir` source).
