---
name: remy-remove-ai-writing
description: Find and fix AI-sounding copy in Remy: rewrite it, check it without changing anything, or edit it in place, keeping the owner's facts, voice and length limits.
---

Edit Remy copy that sounds generic, repetitive or machine-written, so it reads like the owner wrote it: plain, specific and calm. Keep its meaning, facts and personality, inside the template's length limits. Adapted from Avoid AI Writing by Conor Bronsdon (MIT License, see Credit at the end).

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch; if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work in the project's preview at 1200, 810, about 700 and 390 px wide and in dark mode. If you can't see it, say so in your report.

- Rewrite and Detect work without a connection; Edit in Framer needs Framer MCP. Without it, ask the owner to paste the copy and say where each piece lives (page, component, or CMS item and field). Return only the sentences you changed, each with where it goes, so they replace just those words in Framer. You can't see the layout, so keep strictly to the length limits.
- To Detect across the site, read the published or preview site with your web tools, then find where each passage lives in Framer before you edit it.

## Modes

- **Rewrite** (default): find the AI patterns, fix them, and return the final text once.
- **Detect**: when the owner says "check", "scan", "flag" or "audit only", list what you found and change nothing.
- **Edit in Framer**: when the owner points at a page, a component, a CMS item or a selected layer, change the copy in place. Replace only the words that change, so bold, italics, links and subheads survive, and leave every passage that already reads as human.

If the owner hasn't pasted copy or said where it is, and nothing is selected, ask: one page, one component, one CMS item or the whole site.

## Before you start

- Read section 07, Voice and tone, on /design-system. Where it differs from this skill, section 07 wins.
- Skip these unless the owner names them: the sample case studies in the Work collection, the sample posts in the Blog collection and the sample designer's details (they're replaced before launch), and /design-system and the User guide (the template's own docs, which quote bad examples on purpose).

## Where Remy's copy lives

- **Pages:** the openings and section text on Home, /work, /contact, /blog and /404. Home's statement and the role line under it are inside Hero and work.
- **Shared component text** shows on every page that uses the component: the lead-in and "Write to me." in Contact CTA, the copyright line in Footer, the city line in Nav and the letter greeting in Contact Form. Before changing it, tell the owner which pages it appears on.
- **Instance text** belongs to one instance; change the property there: a Section Header title or note, a Service Card, a Label Row or Detail row, a Polaroid caption, a Field label, placeholder or error message, a Button or Arrow Link label.
- **CMS text:** Project Row, Project Card and Post Card show collection text, so edit the CMS item, never the card. Work: Summary, Case summary, Client, Role, Scope, Outcome label, Brief, What I did, What changed and the print captions. Blog: Title, Summary and Body.
- **Search text:** each page's search title and description are in its page settings. /work/:slug and /blog/:slug take theirs from each item's Title and Summary, so a new Summary is also the search description.

## Ground rules

- These patterns are signals, not proof; people write this way too, especially in a hurry or in a second language. Never tell the owner their copy "was written by AI".
- **Stay true to the source.** Every fact, number, name, client, date and result must come from the copy or the owner. Never invent one to make a sentence more concrete; if a fix needs a detail you don't have, leave the sentence and ask.
- **Protect what isn't yours to reword:** quotations, testimonials, client and project names, legal text, prices, URLs, slugs, CMS field names, the Discipline and Topic options and the Filter Tab labels that match them, and code. Report a pattern inside them instead of editing it. A Choice Chip label is also the answer the form sends, so ask before rewording one.
- **Prose and labels differ.** The rhythm rules (sentence length, groups of three, paragraph length, bare noun phrases) apply to prose: leads, the About intro, Brief, What I did, What changed, summaries and post bodies. Labels, buttons, nav links, field labels, chips, captions and rows such as Client, Role and Scope only follow the length limits and the word lists; short noun phrases are right there.
- **Edit only the words,** never layout, styles, components, colors, spacing or motion.
- Keep the owner's voice. If a paragraph is already clear and natural, leave it alone. Text that quotes a bad example on purpose (in docs or a post about writing) is exempt.

## Voice and length limits (section 07 wins)

- First person singular, plain, specific and calm; let the work carry the claim. Sentence case for headings and buttons.
- Mix short and long sentences, about 8 to 18 words on average. Don't open every sentence with "I". Use contractions (I'm, I'll, it's).
- No em dashes, exclamation marks or emoji. No "passionate about", "seamless", "elevate" or "stunning". The only question allowed is the short lead-in above the Contact CTA ("Have an idea in mind?").
- Keep every rewrite inside these limits, so it can't break the layout:
    - Home statement: 10 words or fewer, ending in the Accent full stop. Replace only the words, so the full stop keeps its color.
    - Section Header title: 1 to 3 words, no full stop. A Large title has one word in italics; a Compact title has none.
    - Lead under a page title: one or two sentences.
    - Work Summary: one line, 60 characters or fewer (the row and card text and the case study's search description).
    - Case summary: one sentence with one phrase in italics.
    - Blog Summary: one sentence, under about 120 characters (card, under the title and search results).
    - Service: one sentence, 20 words or fewer.
    - Outcome: a real figure or a plain fact the owner gave you.
    - Link or button: 1 to 3 words, verb first.
    - Missing detail: a placeholder in capitals and square brackets, such as [CLIENT].
- Copy with italics (page statements such as "Notes from *the studio*.", Large Section Header titles, Case summary) keeps the italic on one word or phrase. If the italic word goes, put the italic on the new key word.

## What to fix first

**P0, fix always**

- Chatbot leftovers: "Great question!", "I hope this helps", "As of my last update", "Certainly!", "Here's a…" intros.
- Placeholders and leaks: [INSERT NAME], "Lorem ipsum", citation marks such as 【1】, tracking parameters such as utm_source=chatgpt.com in links.
- Vague authorities: "experts say", "studies show", "industry leaders agree", with no source.
- Inflated importance for ordinary work: "a pivotal moment", "a testament to", "redefining the industry".

**P1, fix before publishing**

- Words from the lists below.
- Formula openers: "In today's fast-paced world", "In an ever-evolving landscape", "Let's dive in", "When it comes to".
- Contrast templates: "It's not just X, it's Y", "This isn't about X. It's about Y." Say the positive claim directly.
- Performed candor and hype: "Let's be honest", "Here's the thing", "the best part?", "game-changer", "hits different".
- Stacked hedges: "could potentially", "may eventually", "it's important to note that". Keep a hedge that carries real uncertainty.
- Empty intensifiers: "genuinely", "truly", "real" (a real difference), "actually" when it only adds emphasis.
- Bold sprinkled through a paragraph, emoji in headings, lists of bare noun phrases with no verbs in prose.
- The same idea said three ways, or synonyms swapped in to avoid repeating a word.
- Copy that breaks a length limit above.

**P2, fix when there's time**

- Habitual groups of three, when there aren't really three things.
- Every paragraph the same length; several sentences in a row that start the same way.
- "Serves as", "features", "boasts" instead of "is" or "has".
- Transitions such as "Moreover", "Furthermore", "Additionally".
- Generic closers: "The future looks bright", "Only time will tell", "Let's build something great together".
- Staccato drama: short fragments stacked for effect. Punchy. Like. This.

## Words to replace

**Always review** (swap for the plain word unless it's the right word in context): delve, landscape (as a metaphor), tapestry, realm, paradigm, embark, beacon, testament to, robust, comprehensive, cutting-edge, leverage (use), pivotal, underscore, meticulous, seamless, game-changer, nestled, vibrant, thriving, showcase, deep dive, unpack, intricate, ever-evolving, holistic, actionable, impactful, learnings, best practices, at its core, synergy, interplay, embrace (adopt), utilize (use), in order to (to), due to the fact that (because), commence (start).

**Fix when two or more meet in one paragraph** (one alone is fine): harness, navigate, foster, elevate, unleash, streamline, empower, bolster, spearhead, resonate, revolutionize, facilitate, nuanced, crucial, multifaceted, ecosystem, myriad, plethora, encompass, reimagine, cultivate, transformative, cornerstone, paramount, poised, overarching.

**Fix only when one word repeats a lot** (three or more times in a short piece): significant, innovative, effective, dynamic, compelling, exceptional, remarkable, sophisticated, world-class.

## Never add

A rewrite fails if it adds any of these, even when the result looks clean:

- Experience or opinions the owner never stated ("In my experience", "I've seen this a hundred times").
- Numbers, clients, tools, results or dates that aren't in the source.
- Manufactured stakes ("now more than ever"), invented foils ("everyone says X, but…"), performed honesty ("let's be honest").
- Em dashes, or sentences chopped into fragments to fake rhythm.

## How to work

1. Read the whole passage and the page or section it sits in. Note who it's for and how the owner already sounds.
2. List the P0 and P1 findings, then P2 if there's time. Check each against the ground rules and the limits before treating it as a problem.
3. Rewrite only what a finding justifies, in one pass. Reread; make a second pass only if something still clearly needs it. Two passes at most.
4. Compare with the original: same facts, claims and certainty, nothing invented, every limit kept.
5. In Edit in Framer, if you'd change more than five passages, first list them (where, before and after) and wait for the owner's OK. Five or fewer can go ahead.
6. Check each changed page at every size, so new line lengths don't break the layout.
7. If you changed Home's statement: it types at about 20 characters a second and the role line fades in at 2.4 s, so a statement over about 40 characters is still typing when the role line and the prints appear. Then tell the owner the role line's appear effect needs a later start.

## Report

- **Rewrite**: the final text once, then a short list of what changed and anything left alone on purpose (protected text, a detail you need from the owner).
- **Detect**: findings grouped P0, P1 and P2, each quoted with where it lives, noting which are clear problems and which are judgment calls.
- **Edit in Framer**: where you changed copy (page, component or CMS item, and the layer or field), before and after, which changed text shows on other pages, and anything still open.
- If nothing needs fixing, say the copy is clean and change nothing.

## Credit

Adapted from Avoid AI Writing (github.com/conorbronsdon/avoid-ai-writing), Copyright (c) 2026 Conor Bronsdon, used under the MIT License:

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
