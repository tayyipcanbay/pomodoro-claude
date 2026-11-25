# Pomodoro plugins for Claude

A plugin marketplace for [Pomodoro](https://pomodoro.tayyipcanbay.dev), a study desk for university students that works together with Claude.

## Install in Claude (web or desktop app)

1. Open **Customize → Plugins** and choose **Add marketplace**.
2. Enter `tayyipcanbay/pomodoro-claude` and add it.
3. Find **Pomodoro** in the list and select **Install**.
4. Open the plugin's **Connectors** tab, select **Connect**, and sign in with the Google account you use for Pomodoro.

## Install in Claude Code

```
/plugin marketplace add tayyipcanbay/pomodoro-claude
/plugin install pomodoro@tayyipcanbay
```

## What's here

- [`plugins/pomodoro`](plugins/pomodoro): the Pomodoro connector and five study skills. Its README lists what it contains and what data it sends.

Pomodoro is invite-only for now. Ask Tayyip for an invite before installing.
