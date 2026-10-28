# remy-add-blog-post re-test plan (queued after the case study re-tests)

Owner: the "Fix the blog post skill" thread (Oct 28, 2026). Start only after the "Fix the case study skill" thread says re-tests 2b to 2e are done; the PC and the Framer connector are shared, and the make it yours runs (1b to 1e) go first.

## Setup, every run

1. **Fresh remix** of framer.link/ZU6lsXr, named "Remy skills test 3b – blog post" (3c, 3d, 3e). Never touch, change settings on, or publish the main Remy project.
2. **Outside skills:** every remy skill from GitHub branch skills-update at commit 38e441e or later (pull right before the runs; write the commit in the run notes), installed as local files in the clean test profile. This includes the held remy-base. Never upload anything.
3. **Skill copies follow the tool (Isaiah, Oct 28, about 1:00 a.m.):** these runs test an external agent (Claude Code), so it uses only the external skill files from the branch and never the project's built-in copies. Don't paste anything into the remix. remy-base now tells outside agents to ignore the project's copies. Testing Framer's internal agent would be a separate run that pastes fixes/remy-add-blog-post-framer-held.md and fixes/remy-base-framer-held.md into the remix only.
4. **New Claude session** in the clean test profile; never name the skill. Free Unsplash photo links (public, direct image links) unless the run says otherwise.
5. Publish only that copy, to a free framer.website address (remy-skills-test-3b and so on). Before publishing, make one small real edit in the editor (change a value and back) to anything changed through the connector on a page or layout (a new Filter Tab on /blog, the /blog intro). Never publish a copy that ends up with real personal data, such as Isaiah's name from the Framer account.
6. **Evidence:** full transcript (which skill copies it read), a read-back of the new Blog item (every field, and the Body block by block: paragraph, Heading 2 or empty), and screenshots of /blog (All and the topic tab) and the post page at 1440, 1200, 810, about 700, 390 and 360 px, light and dark, and with reduced motion. Save to C:\Users\Izzy\claude\skills-test-runs\test-3b (and so on), and copy transcript and read-back to /mnt/project-files/skills-test-oct-23/runs/test-3b/ if reachable.

## Runs (play the buyer; send each turn as written, one at a time)

**3b. Ordinary buyer, thin notes (the main writing fix).** Kenji Watanabe, UX designer.
- T1: "Can you turn these notes into a blog post? Topic Process, dated today. I record every usability test, even the quick ones. I only watch the clips where someone hesitates. Hesitation tells me more than a wrong click. I keep a folder called pauses. Cover: https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?w=2400 [REMIX LINK]"
- Expected: one numbered list, nothing changed yet; its title and summary guesses; the date written out in the Nav clock's time zone (the remix's clock is still the sample's); two or three questions drawn from the notes.
- T2: "Title: Watch the pauses. Summary works. The cover is a laptop on a desk with a test session paused. To your questions: I started doing it after a test where nobody failed the task but everyone paused at the same field, and that field was the problem. Now I tag every pause with the screen name so I can see which screens pile up."
- Expected: body in joined paragraphs of two to four sentences, every sentence traceable to the notes or T2, nothing added; no subheads needed; spacing clean; live.

**3c. Messy buyer.** Valentina Ruiz-Ortega, graphic designer.
- T1: "ok so blog post!! its about café menus and what they taught me about hierarchy. topic process i guess, or maybe tools?? date it last friday. notes: menus have like 3 seconds to work. price is never the biggest thing. the café near my studio, Pájaro, uses one typeface in two weights and it works. I want these three things as a bullet list: 1 size, 2 weight, 3 space. a customer once told me 'I only read the bold bits' which honestly is the whole point. cover: https://unsplash.com/photos/a-menu-on-a-table-abc123 [REMIX LINK]"
- Expected: asks which topic (Process or a new Tools option), writes out last Friday's date for confirmation, says the cover link is a web page, not an image, and asks for a direct image link; says the Body isn't styled for lists and offers paragraphs instead; keeps the customer's words inside a paragraph (no quote block).
- T2: "process. the date is right. title: What café menus taught me about hierarchy and why I think about them every single day. ok paragraphs are fine. cover: https://images.unsplash.com/photo-1554118811-1e0d58224f24?w=2400 it shows a chalkboard menu above a counter"
- T3, only if it suggests a shorter title: "fine, use your shorter one".
- Expected: Slug works with the accent in café; no added facts about Pájaro; spacing clean; live.

**3d. Near-silent buyer.** Sam Ilunga.
- T1: "add a blog post [REMIX LINK]"
- T2 (to whatever it asks): "idk, something about design"
- T3: "just do it"
- Expected: asks once more for a few points, doesn't write a post from nothing, no owner details from the Framer account; then a draft item with placeholders in square brackets, kept as a draft (also no cover), with the steps to add a cover and switch it live; nothing shows on /blog.

**3e. Complete buyer, own text, new topic, publish request.** Amara Lindqvist, design researcher.
- T1: "Here's a finished post for my site. Title: Five interviews are enough to start. Summary: Why I stop at five interviews, and what I do with the sixth slot. Date: September 30, 2026. Topic: Research. Cover: https://images.unsplash.com/photo-1552664730-d307ca884978?w=2400 (a team around a table with sticky notes). Social image: https://images.unsplash.com/photo-1552664730-d307ca884978?w=1200&h=630&fit=crop. Then publish it please. [REMIX LINK]" plus a pasted post of about 400 words with four "## " subheads, Canadian spelling (colour, organise), one em dash and two typos ("teh", "recieve").
- Expected: asks before adding Research as a topic (and its Filter Tab), offers to update the /blog intro; keeps the owner's words, spelling and em dash, fixes only the typos, and suggests rather than makes other changes; "## " lines become Heading 2 with one empty paragraph before each; says it can't publish and the owner publishes; live.
- T2: "yes add Research, and yes update the intro."

## Checks per run (pass/fail)

First-run issues from test 3:
1. Body spacing: no empty paragraph at the start or end, none between paragraphs, exactly one before each Heading 2 (from the block-by-block read-back)
2. Writing: notes shaped into joined paragraphs, not one note per line; nothing added; two or three questions when the notes are thin (3b)
3. Date: written out in the first list and counted in the Nav clock's time zone, never Framer's or the session's own
4. No cover: item kept as a draft, with steps to add a cover and switch it live (3d; any run that ends without one)
5. New topic: asked first, Filter Tab set up like the others, /blog intro update offered (3c if picked, 3e)

New behaviour: sends the list and changes nothing in Framer before the first answer (no writes in turn 1, unless the owner gave everything); bad image link named with its field (3c); list request answered with paragraphs, owner's quote kept in a paragraph (3c); owner's own text and spelling kept (3e); no publishing (3e).

Standing checks: followed the held skill (the transcript shows which copy it read); remy-base loaded first; new item, not a rewritten sample; Summary one sentence under about 120 characters; cover alt text one plain sentence; Social image is the owner's 1200 × 630 image or the cover; only paragraphs and Heading 2 in the Body; samples counted and deleting them offered; Written by byline mentioned; /blog shows it first under All and under its topic tab (live runs); post page reads well at every width, light and dark, reduced motion, and More notes shows other posts; new-session read-back and screenshots before reporting; owner details only from the owner.

## After the 4 runs

One combined report for the blog post skill (a Claude Doc, separate from the other skills' reports): what it did well, what it did poorly, how to improve it for a template buyer, and pass/fail on every first-run issue in every run. Then wait for Isaiah's feedback before changing the skill again.

## Appendix: the post Amara pastes in 3e (send it in T1, after the line "Then publish it please.")

```
Most teams I work with want to book twelve interviews before they'll trust what they hear. I understand the instinct. But by the fifth conversation I'm usually hearing teh same three problems in slightly different words, and the next seven rarely change the plan.

## Why five

Five is not a magic number. It's the point where my notes stop surprising me. I write every new problem on its own sticky note, and I colour the ones I've heard before. Somewhere around the fourth or fifth interview the board goes mostly yellow.

That doesn't mean the research is finished. It means I know enough to make something rough and put it in front of people, which teaches me more than another hour of questions would.

## What I do with the sixth slot

I still book a sixth interview, but I don't use it for questions. I bring the rough version and watch someone use it. People find it hard to describe a problem in the abstract — they find it easy to point at a screen and say "that's wrong".

The sixth slot is also where I recieve the most honest feedback. By then I've stopped defending my first idea, and the participant can tell.

## How I organise the notes

Every sticky note gets a short label and the number of the interview it came from. After five interviews I photograph the board, sort the notes into groups, and write one sentence per group. Those sentences become the brief.

I keep the photos. When someone asks why we built something a certain way, I can show them the board from the week we decided.

## When five isn't enough

If the five people disagree with each other, I keep going. Disagreement usually means I'm talking to two different groups, and each group needs its own five. I'd rather find that out early than average two kinds of people into one who doesn't exist.

Five interviews won't answer everything. They answer enough to stop guessing and start making, and that's the part I care about most.
```
