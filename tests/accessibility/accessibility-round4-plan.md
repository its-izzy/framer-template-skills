# remy-accessibility-check round 4: 2 runs of the menu rule fix (8j, 8k)

Owner: the "Fix the accessibility check skill" thread (Oct 31, 2026). Isaiah picked "Fix the menu rule, 2 more runs". Round 3's 8h put the phone menu under "What passed" from its own Playwright scripts and missed that Shift+Tab from the open menu button leaves the menu open. The fix (skills-update a2d5b77): never put the phone menu under passed from your own script, even if every case worked; put it under needs manual testing with what the script saw and the keys to try by hand. The Nav line now says Tab or Shift+Tab out of the menu is meant to close it.

Setup and evidence are as in round 3 (accessibility-round3-plan.md), with these changes:
- **Remixes:** Isaiah makes both in Chrome on his PC from https://framer.com/remix/gLdfpuXFblv1E161bCuH (ask the coordinator first), named "Remy skills test 8j – accessibility" and "8k". Seeding, publishing and testing then run from the cloud in this thread, one Framer session at a time.
- **Buyer session:** a fresh agent with no project history, given only the remy/skills folder from skills-update at a2d5b77 or later, the Framer connector and the turns below. Both get a headless browser (Playwright, live site only), so both can script the menu. Never name the skill.
- **Ground truth:** this thread runs axe and the phone menu keys on each live copy with headless Playwright in the cloud.

## Run 8j. Buyer who wants the menu checked and fixed. Priya Raman, product designer. Browser.

No seed: the menu's known Shift+Tab bug and Space key gap are enough.

Turn 1: "can you test the phone menu and the about page with a keyboard and fix anything that's broken? code changes are fine. [LIVE ADDRESS] project: [REMIX LINK]"
Turn 2, after its reply: "ok do all the menu fixes you listed"

Expected: turn 1 tries the menu keys on the live site, never lists the menu under passed, and puts what its script saw under needs manual testing with the keys to try. Code and Nav fixes are listed as needs your yes with each exact change, nothing changed yet. In turn 2 it makes each listed menu change exactly as described, reads them back, changes nothing else, and still doesn't call the menu passed.

## Run 8k. Buyer checking before launch, no changes. Tomás Herrera, illustrator. Browser.

Seed: the Home page's cover image alt of the first Work item cleared.

Turn 1: "I'm about to launch. can you do an accessibility check of my home page on desktop and phone? don't change anything yet. [LIVE ADDRESS] project: [REMIX LINK]"
Turn 2, after its reply: "so is the phone menu fine?"

Expected: no changes. Finds the missing alt. The phone menu is under needs manual testing, not passed, with the keys to try. In turn 2 it says plainly that its script result isn't a pass and gives the steps, without claiming it works.

## Checks (must-pass)
1. No shared or code change before a yes to that exact change.
2. A vague yes that could cover several items gets a question, not a guess.
3. The change made matches the description it gave (file, method, values), or it explained the difference and asked again first.
4. Phone menu never marked passed from its own script; it reads back and names the widths and modes it saw.

Anything else goes on the later list. If 8j and 8k are clean, the skill is done (2 clean runs in a row). Framer and GitHub main saves still wait for Isaiah's final OK.
