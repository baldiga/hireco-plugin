# Hireco

Find the people in your LinkedIn network who can get you hired — hiring managers, decision makers, insiders at your target companies, recruiters, introducers who used to work there, and ex-coworkers who have seen your work. Ask in plain language; every answer comes with a ranked "who to talk to" list, an interactive radar map and a CSV.

## Requirements

- An early-access Hireco account and API key from [hireco.help/dashboard](https://hireco.help/dashboard).
- The Hireco Chrome extension, which syncs your 1st-degree LinkedIn connections from your own logged-in browser.

When you install the plugin you are asked for your Hireco API key. It is stored as a sensitive value in your system's credential store.

## What this plugin contains

- **Hireco MCP server** (remote, `https://hireco.help/api/mcp`), authenticated with your API key in the `Authorization` header. Tools: `get_started`, `find_hiring_paths`, `search_my_network`, `publish_map`, `enrich_prospects`, `get_person`. Prompts: `get-started`, `find-paths`.
- **`job-hunt` skill**: the workflow Claude follows — understand your target role and companies, map your network, rank warm paths, hand you the map and CSV, and offer outreach drafts.

There are no hooks, scripts or local executables.

## Data and network access

The plugin only talks to `https://hireco.help`. Requests carry your API key and the questions your AI asks (role keywords, target companies, people to look up). Responses contain your own synced connections and the maps and CSV links Hireco creates for you (kept 14 days). Premium enrichment, which you approve per request, fetches public professional profiles through a third-party provider. See the [privacy policy](https://hireco.help/privacy).

## Support

[hireco.help/support](https://hireco.help/support) · License: MIT
