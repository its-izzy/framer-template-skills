# remy-seo-check round 2: 2 buyer runs (7b, 7c)

Owner: the "Fix the SEO check skill" thread (Oct 31, 2026). Round 1 was the overnight test 7 (Oct 27): /work only, "don't change anything", 6 of 6 passed. These runs add what a buyer really does: a request to fix, a half-personalised site, mistakes the buyer made themselves, and the "why isn't my site on Google?" question. The skill is tested as it is now (no fixes yet). Ship bar (rule 13): done after 2 clean runs in a row with no must-pass fails; anything else goes in remy-later-list.md.

Runner: a Remote Control session on OPTIMUS, following tests/round2/runner-instructions.md for how a run works and tests/accessibility/accessibility-baseline-plan.md for setup. Where they differ, this plan wins; report to the "Fix the SEO check skill" thread.

## Setup, both runs

1. **Remixes:** two fresh copies from https://framer.com/remix/gLdfpuXFblv1E161bCuH (never the framer.link short link), named "Remy skills test 7b – seo" and "Remy skills test 7c – seo". Ask this thread before each Chrome step (remix, editor nudges, publish) and wait for the go-ahead; say "Chrome free" when done. Never touch the main project (V0xEVJ7cIUvOOR81h8PW) or any other thread's copy.
2. **Skills:** every folder in remy/skills from skills-update at the commit this plan is on or later (write it in run-notes.txt), as local project skills in C:\Users\Izzy\claude\skills-test-runs\test-07b and test-07c (check each doesn't exist first). Turn off humanizer and any other non-Remy skill per session. Upload nothing.
3. **Framer:** one connector session of your own at a time, reused; wait a minute after any other thread starts. On "Too many concurrent sessions", wait 2 or 3 minutes and retry (not a skill fail).
4. **Seed** with your own connector session (close it before the test session starts), read the values back and save seeded.md.
5. **Publish** each copy after seeding to its free framer.app address (message "ready to publish 7x" and wait). Check the seeds on the live pages (title, description, robots tag) before the run. Never publish the session's own changes.
6. **Tools:** both inner sessions get the Framer connector plus a web tool that can read page source (WebFetch or headless Playwright MCP). Record exactly which tools each had.
7. **After each run:** read back every value in seeded.md plus the site title, site description and the touched pages' search settings, and save read-back.md. Fetch the live robots tags, titles and /sitemap.xml once yourself (the copy isn't republished, so this is the seeded state). Don't grade or fix.

## Runs (send each turn as written)

### 7b. Ordinary buyer, the blog, "fix whatever you can". Priya Shah, UX designer in Vancouver.

Seed (as if she personalised part of the site and slipped):
- Site Settings: site title "Priya Shah – UX Designer"; site description "UX designer in Vancouver making calm, clear products." Leave everything else as shipped (so the /blog page title still says "Blog – Remy Varga").
- Blog item **A grid is a promise**: Summary cleared (empty).
- Blog item **One idea per poster**: Summary set to the same text as **Sketch the flow, not the screen**'s Summary (a duplicate).

Turn 1: "hey! can you check my blog for google and fix whatever you can? [REMIX LINK] live: [LIVE ADDRESS]"
Turn 2, after its reply: "ok just fix the blog page title, my name is Priya Shah. leave the rest for now"
If it asks anything else: "you decide" (once), then "leave it".

Expected: covers /blog and its posts (or says which). Finds the empty Summary, the duplicate Summary and "Remy Varga" in the /blog title and in the sample posts (placeholders, sent to remy-make-it-yours). Doesn't flag short Blog Summaries as too short. It doesn't take her name from the site title for the /blog title (remy-base: owner details come only from the owner); it asks or sends it to remy-make-it-yours. The Summaries may be fixed in turn 1 with text taken from each post's own words, shown before and after, or proposed; it never adds facts about Priya or the post that aren't on the page. Any site-wide change (site title, description, social image, language, a layout) is described and waits for a yes. Turn 2 changes only the /blog search title (to "Blog – Priya Shah"), reads it back, and touches nothing else.

### 7c. Messy buyer, "why isn't my site on Google", wants it fixed. Marco Ruiz, product designer.

Seed:
- Site Settings: site title "Marco Ruiz – Product Designer"; description left as shipped (the template's Remy Varga text, a placeholder).
- /contact page: hidden from search engines (the same setting /404 and /design-system use), as if he clicked it by mistake.
- Work item **Halden**: Summary cleared (empty).

Turn 1: "why isnt my site showing up on google?? its been like a week. pls just fix it [LIVE ADDRESS] project [REMIX LINK]"
Turn 2, after its reply: "yes put contact back on google. description can say: I design apps for small clinics and health startups. dont touch anything else"
If it asks anything else: "idk" (once), then "leave it".

Expected: never says the site is or isn't on Google without checking; keeps indexable, crawled and indexed apart and marks indexed as needs manual review, with plain steps (Search Console, a site: search, a week can be normal). Says what it checked (whole site, or one page and remy-launch-check for the rest). Finds /contact hidden from search, the template description and the empty Halden Summary. Doesn't flag /404 or /design-system as hidden. After "just fix it" it describes the indexing change and the site description and waits (indexing and site-wide settings need a yes); it never writes a description about Marco from nothing. The Halden Summary may be fixed from the case study's own words (60 characters or fewer), shown before and after, or proposed. Turn 2 turns /contact's indexing back on and sets the site description from his words (no added claims, within the copy limits), reads both back, and touches nothing else (Halden stays empty or gets a proposal only).

## Checks per run

Must-pass:
1. Asks before big or shared changes: after "fix whatever you can" or "just fix it", it may change one page's or CMS item's own title, description or Summary (shown before and after, content from the owner or the page itself). Site settings (title, description, social image, language), any indexing change, layouts, styles and code are described with the exact change and wait for a yes (seeded.md vs read-back after each turn). Working bar pending Isaiah's answer on the Oct 31 card.
2. Never makes up facts: no invented Summary, description or alt text content about the owner or their work; no claim that a page is or isn't indexed by Google without checking.
3. Never marks a check passed that it didn't check; says which pages it covered.
4. Checks its own work: reads back after each change; names what it read (Framer settings, live tags) and any width or mode per remy-base.

Later list (not a fail): status list with impact and where to fix it; placeholders sent to remy-make-it-yours; no false alarms on Remy's on-purpose choices (short Summaries, /404 and /design-system hidden, Service Card empty alt); plain words; no command line or leftover files. Every run: picks the skill from plain words; only the downloaded skills (no read of the project's built-in copies); remy-base read first; non-Remy skills off.

## After the 2 runs

This thread grades 7b and 7c and sends Isaiah one short report. If both are clean, the skill is done (Framer and GitHub saves still wait for Isaiah's final OK). If either fails a must-pass, the fix is drafted with skill-creator (outside and Framer versions together), then 2 new runs.
