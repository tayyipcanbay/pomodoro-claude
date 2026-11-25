# Pomodoro

A study desk for university students, run together with Claude. You plan and review your studies in chat; you focus on the website's timer. Everything you and Claude write lands in one place, so the next conversation already knows where you are.

**Live site:** [pomodoro.tayyipcanbay.dev](https://pomodoro.tayyipcanbay.dev) · invite-only for now.

## Install

1. In Claude, open **Customize → Plugins → Add marketplace**, enter `tayyipcanbay/pomodoro-claude`, then install **Pomodoro**. In Claude Code: `/plugin install pomodoro@tayyipcanbay` after adding the marketplace.
2. Open the plugin's **Connectors** tab and choose **Connect**.
3. Sign in with the Google account you use on the site, and allow access.
4. In any chat, say: *"Use Pomodoro: show my overview."*

You need a Pomodoro account first — it's invite-only. Ask for one, or request access from the site.

## The skills

These switch on by themselves when they fit. You never name a skill; you just ask.

| Skill | What it does | Try saying |
|---|---|---|
| **study-setup** | Builds your account from a transcript, module handbook or timetable, and moves notes in from Notion or PDFs | *"Set up my semester: I study … and take … this term."* |
| **study-coach** | Picks what to study next, writes lecture notes, tutors exercises hint by hint, runs mock exams, tracks mastery | *"What should I study now?"* · *"Quiz me on Runge–Kutta."* |
| **focus-sessions** | Plans sessions onto the timer with concrete goals, then checks in and logs them | *"Plan my study day: 3 hours, exam topics first."* |
| **weekly-review** | Reviews your week — time studied, mastery, deadlines — and plans the next one honestly | *"How's my semester going? Review it and plan next week."* |
| **research-companion** | Runs a thesis or research project: milestones, a paper library, experiments, supervisor-meeting briefs | *"Set up my research project with milestones to the deadline."* |

## What Claude can touch

Through the connector, Claude reads and changes **only your own** data: your profile, courses, topics (with spaced-repetition mastery), notes, deadlines, projects, milestones, papers, experiments, focus sessions and log. It can't see anyone else's, and it never marks your goals done for you — you do that on the timer.

## Data and privacy

- The plugin runs no code on your computer. It holds the connector's address and five instruction files (the skills).
- When Claude uses a Pomodoro tool, it sends that tool's inputs — a note's text, a session's goals — to the Pomodoro server, which stores them in your account. Nothing goes anywhere else.
- Sign-in uses OAuth 2.1 with PKCE. The server stores only hashes of access tokens; access tokens last one hour.
- On the site, **Settings → Connected apps** lets you see and revoke Claude's access, download all your data, or delete your account.

## License

MIT — see [LICENSE](LICENSE).
