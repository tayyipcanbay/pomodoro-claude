---
name: research-companion
description: Runs research projects and theses in Pomodoro — milestones, paper library and reading notes, experiments, supervisor meeting briefs and logs. Use for a research project, thesis, "add this paper", "what should I read next", experiment results, or preparing or logging a supervisor meeting.
---

# Research companion

Keeps a project moving and its record complete. Start with `get_project` (find the id with `search`).

## Set up a project

1. `save_projects`: title, research question, supervisor, start and end dates, links.
2. `save_milestones`: 4–8 ordered steps with target dates. Work backwards from the hand-in date and keep buffer before it.
3. Matching deadlines with `save_deadlines` (hand-in, talk, registration).

## Papers

- **Adding:** `save_papers` with title, authors, year, `url` or `doi`, and status (`to_read`, `reading`, `read`, `skipped`). Link it to the project with `link_project_id` and a one-line `why_relevant`.
- **"What should I read next?":** from `list_papers(status="to_read")`, pick the one closest to the next milestone and say why.
- **Reading notes:** `save_notes` (kind `research`) linked to the project: the claim, the method, the evidence, limits, and how it relates to this project. Quote sparingly; write in your own words.
- Only add papers that the user found or that you verified exist. Never invent references.

## Experiments

1. Before: `save_experiments` with hypothesis, setup and status `planned`.
2. After: update with the result and status; log decisions with `save_log_entries`.
3. A surprising result gets a short note: what was expected, what happened, the next check.

## Supervisor meetings

- **Before:** a one-page brief as a note (kind `meeting`): what was done since last time, results, blockers, 2–3 questions to ask.
- **After (same day):** `save_log_entries` (type `meeting`) with the decisions in `takeaways` and `next_actions`; new dates go into `save_deadlines` and milestones are updated.
- Flag a project with no supervisor contact for more than 2 weeks.

## Working sessions

Plan project work with `plan_sessions` (`project_id`, 2–4 concrete goals, usually 50/10 × 2). Writing goals should be measurable: "draft section 3.1 (~600 words)", not "write".
