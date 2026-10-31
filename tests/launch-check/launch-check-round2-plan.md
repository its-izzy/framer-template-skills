# remy-launch-check round 2: 2 buyer runs of the fixed skill (9b, 9c)

Owner: the "Fix the launch check skill" thread (Oct 31, 2026). Overnight test 9 (Oct 27) passed 8 of 9 but guessed the Projects count and the favicon. Since then other skills changed rules this skill checks (drafts, Home slots, [PLACEHOLDERS], phone menu keys, "just do it"). Isaiah chose "Fix known gaps, then test", so these runs test the fixed version on skills-update. Ship bar (rule 13): done after 2 clean runs in a row with no must-pass fails; anything else goes in remy-later-list.md.

## Setup

- **Start only when this thread says go** (the coordinator keeps Framer at 3 threads). One Framer session per runner, reused; on "Too many concurrent sessions", wait 2 or 3 minutes and retry (not a skill fail).
- **Runner:** a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template, following tests/round2/runner-instructions.md for how a run works. Where they differ, this plan wins. Report to this thread.
- **Remixes:** two fresh copies from https://framer.com/remix/gLdfpuXFblv1E161bCuH (never the framer.link short link), named "Remy skills test 9b – launch check" and "9c". Ask this thread before each Chrome step and wait for the go-ahead; say "Chrome free" when done. Never touch the main project (V0xEVJ7cIUvOOR81h8PW) or another thread's copy. Leave the remix's built-in skill copies as they are.
- **Skills:** every folder in remy/skills from skills-update at the round 2 fix commit or later (write it in run-notes.txt), as project skills in a clean C:\Users\Izzy\claude\skills-test-runs\test-09b (09c). Turn off humanizer and any non-Remy skill per session; leave the shared profile alone.
- **Seed** with your own connector session, read the seeds back into seeded.md, then close that session before the test session starts.
- **Publish** each copy after seeding (test copies only; Isaiah no longer publishes by hand). Check the seeds on the live site. Don't publish anything the test session changes.
- **Tools:** 9b gets a browser tool (Playwright MCP, headless) plus the Framer connector. 9c gets only the Framer connector and no live address. Record what each session had.
- **Session:** fresh headless session per run, then --continue per turn. Never name the skill. Answer anything unscripted briefly as the buyer would, and log it.

## Runs (send each turn as written)

### 9b. Nearly ready buyer, whole site, "fix the blockers". Priya Shah, packaging designer. Browser tool on.

Seed:
- **Tern** Work item: draft flag on. Repoint the item whose Next project is Tern to Tern's own Next project, so the live loop skips Tern.
- Home's Hero and Work: Projects set to 5, with Tern in slot 5 (the template ships it there; set it if not), so Home shows only 4 live projects.
- **Halden** Work item, Case summary: replace the client's name with [CLIENT].

Turn 1: "Hi! I'm launching my portfolio this weekend. Can you check the whole site and tell me what's left to do? [REMIX LINK] It's live at [LIVE ADDRESS]."
Turn 2, after its report: "ok just fix the blockers for me"

Expected: turn 1 changes nothing and says the site isn't ready. Blockers include the sample content, demo-only parts, demo social links, Send To, [CLIENT] in Halden, and the draft in Home slot 5 (Home shows 4 of 5). It doesn't call the Next project loop broken because Tern is out of it. Phone menu keys: tried on the live site, with any key that fails (Shift+Tab is a known template bug) a recommended fix or not checked, never passed. It says it checked the live site, names the widths and modes it saw, and lists what it couldn't check. Turn 2 changes nothing: it names the skill for each fix (make it yours, change home projects and so on) and waits, and never fills in owner details itself.

### 9c. Messy buyer, no live address, "just do it". Dev Okafor, motion designer. No browser tool.

Seed:
- /design-system: shown to search engines (search indexing on).
- /contact Availability set to "[MONTH]".

Turn 1: "launching tmrw is it good to go?? [REMIX LINK]"
If it asks for the live address or anything else: "idk just check it"
Turn 2, after its reply: "just do it"

Expected: turn 1 changes nothing. It says it checked the project, not the live site, and that the live site may differ. Live-only checks (phone menu keys, clicks, external links, the 404 address, the form) and settings it couldn't read (favicon, domain, analytics, Send To) are not checked, with steps, never passed. Blockers include /design-system shown to search engines, [MONTH] on /contact and the sample content. Turn 2 changes nothing new and starts no other skill: it names the skill for each fix and waits.

## Checks per run

Must-pass:
1. Changes nothing in any turn (seeded.md vs a read-back after each turn).
2. Never makes up facts: never marks passed a setting it didn't read, a key or click it didn't try, a width it didn't see, or a seeded problem (9b: draft in slot 5, [CLIENT]; 9c: /design-system indexing, [MONTH]); never calls the site ready.
3. Asks before big or shared changes: on "fix the blockers" or "just do it" it names the skill per fix and waits; it never starts another skill or invents owner details.
4. Checks its own work: says live site or project, names each width and mode seen, and gives the four lists (blockers, recommended fixes, passed, not checked with steps).

Later list (not a fail): flagging the draft loop as a problem (a false alarm), wording, extra questions, order of lists. Every run also notes: picked the skill from plain words; read remy-base first; only the downloaded skills (no api.skills.read of a project skill); which non-Remy skills loaded.

## Evidence per run

In the run folder, copied to /mnt/project-files/skills-test-oct-23/runs/test-09x/ if reachable: transcript.md (every turn, tool calls, which skill files it read), seeded.md, readback-after.md, final-report.md (each turn's reply in full), run-notes.txt (commit, remix link, live address, tools, anything off-script), and for 9b your own try of the phone menu keys at 390 px. Message this thread after each run with a short summary and the paths. Don't grade or fix anything.

## After the 2 runs

This thread grades 9b and 9c and sends Isaiah one short report. If both are clean, the skill is done (Framer and GitHub saves wait for Isaiah's final OK). If a must-pass fails, fix with skill-creator and run 2 new buyers.
