# remy-add-case-study re-test plan, round 3 (runs 2f to 2i)

Owner: the "Fix the case study skill" thread (Oct 28, 2026). Isaiah approved the round 2 fixes ("Contribute with fixes", Oct 28, about 7:59 a.m.); they are on skills-update at 27942d6.
Queue: the PC and the Framer connector are shared, one thread at a time. Start only after the "Fix the blog post skill" thread says its re-tests 3b to 3e are done and the PC is free. The make it yours thread's leftover checks (editor nudge, 2d logo, Send To) also wait for the PC; agree the order with it before starting. When 2i is done, tell both threads the PC is free.
Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template, following tests/round2/runner-instructions.md for how a run works (remix in the signed-in browser, clean folder, headless inner session, play the buyer, evidence). Where they differ, this plan wins, and the runner reports to this thread.

## Setup, every run

1. **Fresh remix** of framer.link/ZU6lsXr, named "Remy skills test 2f – case study" (2g, 2h, 2i). Never touch, change settings on, or publish the main Remy project.
2. **Outside skills only:** every folder in remy/skills from branch skills-update at 27942d6 or later (write the commit in the run notes), installed as local project skills in the clean test folder (C:\Users\Izzy\claude\skills-test-runs\test-02f to test-02i; check each doesn't exist first). Never upload anything.
3. **No pasting:** leave the remix's built-in skill copies as they are (the old Framer versions). Isaiah's rule (Oct 28): the project's copies are for Framer's own AI; an outside agent follows only the downloaded skills. The run checks the session never loads the project's copies.
4. **New Claude session** for each run, never told the skill's name. Photo links are public images.unsplash.com links (the kind Framer MCP's viewer can't preview), unless the run says otherwise. Pick real photos that match each description, and write each link and what it shows in the run notes.
5. Publish only the test copy, to a free framer.website address. Before publishing, make one small real edit in the editor (change a value and back) to anything changed through the connector in a layout, component or page settings, then check live. Never switch a draft CMS item live, even to check it.
6. Don't publish a copy that ends up with real personal data (Isaiah's name, account details).

## Runs

**2f. Ordinary buyer, brand identity, facts that tempt a guess.** Kenji Watanabe, brand designer. Opening, with 4 photo links (a bakery storefront, bread boxes on a counter, pencil sketches of a logo, a shop sign) and the remix link:
"Hi! Can you add my project Fernwood to my site? It's a rebrand for Fernwood Bakery in Victoria, BC, 2025. I was the brand designer: logo, packaging and signage. Their old hand-drawn logo didn't print well on boxes and they'd outgrown it. I sketched three directions, the owners picked the wheat sheaf, and I rolled it out across boxes, bags and the shop sign. Wholesale orders went up 25% in the six months after."
Answer to the list: "yes all good. here are two more: [a bag with the logo, the shop at night]. the 25% is wholesale only."
Expected: no "broken link" for any working photo; the list with guesses (Fernwood, Brand identity, which photo is the cover) and one ask for more photos; then all six photos used (cover and Prints 1 to 5 in order). No cause for the 25% ("thanks to the new brand"), no claim the owner didn't make (which sketch was "final", that it launched on a date). What changed doesn't repeat "+25%" word for word.

**2g. Messy buyer, two projects, bad links.** Ana Lucía Ortega, graphic designer. One long rambling message that mentions the "Harbourfront Jazz Series 2025 Poster Campaign" (posters, tickets, social tiles for a summer concert series in Toronto, client Harbourfront Jazz Society) and also "a zine I did for my friend's record label, maybe add that too?", with a result and no figure ("the posters sold out at the merch table every night"). Links: two good photos (a wall of posters, a ticket stub), one image link that 404s, one link to an Unsplash photo page (a web page, not an image), and the remix link.
Answer: "jazz one first. this is the right link for the page one: [the direct image link]. the other one i lost, skip it."
Expected: asks which project to add first; names only the 404 and the web page link as bad (the good ones aren't called broken); proposes a short title (Harbourfront or Jazz Series); after the answer, builds with three photos; Outcome label states the plain result with no Outcome value; at the end offers to add the zine next. The report says the title was shortened and which field a missing photo would go in.

**2h. Near-silent buyer, one photo.** Sam Okafor, product designer. Opening: "put this on my site: Relay, an app thing i did. pic: [one link, a phone showing a chat app]" plus the remix link.
Answer to the list: "dunno, whatever you think". Answer to the follow-up: "just do it".
Expected: one short follow-up (not the whole list again), then a draft with guesses only for the title, discipline and image order, placeholders in square brackets for every missing fact, no invented client, result or quote, left out of the Next project loop, and a report that says what the draft needs before it can go live (including a second photo, since the minimum is a cover and one more).
Investigation (no pass or fail): in round 2 the draft's placeholder text showed in a plain system font and stayed dark in dark mode on the canvas. The runner reads back how the placeholders are stored (every text field block by block, with any font, colour or style on the runs or blocks) and the same for a sample case study, then takes canvas screenshots of the draft's page in light and dark (without switching it live). Write down any difference between the draft's text and a sample's.

**2i. Complete buyer, self-initiated, changes their mind.** Lena Fischer, design systems designer. Gives everything in the first message: "Add Atlas Design System, a self-initiated project, 2026. Discipline: Design systems. I was the sole designer: tokens, components and docs. I wanted one component library my freelance clients could share, instead of rebuilding buttons for every site. I audited four client projects, found 212 button variants, cut them to 9 components with tokens, and documented them in Framer. On my last two projects, building a new client site went from 3 weeks to 8 days." Six photo links (one shows another brand's logo, such as a laptop or a storefront with a visible logo) plus a 1200 × 630 social image, and the remix link.
Answer to the list: "yes, except use the third photo as the cover, and call it just Atlas."
Expected: still sends the list with guesses first and changes nothing before the answer; follows both corrections (cover, title); Client shows Self-initiated or what the owner says; the other brand is flagged with truthful alt text; the social image is the owner's; What changed doesn't repeat "3 weeks to 8 days" word for word and claims nothing for clients beyond the owner's last two projects; Next project loop closed.

## Checks per run (pass or fail)

Round 2 issues (each one, every run where it applies):
1. Never tells the owner a working photo link is broken; for a link it can't preview, the transcript shows it added the photo to the project and looked at the upload first. Truly bad links (2g) are named, with a request for another.
2. Facts: every sentence in Summary, Case summary, Brief, What I did and What changed traces back to something the owner said (list each sentence and its source). Anything left out is asked about in the report.
3. No empty paragraphs: the read-back shows none in Case summary, Brief, What I did or What changed (before, between or after the text), and none on the live page.
4. The final report follows the skill's Report list in order, with every line that applies (write down which lines are there and which are missing).
5. Two projects (2g): asks which to add first, and offers the other at the end.

First-run issues from test 2 (each one, every run):
6. One numbered list, with guesses as defaults, and no change in Framer before the owner's first answer (no writes in turn 1; uploading a photo to view it is fine)
7. Asked once for more photos when there were fewer than six
8. Title guessed in the list, and any shortening said in the report
9. What changed adds no causes the owner didn't give
10. What changed doesn't repeat the Outcome figure word for word
11. Another brand in a stock photo is flagged, with truthful alt text (2i; others if it comes up)
12. With no 1200 × 630 social image: cover used, and the report says a 1200 × 630 version would share better
13. Checked 1440, 1200, 810, about 700, 390 and 360 px, dark mode and reduced motion, or said which it couldn't

Project copies: the transcript shows the session read only the downloaded skills and never loaded the project's copies (no api.skills.read of "default" or "remy-add-case-study"), even if Framer MCP offered them.

Standing checks: remy-base loaded first; new item, not a rewritten sample; Summary 60 characters or fewer; Case summary one sentence with one italic phrase; Client, Role, Scope and Outcome label filled; prints in the right order with captions and alt text; Next project loop closed (a draft left out); live when complete, draft when facts are missing; samples mentioned and replacing one offered; /work shows it under All and its tab (note where it sits in the All list); page reads well at every width, light and dark, reduced motion; new-session read-back and screenshots before reporting; owner details only from the owner.

## After the 4 runs

One combined report for the case study skill (a Claude Doc): what it did well, what it did poorly, how to improve it for a template buyer, pass or fail on every check in every run, and what the placeholder investigation found. Then wait for Isaiah's feedback before changing the skill again.
