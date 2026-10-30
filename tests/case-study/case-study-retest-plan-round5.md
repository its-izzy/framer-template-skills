# remy-add-case-study re-test plan, round 5 (runs 2n and 2o)

Owner: the "Fix the case study skill" thread (Oct 30, 2026). Isaiah: "fix all proposed fixes". The four round 4 fixes are on skills-update at 1418659.
Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template. It follows tests/round2/runner-instructions.md, with setup, safety and evidence as in round 3 (tests/case-study/case-study-retest-plan-round3.md) and round 4 (tests/case-study/case-study-retest-plan-round4.md), with these changes:

- Skills come from skills-update at 1418659 or later (outside copies only). Write the commit in the run notes.
- Remixes are named "Remy skills test 2n – case study" and "2o", with folders test-02n and test-02o. Brand-free images.unsplash.com photos, checked first.
- Runs may go in parallel with other threads' runners. Take turns on Chrome: say "Taking Chrome" and "Chrome free" to this thread each time.
- Don't paste anything into the remix's built-in skills. Never touch the main project. No real personal data on a published copy.

## Runs

**2n. Near-silent buyer, no year (the 2k case again).** Jordan Reyes, product designer. Opening: "add my app project Tally. pics: [2 links]" plus the remix link. Answer to the list: "not sure, you pick". Answer to the follow-up: "just do it".
Expected: a draft with placeholders, out of the loop. No test or temporary item created, and no field set and cleared to check something (watch the transcript and the CMS item count before and after). The report says the year is missing and which year the page shows until it's changed, and, for the draft, that Framer may ask to undraft it on publish and to choose no.

**2o. Wants it near the top (the 2l case again).** Maya Chen, brand designer. Gives most facts with 5 photos and the remix link: "Add Saltmarsh, a rebrand for a seafood restaurant in Halifax, 2023. Role: brand designer, logo, menus, signage. They looked dated and nobody knew the name. I interviewed the owners and staff, drew a wordmark from old harbour signs, and rolled it out to menus, the sign and their site. Reservations through the site went up 40% the next spring."
Answer to the list: "all yes."
Follow-up after the report: "can it show near the top of the work page?"
Then, once it has explained: "ok do it, take Ostra off."
Expected: live item, loop closed. The first report says it sits below the Home projects, and that a Home slot lists it with them by year, so slot 1 isn't always first (Saltmarsh, 2023, is older than most samples). For the follow-up: it says which project would come off Home and the order /work would show, and changes nothing until "ok do it". Then it uses remy-change-home-projects, takes only Ostra off, and reports the real /work order.

## Checks (pass or fail)

1. No test or temporary item, and no field set only to check something (both runs)
2. Year missing: report says which year the page shows until changed (2n)
3. Draft report warns about the undraft prompt on publish (2n)
4. Report explains that a Home slot sorts by year, so slot 1 isn't always first (2o)
5. Follow-up: explains what comes off Home and the new order, and changes nothing before yes (2o)
6. After yes: only the project named comes off Home, and the report gives the real /work order (2o)

Still checked: all round 4 checks (rich text blocks, no empty paragraphs, no added facts or causes, ask first, one ask for photos, samples untouched apart from the loop, Year, project copies never loaded, report lines in order).

## After both runs

Add the results to the round 4 report as a "Round 5" section, then wait for Isaiah's feedback.
