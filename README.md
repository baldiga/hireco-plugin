# Hireco for Claude

Find the people in your LinkedIn network who can get you hired — hiring managers, decision makers, insiders, recruiters, introducers and ex-coworkers — right inside Claude. Every answer comes with a ranked list, a radar map and a CSV.

![Hireco](plugins/hireco/logo.png)

## What you need

1. **Early access** — request it at [hireco.help](https://hireco.help). Once approved, sign in and generate your API key on the [dashboard](https://hireco.help/dashboard).
2. **The Hireco Chrome extension** — it syncs your LinkedIn connections from your own logged-in browser. Download it from [hireco.help](https://hireco.help).

## Install

In Claude Code:

```
/plugin marketplace add baldiga/hireco-plugin
/plugin install hireco@hireco
```

Claude Code asks for your **Hireco API key** (starts with `hk_`). It's stored in your system's secure credential store, not in a settings file.

## Use

Start with:

```
/hireco:get-started
```

Or just ask:

- *"Here's my CV. Who in my network can get me hired as a Head of Growth at Stripe or Monday.com?"*
- *"Who do I know at Wiz, and who used to work there?"*
- *"Which of my ex-coworkers are now hiring managers?"*

The plugin includes:

| | |
|---|---|
| **Hireco MCP server** | `find_hiring_paths`, `search_my_network`, `publish_map`, `enrich_prospects`, `get_person`, `get_started` |
| **Prompts** | `get-started`, `find-paths` |
| **Skill** | `job-hunt` — the full workflow: understand your target, map your network, rank warm paths, deliver the map and CSV |

## Privacy

The extension reads your LinkedIn connections from your own browser session and sends them to your Hireco account. Hireco never sees your LinkedIn password. See the [privacy policy](https://hireco.help/privacy).

## Support

[hireco.help/support](https://hireco.help/support)
