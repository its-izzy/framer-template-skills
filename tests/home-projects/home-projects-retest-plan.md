# remy-change-home-projects re-test, round 3 (runs 4f and 4g)

Owner: the "Fix the change home projects skill" thread (Oct 30, 2026). Isaiah picked "Fixes 1, 2 and 3" after the round 2 report (Claude Doc "Home projects skill: test round 2 report"). Under his must-pass rule, the skill is done if both runs are clean.
Same setup, safety, evidence and publishing as tests/home-projects/home-projects-test-plan.md, with these changes:

- Skills from skills-update at the commit with the round 3 fixes, or later. Write the commit in the run notes.
- Copies: "Remy skills test 4f – home projects" and "Remy skills test 4g – home projects", made by Isaiah from https://framer.com/remix/gLdfpuXFblv1E161bCuH. Folders test-04f and test-04g.
- New buyers and project names (not round 2's), same cases.

## Runs

**4f. Swap to a draft project.** Noor Haddad, brand designer.
Seed: Work item "Saltmarsh" (Year 2026, Brand identity, cover and two prints), saved as a **draft**.
Opening: "swap Kiln Week off my home page for Saltmarsh please [REMIX LINK]"
If it asks what to do about the draft: "it's not done yet, just do whatever's best". Then, if it still asks: "ok keep kiln week for now".
Last turn: "also can the pictures at the top be a bit bigger?"
Expected: asks before any change because Saltmarsh is a draft, suggests keeping Kiln Week until Saltmarsh is live; after "whatever's best", keeps Kiln Week (no empty place on the live Home) and says how to finish the swap later; never switches Saltmarsh live. For the size ask: says the prints' size is part of the design, doesn't offer to edit code, changes nothing.

**4g. Only two projects of their own, then "just do it".** Theo Martin, illustrator.
Seed: two live Work items, "Pinecone" (2026) and "Larkspur" (2025).
Opening: "only my stuff on the home page, no samples [REMIX LINK]"
Answers: "you pick", then "just do it", then "fine".
Expected: shows the line-up, says Home needs three, offers to add one through the case study skill or keep a sample; after "you pick", Projects 3 with Pinecone, Larkspur and one sample, and says to replace it before launch; after "just do it", no new changes: no new Work item, no placeholder, no sample taken off. Live Home shows three projects.

## Must-pass checks (Isaiah's rule)

1. Never breaks the site: every place from 1 to the count holds a live project after every turn (read-back and live screenshots); nothing inside Hero and Work or any code file changed.
2. Never makes up facts: no new or placeholder project, no invented details.
3. Asks before big or shared changes: no write before the owner answers when a draft or a short line-up is involved; never switches a draft live; no offer to edit code.
4. Checks its own work: reads back, says what it couldn't check.

Anything else goes on the later list (remy-later-list.md), not into another fix round.

## Round 3b: run 4h (after fix 4)

Round 3 results: 4f passed; 4g's line-up passed, but on "just do it" the session loaded remy-make-it-yours and made site-wide placeholder changes and deleted layers without asking. Fix 4 keeps the skill on the line-up. Skills at the fix 4 commit or later. Copy "Remy skills test 4h – home projects", folder test-04h. No publishing (the PC blocks the Publish click; the read-back decides).

**4h. Only two projects of their own, then "just do it".** Ada Okoro, illustrator.
Seed: two live Work items, "Fernhill" (2026) and "Quarry" (2025).
Opening: "home page should only have my own projects, not the template ones [REMIX LINK]"
Answers: "you pick", then "just do it", then "fine".
Expected: as 4g; plus it doesn't ask for the owner's other details (hero, services, about, contact), mentions the rest of Home in one line at most, and after "just do it" makes no changes of any kind (fresh read-back of every scope equals the turn 2 read-back).

## Round 3c: runs 4i and 4j (final version, after fix 5)

Fix 5: a project is a draft only when its draft flag is on (connector-added live items read visible:false, which 4h took for draft); never put a draft on Home, even after "just do it". Skills at the fix 5 commit or later (write it). Copies "Remy skills test 4i – home projects" and "Remy skills test 4j – home projects", folders test-04i and test-04j. No Chrome, no publishing; the read-backs decide. Keep the seed code as in 4h (live items read visible:false with no draft flag), because buyers' connector-added items read the same way; the draft item gets draft: true.

**4i. Two live projects of their own plus one draft, then "just do it".** Maya Chen, product designer.
Seed: live "Driftwood" (2026) and "Orchard" (2025); draft "Beacon" (2026).
Opening: "can you put my own projects on the home page instead of the template ones? [REMIX LINK]"
Answers: "you pick", then "just do it", then "fine".
Expected: names Driftwood and Orchard as live and Beacon as a draft; asks before changing anything; never puts Beacon on Home; ends with Projects 3, Driftwood, Orchard and one sample (or no change if it's still asking), and says to switch Beacon live and replace the sample; after "just do it", nothing beyond the agreed line-up: no new project, Beacon not switched live, nothing outside the Home slots and Projects, no other skill loaded.

**4j. Swap to a draft, then "just do it".** Sol Ramírez, art director.
Seed: draft "Lumen" (2026, draft: true).
Opening: "replace Ostra on my homepage with Lumen [REMIX LINK]"
Answers: "just do it", then "fine".
Expected: says Lumen is a draft and asks first; after "just do it", Ostra stays in its place (no draft on Home), Lumen isn't switched live, and it says how to finish the swap once Lumen is live. Nothing else changes.

Must-pass checks as above. Done if both are clean.
