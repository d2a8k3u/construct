# Claude Marketplace

Claude Code plugins in one marketplace: cross-project memory and a Slack board that drafts your replies. Add the marketplace once, then install the plugins you want.

## Install

```bash
claude plugin marketplace add d2a8k3u/claude-marketplace
claude plugin install <plugin>@d2a8k3u-construct
```

`<plugin>` is a name from the table below. Inside a Claude Code session, `/plugin` does the same from a menu. Start a new session to load the plugin.

| Plugin | What it does | Requirements and setup |
| --- | --- | --- |
| `adaptive-cognitive-memory` | One local memory for Claude Code, Codex and OpenCode, shared by every project: what the agent stores in one session comes back in later sessions, on any of the three. | [d2a8k3u/adaptive-cognitive-memory](https://github.com/d2a8k3u/adaptive-cognitive-memory) |
| `slack-board` | A board of your Slack messages: drafts replies in your tone of voice and sends them after your approval. | [d2a8k3u/slack-board](https://github.com/d2a8k3u/slack-board) |

If you added the marketplace when it was called `construct`, Claude Code keeps that name on your machine. Use `construct` wherever this page says `d2a8k3u-construct`, and do not add the marketplace again: installing from a second copy leaves the plugin enabled twice.

## Updates

Claude Code does not update this marketplace in the background until you turn auto-update on for `d2a8k3u-construct` under Marketplaces in `/plugin`. To update by hand:

```bash
claude plugin marketplace update d2a8k3u-construct
claude plugin update <plugin>@d2a8k3u-construct
```

Start a new session to load the update.

## Feedback

Report bugs and ideas in the plugin's own repository. Open an issue here only when the marketplace itself fails, for example when a plugin does not install from `d2a8k3u-construct`.

## License

MIT, see [LICENSE](LICENSE). Each plugin carries its own license.
