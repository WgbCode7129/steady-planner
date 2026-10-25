# Steady Planner

A free web app for Year 1 hall residents, built as the secondary product of **Steady@Hall**
(CC0015 Health & Wellbeing, NTU, TG63 Group 1).

It runs in any phone browser. There is nothing to install and no server code.

## What it does
- **Today**: your next chunk as an if–then plan ("IF it's Tue 4 pm in the common room → THEN I write the outline"), with Done, Not today and Add reminder (Google Calendar).
- **Off track? Re-plan**: missed chunks, or a whole week gone wrong, are re-planned in one tap: nearest deadline first, at most two chunks a day, on your free days, never past the cut-off. It then points you to the basics (a proper meal, sleep) and Flex Day.
- **9:30 pm guardrail**: after the deep-work cut-off, it offers to move unfinished chunks to your next free day instead of into your sleep. If something is due tomorrow, it offers a capped 45-minute last push instead.
- **Your timetable**: set your usual study time, your cut-off and the days you can't study (classes, CCA). Chunking and re-planning follow them.
- **Radar**: deadlines per teaching week, with crunch weeks flagged.
- **Plan**: add deadlines and split them into timed chunks with templates (essay, lab report, problem set, presentation, exam).
- **Check-in**: a 60-second weekly check-in. Green gets a tip, amber gets a Flex Day and an opt-in buddy kopi, and red shows help lines immediately. An "Are things improving?" card compares your sleep, meals, stress and chunks done with the previous week.

## Privacy
Everything is saved in the browser on the student's own phone (`localStorage`). Nothing is sent to a server.
Clearing the browser's site data erases it.

## Help lines shown in the app
NTU counselling 6790 4462 (office hours) · 6904 7041 (after hours) · SOS 1800 221 4444 (24 h) · IMH 6389 2222 (24 h) · Emergency 995

## Deploy (free)
This is a static site: `index.html` plus an icon and manifest, with no build step.
On Render, create a **Static Site** from this repo with an empty build command (or `echo`) and publish directory `.`,
or use **New → Blueprint**, which reads `render.yaml`.

## Credits
Built by TG63 Group 1 with generative AI assistance (Claude, Anthropic). If–then planning is based on
Gollwitzer & Sheeran (2006); the bedtime-procrastination guardrail on Kroese et al. (2014).
