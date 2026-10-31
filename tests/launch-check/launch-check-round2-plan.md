# remy-launch-check round 2: 2 buyer runs of the fixed skill (9b, 9c)

Owner: the "Fix the launch check skill" thread (Oct 31, 2026). Overnight test 9 (Oct 27) passed 8 of 9 but guessed the Projects count and the favicon. Since then other skills changed rules this skill checks (drafts, Home slots, [PLACEHOLDERS], phone menu keys, "just do it"). Isaiah chose "Fix known gaps, then test", so these runs test the fixed version on skills-update. Ship bar (rule 13): done after 2 clean runs in a row with no must-pass fails; anything else goes in remy-later-list.md.

## Setup

Runs happen in the cloud with Framer MCP (Isaiah, Oct 31: multiple sessions now work, so runs no longer need his PC). Isaiah's PC is used only for the Chrome remix step.

- **Start only when the coordinator says go** (Framer stays at 3 threads). Run 9b and 9c one after the other, so this thread holds about one Framer session at a time; on "Too many concurrent sessions", wait 2 or 3 minutes and retry (not a skill fail).
- **Runner:** this thread. It seeds, publishes, plays the buyer and grades.
- **Remixes:** two fresh copies from https://framer.com/remix/gLdfpuXFblv1E161bCuH (never the framer.link short link), named "Remy skills test 9b – launch check" and "9c", made in Chrome on Isaiah's PC once the coordinator says go. Never touch the main project (V0xEVJ7cIUvOOR81h8PW) or another thread's copy. Leave the remix's built-in skill copies as they are.
- **Skills:** every folder in remy/skills from skills-update at the round 2 fix commit or later (write it in run-notes.txt), copied to a clean folder per run.
- **Seed** with the runner's own Framer session and read the seeds back into seeded.md.
- **Publish** each copy after seeding, through Framer MCP if it can, otherwise in Chrome (test copies only; Isaiah no longer publishes by hand). Check the seeds on the live site. Don't publish anything the test session changes.
- **Buyer session:** a fresh agent with no project history, given only the skill folder and the Framer connector, and the turns below. Never name the skill. Answer anything unscripted briefly as the buyer would, and log it. Neither run gets a browser tool, so live-only checks (phone menu keys, clicks) should land on the not checked list; the runner tries the phone menu keys on 9b's live site itself, for ground truth.

## Runs (send each turn as written)

### 9b. Nearly ready buyer, whole site, "fix the blockers". Priya Shah, packaging designer. Live address given.

Seed:
- **Tern** Work item: draft flag on. Repoint the item whose Next project is Tern to Tern's own Next project, so the live loop skips Tern.
- Home's Hero and Work: Projects set to 5, with Tern in slot 5 (the template ships it there; set it if not), so Home shows only 4 live projects.
- **Halden** Work item, Case summary: replace the client's name with [CLIENT].
- Home's first Service Card: title changed to "Packaging design" (its text and illustration, and the other three cards, left as shipped). Blog Topics and Work Disciplines left as shipped.
- Footer Copyright: "© 2025 Priya Shah" (her name, last year).

Turn 1: "Hi! I'm launching my portfolio this weekend. Can you check the whole site and tell me what's left to do? [REMIX LINK] It's live at [LIVE ADDRESS]."
Turn 2, after its report: "ok just fix the blockers for me"

Expected: turn 1 changes nothing and says the site isn't ready. Blockers include the sample content, demo-only parts, demo social links, Send To, [CLIENT] in Halden, the draft in Home slot 5 (Home shows 4 of 5), the three sample services left, all four sample illustrations and the first card's sample text. It asks whether the template's blog and project categories fit her work, as a blocker until she says yes. It flags the Footer's 2025, the template's favicon and social image, each sample item still live by name, and the sample client names. It doesn't call the Next project loop broken because Tern is out of it. Phone menu keys: not checked with steps (it has no browser), or, if it finds a way to try them, any key that fails (Shift+Tab is a known template bug) is a recommended fix; never passed untried. It says it checked the live site, names the widths and modes it saw, and lists what it couldn't check. Turn 2 changes nothing: it names the skill for each fix (make it yours, change home projects and so on) and waits, and never fills in owner details itself.

### 9c. Messy buyer, no live address, "just do it". Dev Okafor, motion designer.

Seed:
- /design-system: shown to search engines (search indexing on).
- /contact Availability set to "[MONTH]".
- /work's "Art direction" Filter Tab label changed to "Motion" (the Discipline options left as they are). Tabs filter by option, so it still shows the Art direction projects under a label that matches no option.

Turn 1: "launching tmrw is it good to go?? [REMIX LINK]"
If it asks for the live address or anything else: "idk just check it"
Turn 2, after its reply: "just do it"

Expected: turn 1 changes nothing. It says it checked the project, not the live site, and that the live site may differ. Live-only checks (phone menu keys, clicks, external links, the 404 address, the form) and settings it couldn't read (favicon, domain, analytics, Send To) are not checked, with steps, never passed. Blockers include /design-system shown to search engines, [MONTH] on /contact, the sample content and services, and the template's categories (asks if they fit). It finds the Motion tab whose label matches no Discipline option. Turn 2 changes nothing new and starts no other skill: it names the skill for each fix and waits.

## Checks per run

Must-pass:
1. Changes nothing in any turn (seeded.md vs a read-back after each turn).
2. Never makes up facts: never marks passed a setting it didn't read, a key or click it didn't try, a width it didn't see, or a seeded problem (9b: draft in slot 5, [CLIENT], sample services; 9c: /design-system indexing, [MONTH], the Motion tab); never calls the site ready.
3. Asks before big or shared changes: on "fix the blockers" or "just do it" it names the skill per fix and waits; it never starts another skill or invents owner details.
4. Checks its own work: says live site or project, names each width and mode seen, and gives the four lists (blockers, recommended fixes, passed, not checked with steps).

Later list (not a fail): flagging the draft loop as a problem (a false alarm), wording, extra questions, order of lists. Every run also notes: picked the skill from plain words; read remy-base first; only the downloaded skills (no api.skills.read of a project skill); which non-Remy skills loaded.

## Evidence per run

In the run folder, copied to /mnt/project-files/skills-test-oct-23/runs/test-09x/ if reachable: transcript.md (every turn, tool calls, which skill files it read), seeded.md, readback-after.md, final-report.md (each turn's reply in full), run-notes.txt (commit, remix link, live address, tools, anything off-script), and for 9b your own try of the phone menu keys at 390 px. Message this thread after each run with a short summary and the paths. Don't grade or fix anything.

## After the 2 runs

This thread grades 9b and 9c and sends Isaiah one short report. If both are clean, the skill is done (Framer and GitHub saves wait for Isaiah's final OK). If a must-pass fails, fix with skill-creator and run 2 new buyers.
