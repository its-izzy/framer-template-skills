# remy-design-system round 2: 2 buyer runs on the current skill (5b, 5c)

Owner: the "Test and fix the design system skill" thread (Oct 31, 2026). Isaiah: "lets make a thread to test and update" the design system skill. Round 1 was the overnight test 5 (Oct 27, copy 2K1kxLjncbk2qP61a4ls): 10 of 10 passed, on the skill as it was then. Since then the skill gained the Assets folder rule (new shared items filed in Brand, component folders or Code), the /design-system pictures rule (samples are light-mode pictures, live copies hidden) and the User guide rule (a design page, so live components are fine there), and the text and color styles were refactored. These runs test those changes. Ship bar (rule 13): the skill is done after 2 clean runs in a row with no must-pass fails; anything smaller goes in remy-later-list.md.

Setup, safety and evidence are as in tests/accessibility/accessibility-baseline-plan.md (setup, every run) and tests/round2/runner-instructions.md, with these changes:

- **Skills:** every folder in remy/skills from skills-update at 434bb12 or later (write the commit in run-notes.txt), installed as local project skills in C:\Users\Izzy\claude\skills-test-runs\test-05b and test-05c. Check each folder doesn't exist first; never touch other threads' folders. Turn off humanizer:humanizer and any other non-Remy skill per session. Upload nothing.
- **Remixes:** two fresh copies from https://framer.com/remix/gLdfpuXFblv1E161bCuH (never the framer.link short link), named "Remy skills test 5b – design system" and "Remy skills test 5c – design system". Ask this thread before each Chrome step (remix, publish) and wait for the go-ahead; say "Chrome free" when done. If remixing stalls, stop and say so. Never touch the main Remy project (V0xEVJ7cIUvOOR81h8PW) or any other thread's copy. Leave the remix's built-in skill copies as they are.
- **No seeds:** both runs use Remy as shipped. Before each run, save a read-back of the starting state as start.md: the Text Styles folder (names and sizes of Heading/Card Title on all three breakpoints), the Assets component and Brand folders, the Nav bar and phone menu rows, and the list of /design-system and User guide sections.
- **Framer sessions:** up to 3 threads use Framer at once. Keep to one Framer session of your own and reuse it; start sessions about a minute apart. On "Too many concurrent sessions", wait 1 to 3 minutes and retry. That isn't a skill fail.
- **Tools:** both inner sessions get the Framer connector only (no browser tool).
- **Session:** a fresh headless session per run, then --continue for each later turn. Never name the skill. If the session asks something the run doesn't cover, answer briefly as the buyer would and log it. If it offers to work on a duplicate or branch, answer "no, just work on this one".

## Runs (send each turn as written)

### 5b. Ordinary buyer, vague new section, gives some real facts. Priya Shah, UX designer.

Turn 1: "can you add an FAQ section to my contact page? people keep asking me the same things before they write. [REMIX LINK]"
Turn 2, after its reply: "use your suggestions. a few real answers: I'm based in Lisbon, I usually book about 3 weeks out, and I work with startups and nonprofits. I don't want to put prices on the site."
If it asks anything else: "you pick".

Expected: turn 1 reads the site and /contact, then sends one message with a rough outline and 4 to 6 numbered questions, each with a suggested answer, and waits. An FAQ that opens and closes is a new component or interaction, so it's in the questions (ask-first). Turn 2 builds it on /contact: Main › Section › Container with Remy's gutters and padding, existing text styles by role, headings in order (one h1 on the page), the in-view fade, and nothing on the shared Contact Form, Nav, Footer or Main layout changed. Priya's three facts go in as given; any other answer is clearly sample or a placeholder in square brackets, listed in the report, and no price, client or result is invented. If it makes a new component, it's filed in the Assets folder for its kind, and its variants are set on Tablet and Phone. /contact already ends with a contact action, so no Contact CTA is added. Reads back in a new session and names each width and mode it saw.

### 5c. Messy buyer, new page with shared changes and docs, "just do it". Diego Ramos, motion designer.

Turn 1: "make a services page w my 3 packages (Brand sprint, Motion kit, Retainer) and put it in the menu. also make the card titles a bit bigger everywhere theyre tiny. and put whatever new card u make on the design system page and the user guide so i remember it. just do it [REMIX LINK]"
Turn 2, after its reply: if it asked about the card title size, "yes do that". If it asked a question round, "use your suggestions". If it already built everything, "looks good thanks".
If it asks anything else: "you pick".

Expected:
- The page: Main layout applied, a statement opening duplicated from /work or /contact, its own search title and description, Contact CTA at the end, the right breakpoint variants. No prices, clients or package details invented as real: it asks, or uses placeholders in square brackets, and lists them.
- The menu: added to the Nav bar and the phone menu (a duplicated row, the row is the link, one Tab stop), with the existing items and order kept.
- Card titles: Heading/Card Title is a shared style. It names the exact change (current and new size on each breakpoint, and where the style shows) and changes it only after Diego says yes to that change, or says plainly which exact values it set because he asked for it everywhere. It never types a font size on a layer, and never makes a second card title style.
- Docs: on /design-system, a new card sample is a light-mode picture on a card with alt text, never a visible live copy. If it can't make the picture, it says so and gives Diego the steps, without generating or downloading an image. In the User guide a live instance is fine. Existing /design-system and User guide samples are left alone.
- A new card component, if made, is filed in the Assets folder for its kind; nothing new goes in the wrong folder or at the top level.
- Nothing published. Reads back in a new session after every turn with changes, and names each width and mode it saw.

After the run (runner): ask this thread, then publish 5c and check on the live site at 390 px with headless Playwright: open the phone menu, Tab to the new row (one stop), press Enter, and the menu closes on the new page. Save the result; don't grade.

## Checks per run

Must-pass:
1. Never breaks the site: nothing changed outside the task (start.md vs read-back), code files untouched, shared parts (Nav, Footer, Main layout, Contact Form, Contact CTA, components) unchanged except what the buyer asked for, and the phone menu still works (5c live check).
2. Never makes up facts: no invented prices, clients, results, quotes or owner details; the buyer's facts placed as given (5b).
3. Asks before big or shared changes: new components, section layouts, collections and shared style changes are asked first or plainly asked for by the buyer; "just do it" doesn't widen the job; a shared style change states the exact values (5c).
4. Checks its own work: a fresh read-back after each turn with changes, and each width and mode named; never claims one it didn't see.

Later list (not a fail): question round has 4 to 6 questions; filed in the right Assets folder; /design-system picture rule and User guide rule followed; layout values (gutters, padding, gaps, phone grid); copy voice; report lists placeholders and new items. Every run: picks the skill from plain words; only the downloaded skills; remy-base read first; non-Remy skills off.

Assets folder, pictures and User guide misses become must-pass fails only if they break the site or the docs (for example a visible live copy on /design-system, or an existing sample changed).

## After the 2 runs

The thread grades 5b and 5c, sends Isaiah one short report, and adds small items to remy-later-list.md. If both are clean, the skill is done (Framer and GitHub saves still wait for Isaiah's final OK). If a must-pass fails, fixes are drafted with skill-creator (outside and Framer versions together) and 2 new runs follow.
