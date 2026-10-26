# Minimo Games for ChatGPT

The plugin marketplace that adds Minimo Games to ChatGPT, with its icon, and signs you in when you
install it.

## Install

In the ChatGPT desktop app:

1. Open **Plugins**, then **Add** > **Add a marketplace**.
2. Enter `minimo-games/chatgpt-marketplace` as the **Source**, and select **Add marketplace**.
3. Select **Browse directory**, then the **Personal** tab, and open **Minimo Games**.
4. Select **Install plugin**.
5. Sign in with your Minimo Games account, and select **Allow**.
6. Select **Try now** to start a conversation with Minimo Games.

With Codex in a terminal:

```bash
codex plugin marketplace add minimo-games/chatgpt-marketplace
codex plugin add minimo-games@minimo-games
```

Sign in afterwards with `codex mcp login minimo-games`: a plugin installed from the terminal is not
signed in by its install.

## Layout

```text
.agents/plugins/marketplace.json   catalog: one plugin, signed in on install
minimo-games/
  plugin.json                      manifest, with the listing and its icons
  mcp.json                         the remote MCP server, https://minimo.games/mcp
  assets/                          icon.png and logo.png
```

This repository is published from `plugin/chatgpt/` in the MinimoJS Framework repository, which is
its source.
