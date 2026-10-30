# remy-add-blog-post re-test round 3 (runs 3j to 3m)

Owner: the "Fix the blog post skill" thread. Isaiah said "make them" (Oct 30, about 12:26 p.m. Vancouver) to the three round 2 report fixes, now on skills-update 0f1d68b. Runner rules: tests/round2/runner-instructions.md, reporting to the "Fix the blog post skill" thread. Isaiah wants work in parallel (Oct 30): the case study and AI writing runners may be on the PC at the same time, so use only your own Chrome tab and folders, never touch another thread's remixes or test folders, run one test session at a time, and wait a few minutes (not a retry loop) if Framer says "Too many concurrent sessions". Copies publish to framer.app ("Get free domain" is blocked on the PC).

## Setup, every run

1. **Fresh remix** of framer.link/ZU6lsXr, named "Remy skills test 3j – blog post" (3k, 3l, 3m). Never touch, change settings on, or publish the main Remy project. Make the remixes in one go and close your Chrome tab after, so other runners can use Chrome.
2. **Outside skills:** every remy skill from GitHub branch skills-update at commit 0f1d68b or later (pull right before the runs; write the commit in the run notes), installed as local files in the clean test profile. Never upload anything.
3. **Skill copies follow the tool:** leave the remix's built-in skills as they are for 3j and 3l. For 3k and 3m, paste tests/blog-post/default-framer-build.md into the remix's "default" skill and tests/blog-post/remy-add-blog-post-framer-build.md into its remy-add-blog-post skill (remix only, never main). Wait about 3 minutes, then read them back fresh to confirm. A run passes only if the session doesn't load the project's skill copies and follows the downloaded files.
4. **New Claude session** in the clean test profile; never name the skill. Before each run, open each image link below; if one doesn't load or plainly doesn't match the buyer's description, swap in a free Unsplash photo that does, and log it.
5. **Safety:** confirm from the session's open_project reply that it opened the test remix. Publish only that copy. After publishing, check /blog live; if a change made in the run is missing, make one small real edit in the editor (change a value and back) and publish again. Never publish a copy that ends up with real personal data, such as Isaiah's name from the Framer account.
6. **Evidence:** full transcript (which skill copies it read, and every Body write exactly as sent), a read-back of the new Blog item from a fresh read-only session (every field, and the Body block by block: paragraph, Heading 2 or empty, plus any font, colour or style set on the blocks or runs, and the same for one sample post to compare), **canvas screenshots** of the new post's page in the Framer editor in light and dark (works for drafts too; this is the check for the system-font problem), and live screenshots of /blog (All and the topic tab) and the post page at 1440, 1200, 810, about 700, 390 and 360 px, light and dark, and with reduced motion. Save to C:\Users\Izzy\claude\skills-test-runs\test-03j-blog (test-03k-blog, test-03l-blog, test-03m-blog). Check a folder doesn't exist before creating it. Report paths and paste the read-backs and final reports to the "Fix the blog post skill" thread.

## Runs (new buyers; send each turn as written)

**3j. Ordinary buyer, everything given but "today".** Priya Raman, service designer.
- T1: "Please add this as a blog post. Title: Map the handoffs. Summary: Why I draw every handoff before I draw a single screen. Date: today. Topic: Systems. Cover: https://images.unsplash.com/photo-1531403009284-440f080d1e12?w=2400 (sticky notes on a wall in rows). Notes: most problems I find happen between teams, not inside one. I draw a box for each team and an arrow for each handoff. The arrows with no owner are where things get lost. Last project had 14 arrows and 3 had no owner. [REMIX LINK]"
- T2 (to the date question): "yes that's right"
- T3, only if it asks anything else: answer briefly as Priya, and log it.
- Expected: changes nothing in turn 1 and sends back today's date written out (Nav clock time zone) to confirm, even though everything else is given (fix 2); then a body in joined paragraphs, nothing added; Body written block by block with no empty paragraph at the start on the first save (fix 1); canvas shows the post in the template's fonts, light and dark; live.

**3k. Messy buyer, asks Claude to write the Summary.** Mateo Esposito-Kahn, motion designer.
- T1: "hey can u put up a post. title 'Ease out, always' i think? you write the summary. date: yesterday lol. topic craft. notes: i used to animate everything with linear timing. a senior on my team told me to try ease-out. now i use it for almost everything that enters the screen. things that leave get ease-in. i still dont know why exactly it feels better, it just does. cover https://images.unsplash.com/photo-1550745165-9bc0b252726f?w=2400 its an old monitor with colours [REMIX LINK]"
- T2: "title is fine. date yes. summary ok"
- Expected: date written out for confirmation (yesterday in the Nav clock time zone); a Summary that says only what the notes say, with no promised lessons, tips, rules or "why" (Mateo says he doesn't know why), under about 120 characters (fix 3); the body doesn't explain why ease-out feels better; flags the cover if it shows another brand; Body block by block, clean first save; canvas fonts right; live.

**3l. Near-silent buyer, then a placeholder draft.** Jo Okafor.
- T1: "need a blog post up [REMIX LINK]"
- T2: "about my process i guess"
- T3: "just make it, i'll fill it in"
- Expected: asks once more for a few points, doesn't write a post from nothing, no owner details from the Framer account; a draft with [YOUR TITLE], Slug draft-post, [YOUR SUMMARY] and [YOUR POST], the owner told to change the Slug when they add a title; the placeholder Body has no empty paragraph before it, and on the canvas it shows in the template's font, not a system font (light and dark); nothing shows on /blog.

**3m. Complete buyer, own long post, a title that clashes with a sample.** Hana Sato, design lead.
- T1: "Here's a finished post, all details below, please add it. Title: Sentences catch what sketches hide. Summary: Why I start a design review by reading the brief out loud. Date: October 14, 2026. Topic: Process. Cover: https://images.unsplash.com/photo-1517048676732-d65bc937f952?w=2400 (people around a table in a meeting). [REMIX LINK]" plus the post below.
- T2, only if asked about the title or Slug: "oh, keep my title but give it a different link"
- Expected: notices the title (and Slug) clash with a sample post's subhead or title only if they really clash, and keeps the Slug unique; builds straight away is fine, since the date is written out; keeps Hana's words, spelling (colour, programme) and em dash, fixes only "seperate" and "thier"; five subheads with exactly one empty paragraph before each and none at the start or end on the first save; canvas fonts right for both paragraphs and subheads, light and dark; live.

Before the run, read /blog and the six sample posts (read only) and note whether "Sentences catch what sketches hide" is already a sample title, subhead or Slug, so the check knows what a clash is.

```
I start every design review the same way: someone reads the brief out loud before anyone looks at a screen. It feels slow the first time. By the third review nobody wants to skip it.

## Why out loud

Reading silently lets everyone skim to the part they care about. Reading out loud makes the room hear the whole thing, including the sentence nobody agreed with. That sentence is usually the reason the review exists.

## What it catches

Most of the problems we find in the first ten minutes aren't visual. They're two goals that pull in seperate directions, or a user the brief never mentions. A sketch can hide those for weeks — a sentence can't.

## Who reads

Never the designer. When someone else reads thier brief, the designer hears where the words don't match what they meant. Half the time they fix the brief before we get to the screens.

## The colour question

People always ask whether this works for visual work, like colour or type. It does, but differently. The brief says what the colour has to do, and the review checks the screens against that, not against anyone's taste.

## When we skip it

We skip it when the brief hasn't changed since the last review. Otherwise it stays in the programme, even for small things.
```

## Checks per run

Round 1 and round 2 fixes still hold (ask first, date written out in the Nav clock zone, nothing invented, draft without a cover, owner's text kept, no publishing, placeholder Slug draft-post, widths checked or listed for the owner, only downloaded skills, no account details), plus the three round 3 fixes:
1. Body written block by block into the empty first paragraph: no empty paragraph at the start on the first save (transcript), no Body sent as one string, read-back still done, and the canvas shows the template's fonts in light and dark (all runs)
2. A relative date ("today", "yesterday") is sent back written out before anything is saved, even when everything else is given (3j, 3k)
3. The Summary says only what the notes or post say (3k; and any run where Claude writes the Summary)

Then one combined report for round 3 and wait for Isaiah's feedback.
