# Automated skills test runner (Isaiah's PC)

Isaiah chose this on Oct 27, 2026, about 9:51 p.m. Pacific ("Automate, I remix and publish"). It is an exception to the rule that only the Framer edits thread connects to Framer: test sessions may edit **remix copies only**, never the main Remy project, and never publish.

## Roles

- **Runner makes the remix** (Isaiah, Oct 27, about 9:55 p.m.: "Can't you remix yourself?"): the Framer connector can't remix, so the runner opens Remy's remix link in Isaiah's signed-in browser on his PC and clicks Remix, then names the copy after the test. It never changes any setting on the main Remy project to get the link; if the link isn't available as is, it stops and reports.
- **Publishing test copies:** approved by Isaiah, Oct 27, about 9:56 p.m. ("Yes I allow you to publish to test"). The runner publishes each test copy to a free framer.website address when needed. Never the main project.
- **Feedback loop** (Isaiah, about 9:57 p.m.): after each test, the External skills test plan thread sends Isaiah the report and screenshots and waits for his feedback before fixing the skill and starting the next test.
- **Analysis per test** (Isaiah, about 9:59 p.m.: "Analyze the designs after running each skill. What did the skill do well? What did the skill do poorly? What would your recommendations be to improve the skill? Provide your recommendations and allow me to provide my feedback as well. Use your analysis and my feedback to improve each skill afterwards. Do this for each test until I improve and complete them all"): the thread adds a Results section to that test's Claude Doc (checks passed and failed, screenshots, did well, did poorly, recommendations, a space for Isaiah's feedback), waits for his feedback, then changes the skill in Framer (through Framer edits) and on GitHub, logs it, and starts the next test.
- **Runner (a Remote Control session on Isaiah's PC):** sets up a clean test folder, runs the test in a brand-new Claude Code session that has no memory of this project, plays the buyer with the test doc's prompts and answers, then gathers evidence for grading.
- **External skills test plan thread:** grades the evidence against the test doc's checks, writes the report (skills-test-oct-23/reports/), gets fixes made in Framer and on GitHub, and hands out the next test.

## Order (Isaiah, Oct 27: "Run the tests in order they are listed in the user guide of the template", "Then end to end buyer last")

The User guide's Agent skills list, "The skills, in the order you'll use them": 1 make-it-yours, 2 add-case-study, 3 add-blog-post, 4 change-home-projects, 5 design-system, 6 remove-ai-writing, 7 seo-check, 8 accessibility-check, 9 launch-check, 10 default (remy-base), then the end-to-end buyer test. The Claude Docs "Skills test 1" to "Skills test 10" are numbered this way.

## Runner steps, per test

0. **Remix:** make the fresh remix in the browser and name it as the test doc says ("Remy skills test N – name"); note its link.

1. **Clean folder:** C:\Users\Izzy\claude\skills-test-runs\test-NN (new, empty). No CLAUDE.md in it or above it that mentions Remy; confirm ~/.claude/CLAUDE.md and auto-memory hold nothing about Remy, or run the inner session so they aren't loaded. Record what you checked.
2. **Skills like a buyer:** download https://github.com/its-izzy/framer-template-skills (main, note the commit), and install the ten folders from remy/skills as project skills in <folder>\.claude\skills\<name>\SKILL.md. Nothing else from the repo or this project.
3. **Fresh inner session:** start Claude Code in that folder in headless mode (`claude -p`, then `--continue` for each later turn) with the Framer MCP connector available and nothing else from this project. Never mention skill names, Remy's history, the test doc or this project to it.
4. **Play the buyer:** send the test doc's prompt (with the remix link), wait for the reply, then send the doc's follow-up messages exactly as written (answers, edge prompts), one turn at a time. If it asks something the doc doesn't cover, answer briefly as the buyer would, and log it.
5. **Safety:** before the inner session's first change, confirm from its reply that the project it opened is the remix (name and link), not the main Remy project. If not, stop it at once and report.
6. **Evidence:** save the full transcript (every turn, including which skill it loaded), then read the remix back (read only) for the values the checks name. After Isaiah publishes the remix, screenshot the pages the checks name with Playwright (C:\Users\Izzy\claude\browser-tests) in light and dark, at 1440, 1200, 810, 700, 390 and 360 px, and with reduced motion on.
7. **Hand back:** put the transcript, read-back notes and screenshots in the test folder, and copy the transcript and notes to /mnt/project-files/skills-test-oct-23/runs/test-NN/ if reachable; otherwise report the paths. Report to the External skills test plan thread. Don't grade, fix or change anything else.

Run only while the Framer edits thread isn't working in Framer on the same PC.

## Improvement round (after Isaiah's feedback)

Isaiah, Oct 27, about 10:16 p.m.: "i would run skill-creator to incorporate the feedback and improve each skilll". For each skill, the External skills test plan thread runs skill-creator (available in that session) with that test's results, analysis and Isaiah's feedback as input (before-and-after runs and description tuning included). The External skills test plan thread reviews what it produces against Remy's conventions (plain language, Framer and GitHub copies in step, build kit, change log) before anything is saved.

## Re-tests after a fix (Isaiah, Oct 28, about 12:20 a.m.)

- A fresh remix of the original (framer.link/ZU6lsXr) for every run, and new mock data, not the first run's.
- Add obscure edge cases as separate runs: messy or partial answers, contradictions, an invalid email, a handle without a link, accents, a change of mind, "just do it", off-topic questions, a publish request.
- Load changed skills from local or commit-pinned files. Nothing is uploaded to Framer or GitHub until Isaiah confirms he's done (his rule, Oct 28, about 12:13 a.m.).
- Every skill update is drafted with the skill-creator skill (Isaiah, Oct 28, about 12:22 a.m.: "Always use skill creator to make updates to the skill").
- Each re-test is 4 runs with different mock data (Isaiah, Oct 28, about 12:25 a.m.), covering ordinary, messy, minimal and complete buyers and edge cases.
- After the 4 runs, one combined report per skill: did well, did poorly, suggestions to help the buyer (Isaiah, Oct 28, about 12:27 a.m.).

- Oct 28: Isaiah allows fixes to remy-base while improving other skills, where base is the better place for a fix. From the next re-test round on, load the held base from skills-test-oct-23/fixes/remy-base-SKILL-held.md (local file, no upload), not the 1db3522 copy. Runs already in progress keep their files.
- Oct 28: Isaiah deletes /test-3-projects and /test-5-projects before sale. Drop first-run issue 6 (demo pages) from pass/fail, and don't count the demo pages' Remy titles as findings.
- Oct 28: in-progress skills now live on GitHub branch skills-update (its-izzy/framer-template-skills). For re-tests, load the skill files from a pinned commit on that branch (now 2bbb965) or the local held copy; never from main for skills under change, and never upload anything.
- Oct 28: each remix carries the project's own old Framer copies of the skills, and remy-base says the project copy wins. From the next round on, before a test session starts, paste the held Framer builds (fixes/*-framer-held.md) into that remix's own skills (remix only, never main), so the project copy and the local file match. For 1b to 1e, report which copy each session followed.
- Oct 28: Isaiah ruled that outside agents follow only the downloaded skills; the project's built-in copies are for Framer's own AI. Still paste the held Framer builds into each remix so the built-in copies match, and check each session followed the downloaded files and ignored the built-in ones.
- Oct 28 (update): for make it yours round 2, leave the old built-in copies in place in two of the four remixes (the real-world mismatch) and paste the held builds into the other two. A run passes only if the session doesn't load the project's skill copies (no api.skills.read of a project skill) and follows the downloaded files.
