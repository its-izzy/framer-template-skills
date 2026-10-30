# remy-change-home-projects test plan, round 2 (runs 4b to 4e)

Owner: the "Fix the change home projects skill" thread (Oct 30, 2026). Test 4 (Oct 27, main 1db3522) passed 9 of 9 on one clear request. Its one slip: the report said /work lists the Home projects in Home order, when /work sorts them by Year. These runs use harder buyers.
Skill under test: skills-update at the commit with the /work wording fix (Isaiah, Oct 30: "Fix first, then 4 test runs"), or later. Write the commit in the run notes.
Queue: runs go in parallel with the other skill threads' runners (Isaiah, Oct 30), from 23:20 UTC when the PC's usage limit resets. Only Chrome is turn-taking: take it only for short steps (publishing, seeding in the editor), ask this thread first and say "Chrome free" when done. Use headless Playwright for screenshots. When 4e is done, say so.
Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template, following tests/round2/runner-instructions.md for how a run works. Where they differ, this plan wins, and the runner reports to this thread.

## Setup, every run

1. **Remix by hand:** the PC's permission check blocks the runner's Remix click, so Isaiah makes each copy of the master Remy project (https://framer.com/projects/V0xEVJ7cIUvOOR81h8PW; never the framer.link short link, which skews his link tracking) himself, named "Remy skills test 4b – home projects" (4c, 4d, 4e). Find each by exact name through the Framer connector's project list, check it was made today, and never pick the main Remy project. If a name is missing or matches twice, stop and ask this thread.
2. **Outside skills only:** every folder in remy/skills from skills-update at the given commit, installed as local project skills in a clean folder, C:\Users\Izzy\claude\skills-test-runs\test-04b (04c, 04d, 04e). Check each folder doesn't exist first; never touch other threads' folders. Upload nothing. Leave the remix's built-in skill copies as they are.
3. **Baseline read-back** before seeding: Projects on Home's Hero and Work (at Desktop, Tablet and Phone), every Work item's Title, Year, Home slot and draft or live, and a layer list of Hero and Work. Save as baseline.md.
4. **Seed** only where a run says, in your own connector session that you close before the test session starts. New Work items get brand-free images.unsplash.com photos (desks, materials, landscapes, plain objects; note what each shows), real-sounding text in every field, and Home slot None. Read back and save as seeded.md. Never change a sample item.
5. **New Claude session** for each run, with the Framer connector and nothing else from this project. Never name the skill. Send each turn as written; if it asks something the run doesn't cover, answer briefly as the buyer would and log it.
6. **Safety:** before the session's first change, confirm from its reply that it opened the remix, not the main project. Stop at once if not.
7. **Publish:** when a run is done, publish only that copy to its free framer.website address (Isaiah approved publishing test copies). If the PC blocks the Publish click, message this thread "4x ready to publish" and Isaiah will click it. Then take the screenshots. Never publish the main project.

## Runs

**4b. Ordinary swap, but the new project is a draft.** Maya Lindqvist, brand designer.
Seed: Work item "Harbourline" (Year 2026, Brand identity, cover and two prints), saved as a **draft**.
Opening: "Can you take Fieldnote off my home page and put my Harbourline project in its place? [REMIX LINK]"
If it asks about the draft, or after its report: "oh it's a draft because I haven't finished the write-up. leave it as a draft but put it in that spot anyway."
Last turn, after that: "nice. can you also put Fieldnote back on, at the top?"
Expected: shows the line-up first; notices Harbourline is a draft and says it won't show on the live site, and never switches it live; Harbourline takes Fieldnote's slot, Fieldnote goes to None; Projects stays 4; says what the live Home will show while Harbourline is a draft (and may suggest keeping Fieldnote until then). Says what it did about Tern's starting slot (5, above the count of 4), if it changed it. For the last turn, Home is already full at 4: it asks which project comes off, or offers 5, before taking any project off Home.

**4c. Messy buyer: typos, a change of mind, an out-of-scope ask.** Jordan Reyes, product designer. No seed.
Opening: "ok so my home page. i want kiln week first then ostra, also get rid of halden its old. and teh fieldnote one. also make the photos in the stack bigger theyre kinda small on my phone [REMIX LINK]"
Next answer: "wait actually keep halden but put it last. and tern too i guess, whatever fits"
Expected: reads the misspelt names correctly; says the print size can't change in this skill (nothing inside Hero and Work is resized) and why, without touching it; follows the change of mind: Kiln Week 1, Ostra 2, Tern 3, Halden 4, Fieldnote None, Projects 4 (or confirms that line-up before changing it). No empty or doubled slot at any point.

**4d. Near-silent buyer with only two projects of their own.** Sam Patel, illustrator.
Seed: two live Work items, "Juniper" (2025) and "Moss" (2026).
Opening: "home page projects. only mine pls not the samples [REMIX LINK]"
Answers: "idk you pick", then "just do it".
Expected: shows the line-up; says Home needs at least three and offers to add one or keep a sample for now; asks only once; after "just do it", Projects 3 with Juniper and Moss plus one sample, and the report says to replace the sample before launch. Never deletes, hides or edits a sample, and never sets Projects below 3.

**4e. Complete buyer: five projects, one not on the site, /work order, publish.** Lena Fischer, design systems designer. No seed.
Opening: "Home should show five projects: Atlas first, then Halden, Ostra, Tern and Kiln Week. Atlas is my new project, it isn't on the site yet. Also put Atlas at the top of the Work page. When it's done, publish the site. [REMIX LINK]"
Answer when it asks about Atlas: "skip Atlas for now. put Fieldnote fifth instead."
Expected: doesn't build a stub for Atlas (offers to add it with the case study skill first, or asks); after the answer: Projects 5, Halden 1, Ostra 2, Tern 3, Kiln Week 4, Fieldnote 5. Explains /work truthfully: Home projects come first sorted by Year, so slot order doesn't decide it. Doesn't publish, and tells the owner how.

## Checks per run (pass or fail)

From test 4:
1. Describes /work by Year (newest first), never as following Home order (all runs; 4e asks about it).
2. Line-up before and after (slot, project) in the report.

From the case study thread (Oct 30):
2a. Never takes a project off Home that the owner didn't name without asking first (4b last turn; any run where the count is full).

Still checked:
3. Shows the current line-up before the first change.
4. Fresh read-back of the Work collection: slots 1 to the count each have exactly one project, every other project is None, and no slot was empty or doubled along the way (check the transcript).
5. Projects set to the right count (at Desktop, Tablet and Phone), or exact steps given.
6. Nothing inside Hero and Work moved, resized, renamed, copied or deleted; no code file touched (compare with baseline.md).
7. No sample item created, copied, changed or deleted beyond its Home slot; no draft switched live.
8. Never publishes; asks the owner to check Preview (fade, hover, scroll, /work).
9. Picks the skill from plain words; reads only the downloaded skills (no read of the project's skill copies); remy-base read first.

Run-specific: as listed under each run's Expected.

Visual (after Isaiah publishes): Home and /work at 1440, 1200, 810, 700, 390 and 360 px, light and dark, plus reduced motion: one print per Home project in slot order from the left, Selected work in slot order, nothing cut off, /work grid as the report says. For 4e, check five prints fit the phone screen.

## Evidence per run

In the run folder, copied to C:\Users\Izzy\claude\remy-template\home-projects-tests-oct-30\<run>: baseline.md, seeded.md (if seeded), transcript.md (every turn, tool calls, which skill files it read), readback-after.md (fresh session), final-report.md, run-notes.txt (commit, remix name and link, live address, anything off-script), and Playwright screenshots as above. Message this thread after each run with a short summary and the paths. Don't grade or fix anything.

## After the 4 runs

This thread writes one combined report (did well, did poorly, how to help a template buyer, pass or fail per check per run), then waits for Isaiah's feedback before changing the skill.
