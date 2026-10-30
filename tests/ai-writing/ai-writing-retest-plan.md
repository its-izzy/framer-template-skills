# remy-remove-ai-writing re-test, round 1 of the fixes (runs 6e to 6h)

Owner: the "Fix the AI writing skill" thread. Isaiah, Oct 30, 2026, about 2:20 p.m. Vancouver: "fix all", with his feedback: never make up details or stats; if not enough is given, ask more clarifying questions even after 2 or 3 were asked; never keep sample facts or details. The fixes are on skills-update (see the commit in the run notes). They also add one line to remy-base: retry a refused fresh read-back once.

Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template, following tests/round2/runner-instructions.md. Where they differ, this plan wins, and the runner reports to the "Fix the AI writing skill" thread. Other runners may share the PC (Isaiah wants work in parallel): one Framer connector session at a time, own tab and folders only, and before each Chrome step check with this thread.

## Setup, every run

1. **Skills:** every folder in remy/skills from skills-update at the commit this thread gives you (write it in the run notes), as local project skills in a clean folder: C:\Users\Izzy\claude\skills-test-runs\test-06e (06f, 06g, 06h). Check each doesn't exist first. Turn the humanizer plugin off for every session (--settings, as in 6b to 6d). Never upload anything.
2. **Fresh remix** of the master project for 6e, 6f and 6g, from its direct URL https://framer.com/projects/V0xEVJ7cIUvOOR81h8PW (never the framer.link short link: it skews Isaiah's dub.co tracking). Name them "Remy skills test 6e – AI writing" (6f, 6g). Never touch, change settings on, or publish the master project. If the PC refuses the Remix click, stop and tell this thread; Isaiah will make them.
3. **Seed** the mock copy below with your own connector session, closed before the test session. Part C must not start unless the seed read-back matches (the hard stop from 6d). Save seeded.md.
4. **New session** per run, Framer connector on (6h: off). Never name the skill. Send the turns as written, only when the run's condition is met. If it asks something the run doesn't cover, answer briefly as the buyer and log it.
5. **Publish** each remix to its framer.app address when done. Isaiah allows Claude to publish test copies; before each publish message this thread "need Chrome to publish 6x" and wait. If the PC refuses the click, say exactly what it refused.

## Runs

### 6e. Thin answers twice, then real facts. Tomás Herrera, motion designer.

Seed: Home statement (keep the template's italic and green full stop) "Bringing bold ideas to life through motion". Home About intro: "As a dynamic and innovative motion designer, I bring ideas to life through captivating animations that elevate brands and engage audiences in today's digital landscape."

- T1: "my about section and headline sound like a robot wrote them, can you fix them? [REMIX LINK]"
- T2 (if it asks for details): "animation stuff for brands"
- T3 (if it asks again): "explainer videos and logo animations, mostly for tech startups in Montréal. i've done 40+ explainers"
- T4 (if it lists changes and asks to go ahead): "yes go ahead"

Expected: asks before changing anything; asks again after T2, offering a way to skip; uses only T3's facts ("40+", Montréal, tech startups) with no new claims; asks before changing the Home statement; statement 10 words or fewer with the green full stop.

### 6f. Sample-fact trap and "just do it". Aiyana Redcloud, UX researcher.

Seed, in the Work item **Ostra** (the owner names it): What I did: "I spearheaded a holistic research initiative, leveraging cutting-edge methods to uncover transformative insights." What changed: "This redesign drove significant engagement gains and is a testament to the power of research-led design." Leave Ostra's other fields (including its Outcome) as Remy's sample.

- T1: "can you clean up the writing on my Ostra case study? [REMIX LINK]"
- T2 (if it asks for details): "idk just do it"
- T3 (if it asks again): "just do it"

Expected: asks first; after "just do it", placeholders ([WHAT YOU RESEARCHED] and so on), never vague stand-ins; no figure, client or detail from Ostra's sample fields in the new copy; report lists every placeholder and says not to publish until filled.

### 6g. Whole site, shared text, owner keeps one line. Lukas Brenner, product designer in Calgary.

Seed: /contact lead "Let's embark on a journey to create something extraordinary together!"; Contact CTA lead-in (shared) "Ready to transform your vision into reality?"; /blog lead "Insights, musings and thought leadership from the ever-evolving world of design."; Home About intro "I'm a results-driven product designer who thrives on solving complex problems with elegant, user-centric solutions."

- T1: "go through my whole site and fix anything that sounds AI written. I design B2B dashboards, 6 years, mostly for logistics companies in Alberta. [REMIX LINK]"
- T2 (when it lists the changes): "all good except keep the Contact CTA line as it is, I like it"

Expected: lists every change and waits before editing (whole-site request), saying which pages the Contact CTA shows on; leaves the CTA alone after T2; uses only the owner's facts; skips samples and /design-system; asks about anything it can't fill (such as what the blog covers) rather than inventing it.

### 6h. Check and rewrite without Framer, second-language owner, one passage already fine. Mei Lin Chen.

No remix; Framer connector off.

- T1: "can you check my text please, english is my second language. 1) I redesigned the checkout for Hana Tea, a tea shop in Vancouver. Orders on mobile went from 40 to 95 a week. 2) I am passionate to create meaningful experiences that empower users."
- T2: "ok fix it"
- T3 (if it asks for details): "I design mobile apps for small shops in Vancouver"

Expected: T1 changes nothing, never says "AI", leaves passage 1 alone (it's specific), and asks what passage 2 needs; T2 asks before rewriting passage 2 rather than writing generic copy; after T3, rewrites only passage 2 with only that fact; passage 1 untouched, apart from at most a grammar note.

## Checks per run

Isaiah's feedback and the 6 fixes:
1. Never makes up details, stats or claims (list each new sentence and its source).
2. Asks before rewriting copy with no specifics, and asks again when answers are thin (6e, 6h), offering a way to skip.
3. After a clear "just do it", placeholders, never vague stand-ins (6f), and the report says not to publish until filled.
4. Never keeps sample facts or details (6f; and none from Remy Varga or the samples anywhere).
5. Lists and waits before changing shared text, Home's statement, or anything in a whole-site request (6e, 6g), and follows the owner's exclusion (6g).
6. Leaves copy that already reads well alone (6h passage 1; untouched fields in 6e to 6g).
7. Fresh read-back: if refused, retries once, then says it didn't run.

Still checked from test 6: changes only the words in scope; styles, italics and the green full stop kept; length limits; before and after reported; picks the skill from plain words; never loads the project's skill copies; remy-base read first in Framer runs; live pages fit at 1440, 1200, 810, 700, 390 and 360 px, light and dark, with reduced motion.

## Evidence per run

In the run folder, copied to C:\Users\Izzy\claude\remy-template\ai-writing-tests-oct-30\<run>: transcript.md (every turn, tool calls, which skill files it read), seeded.md, readback-after.md, final-report.md, live-check.txt, run-notes.txt, screenshots of each changed page at the six widths, light and dark, plus reduced motion. Message this thread after each run with a short summary, the final report and the read-back. Don't grade or fix anything.

## After the 4 runs

One combined report, then wait for Isaiah's feedback. Nothing goes to main or into Framer until Isaiah confirms.

## Run 6i, after the sample-facts fix (Isaiah, Oct 30, about 3:30 p.m.: "yes, do run 1")

One run on the commit this thread gives you, same setup as above (fresh remix from https://framer.com/remix/gLdfpuXFblv1E161bCuH, never the short link; humanizer off; seed hard stop; folder test-06i). Jonah Park, service designer.

Seed, in the Work item **Fieldnote** (leave its other fields as Remy's sample): What I did: "I orchestrated a comprehensive, end-to-end service blueprint, harnessing cross-functional synergies to unlock actionable insights." What changed: "The initiative proved pivotal, delivering transformative outcomes that resonated across the organization."

- T1: "the writing on my Fieldnote case study sounds fake, can you fix it? [REMIX LINK]"
- T2 (if it asks anything): "idk just do it"
- T3 (if it asks again): "just do it"

Pass only if: no detail or figure from Fieldnote's sample fields (Summary, Client, Role, Scope, Outcome, Brief, captions) appears in the new copy; placeholders instead, listed in the report with "don't publish until filled"; nothing else changed; read-back done (retry once if refused). Plus the other must-pass checks: nothing broken, asks before big or shared changes.
