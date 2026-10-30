# remy-add-blog-post re-test round 2 (runs 3f to 3i)

Owner: the "Fix the blog post skill" thread. Isaiah chose "Make all six, then re-test" (Oct 28, about 9:30 a.m. Vancouver). Queued after the case study round 3 (2f to 2i); start only when that thread says the PC is free. Runner rules: tests/round2/runner-instructions.md, reporting to the "Fix the blog post skill" thread. Copies publish to framer.app ("Get free domain" is blocked on the PC). Keep connector sessions few: close yours before each test session opens.

## Setup, every run

1. **Fresh remix** of the master Remy project (https://framer.com/projects/V0xEVJ7cIUvOOR81h8PW; never the framer.link short link, Isaiah Oct 30), named "Remy skills test 3f – blog post" (3g, 3h, 3i). Never touch, change settings on, or publish the main Remy project.
2. **Outside skills:** every remy skill from GitHub branch skills-update at commit f9140e2 or later (pull right before the runs; write the commit in the run notes), installed as local files in the clean test profile. This includes the held remy-base. Never upload anything.
3. **Skill copies follow the tool (Isaiah, Oct 28):** these runs test an outside agent (Claude Code), which must use only the downloaded skill files and never the project's built-in copies. As in make it yours round 2, leave the remix's old built-in skills in place for 3f and 3h (the real-world mismatch), and for 3g and 3i paste tests/blog-post/default-framer-build.md into the remix's "default" skill and tests/blog-post/remy-add-blog-post-framer-build.md into its remy-add-blog-post skill (remix only, never main). Wait about 3 minutes, then read them back fresh to confirm. A run passes only if the session doesn't load the project's skill copies (no api.skills.read of a project skill) and follows the downloaded files.
4. **New Claude session** in the clean test profile; never name the skill. Free Unsplash photo links (public, direct image links) unless the run says otherwise. Before each run, open each image link given below; if one doesn't load or plainly doesn't match the buyer's description, swap in a free Unsplash photo that does, and log it.
5. Publish only that copy, to a free framer.website address (remy-skills-test-3f and so on). Make round 2 found that publishing puts page and component changes live; only the Main layout stayed stale, and these runs shouldn't touch it. After publishing, check /blog live; if a change made in the run is missing, make one small real edit in the editor (change a value and back) and publish again. Never publish a copy that ends up with real personal data, such as Isaiah's name from the Framer account.
6. **Evidence:** full transcript (which skill copies it read), a read-back of the new Blog item (every field, and the Body block by block: paragraph, Heading 2 or empty), and screenshots of /blog (All and the topic tab) and the post page at 1440, 1200, 810, about 700, 390 and 360 px, light and dark, and with reduced motion. Save to C:\Users\Izzy\claude\skills-test-runs\test-03f-blog (test-03g-blog, test-03h-blog, test-03i-blog). Check a folder doesn't exist before creating it, and never touch any other test folder (other threads'). The PC can't reach /mnt/project-files, so report paths and paste the read-backs and final reports to the "Fix the blog post skill" thread.

## Runs (new buyers; send each turn as written)

**3f. Thin notes, buyer skips the questions.** Noor Haddad, illustrator.
- T1: "blog post please, topic Craft, dated today. I ink everything with a brush pen. Mistakes stay in. Clients notice the wobble. Cover: https://images.unsplash.com/photo-1513364776144-60967b0f800f?w=2400 [REMIX LINK]"
- T2: "Title: Keep the wobble. Summary is fine. Cover shows paint brushes and ink on a table. Skip the extra questions."
- Expected: no empty first paragraph on the FIRST save (check the transcript); one or two full paragraphs, no one-sentence string, no added framing; live.

**3g. Very long title, new topic, messy.** Bartholomew Ng, brand designer.
- T1: "new post!! title: Everything I learned from redesigning the same coffee bag label eleven times over two very long years. topic: Packaging (new one i think). date: oct 1. notes: the client changed the roast name 3 times. we tested on a real shelf each round. version 7 was almost the final one. the final one is the simplest. cover https://images.unsplash.com/photo-1559056199-641a0ac8b55e?w=2400 [REMIX LINK]"
- T2: "yes add Packaging and update whatever needs it. use your shorter title. cover is coffee bags on a shelf."
- Expected: suggests a shorter title in the first list (title is 98 characters); asks before adding Packaging; adds the tab, and offers to update both the /blog intro and /blog's search description; date written out (October 1, 2026); no blank paragraphs; live.

**3h. Silent buyer.** Ines Duarte.
- T1: "write a blog post for my site [REMIX LINK]"
- T2: "dunno"
- T3: "just do it"
- Expected: no invented post; a draft with [YOUR TITLE] and Slug draft-post, telling the owner to change the Slug when they add a title; nothing on /blog.

**3i. Finished post with subheads, no cover, publish request.** Theo Marchetti-Lund, product designer.
- T1: "Here's my post, please add it and publish. Title: Name the states first. Summary: Why I list every state a screen can be in before I draw it. Date: today. Topic: Process. No cover yet." plus the post below.
- T2 (if asked about the cover again): "no cover, go ahead"
- Expected: keeps his text and spelling; four subheads with one empty paragraph before each and none at the start (first save); kept as a draft for no cover with steps to add it; says it can't publish.

```
Every screen has more states than the one in the mock-up. Empty, loading, error, partial, full. If I don't name them first, I design the happy one and forget the rest.

## Start with a list

Before I open a design tool I write down every state the screen can be in. It's usually more than I expect. A simple list page had nine.

## Draw the ugly ones first

I draw the empty and error states before the full one. They're the ones people see when something has gone wrong, so they deserve the most care.

## Share the list, not the screens

Engineers like the list more than the mock-ups. It tells them what to build and what to test.

## When the list gets long

A long list usually means the screen is doing too much. That's worth knowing before anyone draws anything.
```

## Checks per run

Round 1 fixes still hold (ask first, date written out in the Nav clock zone, nothing invented, draft without a cover, new topic asked first, owner's text kept, no publishing, only downloaded skills, no account details), plus the six round 2 fixes:
1. No empty paragraph on the first save (transcript), and the read-back is still done
2. Shorter title suggested above about 60 characters, owner's kept unless they agree (3g)
3. New topic: /blog search description offered with the intro (3g)
4. Short posts: no one-sentence paragraph string, no added framing (3f)
5. Placeholder draft Slug draft-post, owner told to change it (3h)
6. Widths: screenshots all three breakpoints (1200, 810, 390) in light and dark, names what it saw, and puts 1440, about 700, 360 and reduced motion on the owner's click-through list (new base rule, f9140e2)

Then one combined report for round 2 and wait for Isaiah's feedback.
