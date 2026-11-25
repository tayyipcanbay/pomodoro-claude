# Pomodoro for Claude

Pomodoro is a study desk for university students. You plan and review your studies with Claude, and you run focus sessions on the website's timer. This plugin connects Claude to your Pomodoro account and teaches Claude how to use it well.

Pomodoro is invite-only for now. You need an account at [the Pomodoro website](https://pomodoro.tayyipcanbay.dev) before the connector can sign in.

## What's inside

**Connector:** the Pomodoro MCP server at `https://pomodoro.tayyipcanbay.dev/mcp`. Claude reads and changes your own courses, topics, notes, deadlines, projects, papers, focus sessions and log through it.

**Skills:**

| Skill | Use it for |
|---|---|
| `study-setup` | Setting up your account from your transcript, module handbook and timetable, and moving notes in from Notion or PDFs |
| `study-coach` | Deciding what to study, lecture notes, hint-first exercise help, mock exams, topic mastery |
| `focus-sessions` | Planning focus sessions onto the timer and logging them afterwards |
| `weekly-review` | A weekly look at time studied, mastery and deadlines, and planning the next week |
| `research-companion` | Research projects and theses: milestones, papers, experiments, supervisor meetings |

## Getting started

1. Install the plugin. In Claude, open **Customize → Plugins → Add marketplace**, enter `tayyipcanbay/pomodoro-claude`, then install **Pomodoro**. In Claude Code, run `/plugin install pomodoro --marketplace tayyipcanbay/pomodoro-claude`.
2. Open the plugin's **Connectors** tab and select **Connect**.
3. Sign in with the Google account you use for Pomodoro and allow access.
4. Ask Claude: "Set up my studies" and share your transcript or module handbook.

## Data and privacy

- The plugin contains no code that runs on your computer. It holds the connector address and five instruction files (skills).
- When Claude uses a Pomodoro tool, Claude sends the tool's inputs (for example a note's text or a session's goals) to the Pomodoro server, which stores them in your account. Nothing is sent anywhere else.
- Sign-in uses OAuth 2.1 with PKCE. Pomodoro stores only hashes of access tokens. Access tokens last one hour.
- You can see and revoke Claude's access under **Settings → Connected apps** on the website, download all your data, or delete your account there.

## License

MIT. See [LICENSE](LICENSE).
