# Pomodoro for Claude

A quiet study desk for university students. Plan your week with Claude, keep your courses, notes and research in one place, and run the focus timer on the site.

**Live site:** [pomodoro.tayyipcanbay.dev](https://pomodoro.tayyipcanbay.dev) · invite-only for now.

This repository is a Claude plugin marketplace. Installing the **Pomodoro** plugin adds the connector and five study skills to Claude, so it knows how to plan, tutor and review without being told.

## Install

**In Claude (web or desktop app)**

1. Open **Customize → Plugins → Add marketplace** and enter `tayyipcanbay/pomodoro-claude`.
2. Find **Pomodoro** and choose **Install**.
3. Open the plugin's **Connectors** tab, choose **Connect**, and sign in with the Google account you use on the site.

**In Claude Code**

```
/plugin marketplace add tayyipcanbay/pomodoro-claude
/plugin install pomodoro@tayyipcanbay
```

## What's inside

- **The Pomodoro connector** — a remote MCP server that lets Claude read and change *your own* studies: courses, topics, notes, deadlines, projects, papers, focus sessions and your log.
- **Five skills** — study-setup, study-coach, focus-sessions, weekly-review and research-companion. See the [plugin README](plugins/pomodoro/README.md) for what each one does and what to say.

## Getting an account

Pomodoro is invite-only while it's young. Ask Tayyip for an invite, or request access from the [site](https://pomodoro.tayyipcanbay.dev), before you install.

## License

MIT — see [LICENSE](LICENSE).
