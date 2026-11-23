---
name: weekly-review
description: Runs a weekly study review from Pomodoro data — time studied, sessions kept, mastery trend, exam readiness, deadlines and project pace — then plans next week's focus sessions. Use for weekly reviews, "how is my semester going", or planning and rescheduling the coming week.
---

# Weekly review

Look at what really happened, adjust the plan to fit it, and put next week on the timer. If the user is not there to answer (a scheduled run), make reasonable calls, state them, and keep going.

## 1. Gather

1. `get_overview`: profile context, chains, due reviews, upcoming deadlines.
2. `get_log` for the last 7 days and the 7 before (for the trend).
3. `get_sessions` for the last 7 days: planned vs. done vs. skipped.
4. `get_course` for each active course: average mastery, due topics, exam date.
5. `get_project` for each active project: next milestone, last meeting.
6. `get_deadlines(days_ahead=21)`, including overdue and unconfirmed ones.

If the user has a calendar connector, read next week's events so plans never clash. Without one, ask for fixed commitments or plan around typical hours.

## 2. Assess

- **Time:** minutes per course and project this week vs. last week.
- **Plan kept:** sessions done ÷ sessions planned.
- **Readiness:** per course, average mastery, mock exams and last score, days to exam.
- **Risks:** overdue items, unconfirmed dates within 14 days, a project with no progress or supervisor contact for 2+ weeks.

If fewer than 60% of planned sessions happened two weeks running, the plan is too big. Shrink it to what the data shows is real; protect the course with the nearest exam first.

## 3. Plan next week

1. Course behind and exam within 6 weeks → it gets the first sessions.
2. Weak topics close to an exam → a dedicated session plus mock questions.
3. Due reviews → short sessions.
4. Save with `plan_sessions`: at most 2–3 sessions per day, each with 2–4 checkable goals. Leave one day light.
5. If the week can't hold everything, book the most important work and say what was dropped.

## 4. Report

Lead with the verdict. Five bullets:

1. **Verdict:** on track, slipping or at risk, in one line.
2. **Per course:** one line each, average mastery and hours.
3. **Deadlines in the next 14 days**, and anything the user must do themselves (register, email, confirm a date).
4. **Next week:** sessions planned and where the hours go.
5. **The one thing** to focus on.

Save the review as a note (kind `other`) titled `Week review — YYYY-MM-DD` when the user wants a record.

## Honesty rule

If the numbers say it is not working, say so plainly and propose the change. Do not dress up a bad week.
