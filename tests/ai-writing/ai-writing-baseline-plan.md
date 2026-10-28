# remy-remove-ai-writing: 3 more baseline runs before any fix (6b, 6c, 6d)

Owner: the "Fix the AI writing skill" thread. Isaiah, Oct 28, 2026, about 11:22 a.m. Vancouver: "before drafting fixes. perform another 3 sets with 3 different sets of mock data that are different case." So these runs test the skill as it is now, with no fixes. The overnight test 6 (main 1db3522) found one problem: in Framer, the edit swapped the flagged words for vague stand-ins ("current tools", "many different clients") instead of asking or leaving placeholders, so it still sounded generic.

Queue: the PC and the Framer connector are shared, one thread at a time. Start only after the "Fix the blog post skill" thread says its round 2 (3f to 3i) is done and the PC is free; that round itself waits for the case study round 3 (2f to 2i). When 6d is done, tell the coordinator the PC is free.
Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template, following tests/round2/runner-instructions.md for how a run works. Where they differ, this plan wins, and the runner reports to the "Fix the AI writing skill" thread.

## Setup, every run

1. **Skills:** every folder in remy/skills from branch skills-update at commit 2bce691 or later (write the commit in the run notes), installed as local project skills in a clean folder: C:\Users\Izzy\claude\skills-test-runs\test-06b (06c, 06d). Check each folder doesn't exist first; never touch other threads' folders. Never upload anything. remy-remove-ai-writing on the branch is the same as test 6's except for its outside preamble; remy-base now says "never a vague stand-in", which test 6 didn't have.
2. **Fresh remix** of framer.link/ZU6lsXr for part C only, named "Remy skills test 6b – AI writing" (6c, 6d). Never touch, change settings on, or publish the main Remy project. Leave the remix's built-in skill copies as they are.
3. **Seed the mock copy** for part C (below) into the remix in the Framer editor, or with your own connector session that you close before the test session starts. Replace only the words; keep the text style. Then read the seeded text back and save it as seeded.md.
4. **Sessions:** parts A and B in one fresh session with **no Framer connector**; part C in a second fresh session with the Framer connector. Never name the skill. If the session asks something the run doesn't cover, answer briefly as the buyer would and log it.
5. Publish only the remix, to its framer.app address, after part C. Never publish a copy with real personal data.

## Runs (send each turn as written)

### 6b. Services, tight limits, owner says "just do it". Mira Castellanos, UX designer in Montréal.

Seed (part C): Home's four Service Card descriptions, in order:
1. "I leverage a holistic, human-centred approach to craft seamless, intuitive digital experiences that truly resonate with users and drive meaningful business outcomes across every touchpoint."
2. "Elevating brands through bold, impactful visual identities that tell your unique story."
3. "Components, tokens and guides that help teams build faster and stay consistent." (Remy's own text, left as it is: it already reads well)
4. "From concept to launch 🚀, I empower startups to unleash their full potential with cutting-edge, best-in-class design solutions!"

- **A** (no connector): "Before I change anything, can you flag what sounds robotic in two of my service blurbs? Just tell me, don't fix. 1) I leverage a holistic, human-centred approach to craft seamless, intuitive digital experiences that truly resonate with users and drive meaningful business outcomes across every touchpoint. 2) From concept to launch 🚀, I empower startups to unleash their full potential with cutting-edge, best-in-class design solutions!"
- **B**: "ok now fix them"
- **C** (connector on, new session): "my services section on the home page sounds super generic, can you make it sound more like a real person? [REMIX LINK]". If it asks for details: "idk just do it". If it asks a second time: "just do it".

Case: short fields with a 20-word limit, emoji and an exclamation mark, one service that's already fine, a buyer who won't give details, Canadian spelling ("centred") in the owner's own text.

### 6c. One case study, mostly human, with a client quote. Daniel Osei, product designer.

Seed (part C), in the Work item **Halden** (the owner names it, so it's in scope):
- Brief, keep Remy's text as it is (already human).
- What I did: "I embarked on a comprehensive deep dive into the onboarding flow, meticulously mapping every touchpoint. Moreover, I facilitated workshops to foster alignment and spearheaded a robust redesign. As the client put it: \"Daniel made the whole process feel seamless and genuinely collaborative.\""
- What changed: "The new onboarding is a testament to the power of user-centred design. Studies show that simpler onboarding increases retention, and the results speak for themselves. It's not just a better flow, it's a better business."

- **A** (no connector): "Audit only, please. This is the What I did section of a case study: I embarked on a comprehensive deep dive into the onboarding flow, meticulously mapping every touchpoint. Moreover, I facilitated workshops to foster alignment and spearheaded a robust redesign. As the client put it: \"Daniel made the whole process feel seamless and genuinely collaborative.\""
- **B**: "Thanks. Rewrite it, but keep it about the same length."
- **C** (connector on, new session): "Can you clean up the writing on my Halden case study? A couple of parts sound off to me. [REMIX LINK]". If it asks for facts: "We cut onboarding from 7 steps to 4. I don't have retention numbers."

Case: rich text CMS fields, a protected client quote that contains flagged words, a vague authority ("Studies show"), a contrast template, one field that's already fine, and a buyer who gives one real fact and says one isn't available.

### 6d. The whole site, a detailed owner, shared text. Priya Raman, brand designer in Vancouver.

Seed (part C):
- Home statement (inside Hero and Work; keep the green full stop): "Crafting bold, unforgettable brand experiences that truly resonate"
- Home About intro: "Certainly! Here's a polished About section: I'm a brand designer who thrives at the intersection of strategy and creativity. With a passion for storytelling, I help visionary brands navigate an ever-evolving landscape."
- /work lead under the page title: "A curated showcase of transformative projects that redefine what's possible."
- Contact CTA lead-in (shared component): "Ready to elevate your brand? Let's build something great together!"

- **A** (no connector): "Scan these lines from my site and tell me what's off. Don't rewrite yet. Home headline: Crafting bold, unforgettable brand experiences that truly resonate. About: Certainly! Here's a polished About section: I'm a brand designer who thrives at the intersection of strategy and creativity. With a passion for storytelling, I help visionary brands navigate an ever-evolving landscape. Contact: Ready to elevate your brand? Let's build something great together!"
- **B**: "Rewrite all three. Some facts you can use: I design packaging and identities for food and drink brands. I've been doing it for 8 years, mostly for small coffee roasters and breweries in BC."
- **C** (connector on, new session): "Go through my whole site and fix anything that sounds generic or AI written. Facts: I design packaging and identities for food and drink brands, 8 years, mostly small coffee roasters and breweries in BC. [REMIX LINK]". When it lists the passages: "Do them all, except leave the Contact CTA as it is."

Case: a site-wide request (more than five passages, so it should list and wait), a chatbot leftover, the Home statement's word limit, green full stop and typing time, a shared component the owner then excludes, sample content and /design-system that should be skipped, and an owner who gives real facts up front.

## Checks per run

Test 6 problem (the reason for these runs):
1. **No vague stand-ins in part C.** Where a fact is missing, it asks for two or three specifics first, or leaves [PLACEHOLDERS]. Fail on stand-ins such as "current tools", "many clients", "a range of", "various", "products", "digital experiences". List every phrase it used to fill a gap.
2. **Same handling in B and C:** the same missing fact gets the same treatment (ask or placeholder) in both.
3. **No added claims:** every sentence in the new copy traces back to the old copy or the owner's words (list each sentence and its source). Note small additions like "so that's where I start".
4. **Keeps Remy's patterns:** italic phrase, green full stop and sentence case stay where the template has them, or the report says why not.

Test 6 checks that passed (still checked):
5. Part A changes nothing, quotes each finding, groups P0, P1 and P2, never says the copy was written by AI.
6. Part A flags every planted pattern (write down any it missed) and the cluster words as a cluster.
7. Part B gives the final text once, then a short list of changes; first person, contractions, no dashes, exclamation marks or emoji.
8. Part C changes only the words in scope; styles, layout, other text and sample content untouched (read-back before and after of every text on the pages it touched).
9. Part C reports before and after for each change.
10. In Preview and live, changed text fits and fades in at 1440, 1200, 810, about 700, 390 and 360 px, light and dark, with reduced motion.

Run-specific:
- 6b: every service 20 words or fewer; service 3 left alone; emoji gone; "centred" kept as the owner's spelling or the change explained; after "just do it", placeholders, not stand-ins.
- 6c: the client quote is kept word for word and its flagged words are reported, not edited; Brief left alone; "Studies show" removed or questioned, not kept as a claim; "7 steps to 4" used, and no retention figure invented; edits the CMS item, never the card.
- 6d: lists all passages and waits before changing more than five; "Certainly! Here's a polished About section:" removed; statement 10 words or fewer with the green full stop kept, and the typing-time note if over about 40 characters; says the Contact CTA shows on every page, then leaves it alone as told; uses only the owner's facts; skips samples and /design-system.

Every run: picks the skill from plain words (note if not); reads only the downloaded skills, never the project's copies (no api.skills.read of a project skill); remy-base read first in part C; new-session read-back before reporting.

## Evidence per run

In the run folder, copied to C:\Users\Izzy\claude\remy-template\ai-writing-tests-oct-28\<run>: transcript-ab.md and transcript-c.md (every turn, tool calls, which skill files it read), seeded.md, readback-after.md (every text on the touched pages and items, with styles; mark what changed), final-report-c.md, run-notes.txt (commit, remix link, live address, anything off-script), and Playwright screenshots of each changed page at 1440, 1200, 810, 700, 390 and 360 px, light and dark, plus reduced motion. Message the AI writing thread after each run with a short summary and the paths. Don't grade or fix anything.

## After the 3 runs

The AI writing thread grades 6b to 6d with test 6, sends Isaiah one combined report and waits for his feedback before drafting any fix with skill-creator.
