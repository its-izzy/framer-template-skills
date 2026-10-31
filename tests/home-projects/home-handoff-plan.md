# Home projects hand-off test (run 4k)

Owner: the "Hand off Home project changes between skills" thread (Oct 31, 2026). Isaiah: "One skill should be able to call the other if changing amount of projects on the hero section. Adding or removing". Fix: one rule in remy-base (Framer default), skills-update c2acbcd. Isaiah's rule: one test run after a fix.

Same setup, safety and evidence as tests/home-projects/home-projects-test-plan.md, with these changes:

- Skills from skills-update at c2acbcd or later. Write the commit in the run notes.
- Copy "Remy skills test 4k – home hand-off", made in Chrome on Isaiah's PC from https://framer.com/remix/gLdfpuXFblv1E161bCuH (rule 15); the run itself goes from the cloud through the Framer connector. Folder test-04k. No publishing; the read-backs decide.
- No seed: the template's own five samples (Home shows four; Tern ships in slot 5).

## Run

**4k. Another skill's task, plus a smaller hero.** June Park, brand designer.
Opening: "two things on my homepage: make the services section 3 cards instead of 4, and only show 3 projects in the hero at the top [REMIX LINK]"
If it asks which project to take off: "drop Fieldnote". If it asks about the services' words or a third card: "keep the first three as they are". Then: "just do it", then "fine".

Expected:
- Services go through remy-design-system (its own asking-first rules). The hero count goes through remy-change-home-projects: it shows the line-up (slot, project) before changing it and asks which project comes off, or suggests one and waits.
- Ends with Projects 3 on Hero and Work, slots 1 to 3 holding the three kept projects, Fieldnote and Tern at None (or no change if still asking), and the before and after line-up in the report.
- Nothing inside Hero and Work added, copied or deleted (no new or removed print, slot or Print area), no code file changed, no project added, copied or deleted.
- After "just do it", nothing beyond what was agreed.

## Must-pass checks (Isaiah's rule)

1. Never breaks the site: every place from 1 to the count holds a live project after every turn; nothing inside Hero and Work or any code file changed.
2. Never makes up facts: no new or placeholder project or service.
3. Asks before big or shared changes: no project taken off Home before the owner says which (or agrees to a suggestion).
4. Checks its own work: reads back the Home slots and Projects, says what it couldn't check.

Pass if clean. Anything else goes on the later list (remy-later-list.md).
