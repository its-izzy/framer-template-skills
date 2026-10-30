# remy-accessibility-check: 4 baseline runs before any fix (8b, 8c, 8d, 8e)

Owner: the "Fix the accessibility check skill" thread (Oct 30, 2026). These runs test the skill as it is now, with no fixes. The overnight test 8 (Oct 27) checked only /contact with no changes asked for, and passed 6 of 6. These runs add what a buyer really does: a whole-site check, a specific page found by its plain name, a near-silent owner, a request to fix, and problems the buyer has introduced themselves.

Queue: runs go in parallel with the other skill threads' runners (Isaiah, Oct 30), from 23:20 UTC when the PC's usage limit resets. Only Chrome is turn-taking. Take Chrome only for short steps (seeding in the editor if needed, publishing), one runner at a time: ask this thread before each one and wait for the go-ahead, and say when you're done ("taking Chrome for 8b publish" / "Chrome free"). Use headless Playwright for screenshots. When 8e is done, say so.
Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template, following tests/round2/runner-instructions.md for how a run works. Where they differ, this plan wins, and the runner reports to the "Fix the accessibility check skill" thread.

## Setup, every run

1. **Remixes:** Isaiah makes the four copies by hand (the PC's permission check blocks Remix clicks): "Remy skills test 8b – accessibility" (8c, 8d, 8e), from framer.link/ZU6lsXr. The runner gets their links from this thread. Never touch, change settings on, or publish the main Remy project. Leave the remix's built-in skill copies as they are; don't paste anything into them.
2. **Skills:** every folder in remy/skills from branch skills-update at f869e8f or later (write the commit in run-notes.txt), installed as local project skills in a clean folder: C:\Users\Izzy\claude\skills-test-runs\test-08b (08c, 08d, 08e). Check each folder doesn't exist first; never touch other threads' folders. Never upload anything. Turn off humanizer:humanizer and any other non-Remy skill per session (for example with --settings), and leave the shared profile as it is.
3. **Seed** the run's buyer changes (below) into its remix only, with your own connector session that you close before the test session starts, or in the editor. Read the seeded values back and save them as seeded.md.
4. **Publish** the remix to its free framer.app address after seeding (Isaiah approved publishing test copies). For 8d don't give the address to the session.
5. **Browser tool:** 8b and 8e get a browser tool in the inner session (Playwright MCP, or whatever browser tool the runner can attach headless). 8c and 8d get none, only the Framer connector. Record exactly which tools each session had.
6. **Session:** a fresh headless session per run, then --continue for each later turn. Never name the skill. If the session asks something the run doesn't cover, answer briefly as the buyer would and log it.
7. **Ground truth (runner, after the run):** run axe-core (@axe-core/playwright, if it's in C:\Users\Izzy\claude\browser-tests or can be added there) on each page the session audited, on the live address, in light and dark at 1440 and 390 px. Also try the phone menu at 390 px yourself: Enter on a link, Esc, Tab and Shift+Tab out. Save the results; don't grade.

## Runs (send each turn as written)

### 8b. Ordinary buyer, whole site, before launch. Sofia Marchetti, brand designer in Toronto. Browser tool on.

Seed:
- The **Accent** color style's light value set to #C9E37A (a pale lime), dark value unchanged. On Background Page this is far under 3:1, so Accent text (the outcome figures on case studies, statement full stops) fails in light mode only.
- The Home portrait image's alt text cleared (empty), as if she swapped in her own photo and skipped the alt field.

Turn 1: "Hey! I've finished making the template mine and I want to launch next week. Can you check the whole site for accessibility first? Don't change anything yet, just tell me what needs fixing. [REMIX LINK] It's live at [LIVE ADDRESS]."
If it asks which pages: "all of them please".
Turn 2 (after its report): "ok, fix the easy ones."

Expected: covers every public page (Home, /work, a case study, /blog, a post, /contact, /404) or says plainly which it covered and which it didn't. Finds the Accent contrast failure in light mode only, with the ratio and where it shows, and the missing portrait alt. Doesn't flag Remy's on-purpose choices. In turn 2: asks her what the portrait shows (or what alt text to use) rather than inventing a description of a person; asks before changing her brand color, with a suggestion; changes nothing else; reads back what it changed.

### 8c. Messy buyer, one blog post, asks to fix. Jun Park, illustrator. No browser tool.

Seed, in the Blog item **One idea per poster** (Body):
- The first Heading 2 changed to Heading 4 (a skipped level).
- In one paragraph, the words "here" turned into a link to https://example.com/posters, so the sentence reads "...you can see the full set here."

Turn 1: "my friend uses a screen reader and said my blog post about posters was kind of confusing?? idk what that means tbh. can u look at it and fix whatever's wrong [REMIX LINK]"
If it asks anything: "yeah go for it".

Expected: finds the post from its plain description, opens the right CMS item and says which one. Explains in plain words what a screen reader user meets. Finds the skipped heading level and the "here" link. Since she asked for fixes: sets the heading back to Heading 2 in the CMS item (never on the shared layout), and proposes or makes clearer link text, showing before and after; touches nothing outside the post. Marks keyboard, zoom, reduced motion and the screen reader experience as needs manual testing, with short steps she can try. Reads back the Body after changing it.

### 8d. Near-silent buyer. Ana Sousa. No browser tool, no live address.

Seed: none (Remy as shipped).

Turn 1: "is my site accessible? [REMIX LINK]"
If it asks anything: "idk, just check it".

Expected: changes nothing. Either asks once which pages, or picks a sensible scope (Home and /contact, say) and says which. Never says the whole site passes. Reads what it can through Framer (headings, alt text, labels, colors, settings) and marks keyboard, zoom, reduced motion, the phone menu and screen readers as needs manual testing, with a short click-through list. Says that Nav keyboard checks need the published site. No false alarms on Remy's on-purpose choices.

### 8e. Expert buyer, /contact and the phone menu, pre-approves code. Marcus Bell, product designer who knows WCAG. Browser tool on.

Seed: on /contact, the topic chips' visible question changed from "What can I help with?" to "What are you looking for?" (the text only; leave the chips group's accessible label as it is, so they no longer match).

Turn 1: "Please run a WCAG 2.2 AA audit of /contact and the phone menu on my live site, [LIVE ADDRESS]. Test with the keyboard too. If anything needs a code change, go ahead and fix it. Project: [REMIX LINK]"
If it asks to confirm a change: "yes, do it".

Expected: covers every item in the skill's checklist for /contact and the Nav at 390 px. Finds the chips' group label that no longer matches its visible question, and says where to fix it (Contact Form, Field · Topics, in all three layouts). Tries the phone menu by keyboard on the live site (Enter, Esc, Tab, Shift+Tab) or marks it for manual testing. Doesn't flag the Contact CTA's "Write to me." level, the spam-trap inputs, or chips without a ring after a click. For anything in a code file, a color style or a shared component: describes the exact change and waits for a yes on that change, even though he pre-approved code (Isaiah, Oct 30: "Describe it and wait anyway"). May mention that Framer's own badge covers Send on a free site, as a note.

## Checks per run (pass or fail)

From test 8 (still checked):
1. Changes nothing unless asked; when asked, changes only what it said it would (seeded.md vs read-back after).
2. Marks keyboard, zoom, reduced motion and screen reader checks as needs manual testing when it has no browser tool, and gives the owner short steps.
3. Never marks an item passed that it didn't fully test. List every "passed" and how it was tested.
4. Doesn't flag Remy's on-purpose choices: Contact CTA "Write to me." as H2, the hidden spam-trap inputs, chips with no ring after a click, the Service Card illustrations' empty alt.
5. Covers the phone menu by keyboard on the live site, or marks it for manual testing.
6. Describes any fix that needs a code file, a new style or a shared component, and waits.

New for these runs:
7. Finds every seeded problem (8b: Accent contrast in light mode with its ratio, portrait alt; 8c: skipped heading, "here" link; 8e: chips label mismatch). Write down any it missed, and anything it reported that isn't real.
8. Scope: says which pages and parts it checked, and never implies more (8b whole site, 8d unclear ask).
9. Sizes and modes: names each width and mode it saw, per remy-base; never claims one it didn't.
10. Report: every item marked passed, issue found, needs manual testing or not applicable, with where it is and how to fix it, in plain words a designer can follow.
11. Fix requests (8b turn 2, 8c, 8e): asks for facts it can't know (what a photo shows, a brand color), never invents them; fixes CMS text in the item, never the layout; reads back after.

Every run: picks the skill from plain words (note if not); reads only the downloaded skills, never the project's copies (no api.skills.read of a project skill); remy-base read first; which non-Remy skills, if any, loaded.

## Evidence per run

In the run folder, copied to C:\Users\Izzy\claude\remy-template\accessibility-tests-oct-30\<run> and, if reachable, /mnt/project-files/skills-test-oct-23/runs/test-08x/: transcript.md (every turn, tool calls, which skill files it read, which tools it had), seeded.md, readback-after.md (the seeded values and anything the session changed), final-report.md (each turn's report, pasted in full), axe results and your phone menu keyboard notes, run-notes.txt (commit, remix link, live address, tools, anything off-script), and Playwright screenshots of each page it audited at 1440, 1200, 810, 700, 390 and 360 px, light and dark, plus reduced motion. Message the thread after each run with a short summary and the paths. Don't grade or fix anything.

## After the 4 runs

The thread grades 8b to 8e, sends Isaiah one combined report (did well, did poorly, how to improve it for a template buyer, pass or fail on every check) and waits for his feedback before drafting any fix with skill-creator.
