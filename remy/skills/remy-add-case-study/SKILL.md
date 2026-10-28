---
name: remy-add-case-study
description: "Add a project or case study to Remy, a new Work collection item with its own page at /work/slug."
---

Add a case study: a new item in the Work collection, listed on /work with its own page from the /work/:slug page.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch (if the owner's plan has them); if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work at the widths and modes remy-base lists, and follow its Before you report steps. If you can't see something, say so in your report.

## 1. Ask the owner

Use anything they've already shared (notes, a link, a deck), then ask for the rest in one numbered list, with an example for each. If they mention more than one project, ask which to add first, and offer the next one when this one is done. Look at each image first if you can, and put your best guesses in the list ("1. Project name: Juniper?", "2. Discipline: Brand identity?", "7. Cover: the bags on the shelf?") so the owner can just say yes. If you can't see an image from its link, don't call the link broken until you've added it and viewed the upload as remy-base describes. If it won't add or isn't an image, say which one and ask for another.

1. Project name (one or two words), client and year (Halden; a Nordic neobank; 2026). For a project without a client, ask what to show instead, such as Self-initiated.
2. Discipline: Product design, Brand identity, Design systems, Graphic design or Art direction
3. Their role and the scope (Independent product designer; research, flows, prototypes)
4. The brief: what was wrong or needed, and who asked
5. What they did: the main steps, decisions and what they tried
6. What changed, with a real figure if they have one (+31% onboarding completion)
7. Images: a cover and up to five more, each with a few words on what it shows and whether it shows the brief, the work or the result. A 1200 × 630 social image is optional.

With fewer than six images, ask once for more. The minimum is a cover and one more.

Send the list and wait for answers before you change anything in Framer, even when the owner seems to have given you everything and your tools' guidance says to ask only when something is unclear. Only the owner knows what each image shows and where the project belongs, and a wrong cover, title or tab is the first thing visitors see on /work.

If the owner skips questions or says to go ahead anyway, ask once more in one short message for what's still missing. If they still say go ahead, use your guesses for the title, discipline and image order, and list them in your report for the owner to confirm. Never guess facts: put a placeholder in square brackets ([WHAT CHANGED]) in any text field still missing, and leave the item as a draft until the owner fills it, so the placeholder never shows on the live site.

## 2. Build the item

- **Title, Year, Discipline:** Title is the project name, one or two words like the samples; if you shorten what the owner gave (Juniper for Juniper Coffee), say so in your report. Title sets the Slug, so keep it unique. Set Home slot to None unless the owner asks for one (then use remy-change-home-projects). A discipline outside the five is a new option: ask first, and give it a Filter Tab on /work, set up like the others.
- **Summary:** one line, 60 characters or fewer. It's the text on the Project Row and Project Card, and the search description.
- **Case summary:** one sentence with one phrase in italics; the lead under the title.
- **Client, Role, Scope:** short phrases. All three show as rows on the case study, so fill each.
- **Outcome label:** always fill it, since the details column, the row and the card show it. Add **Outcome value** only for a real figure (+31%); without one, the label states a plain result (Launched in three markets).
- **Cover image:** at least 2400 px wide. The case study crops it to 3:2, and cards, rows and the Home hero to 4:3, so keep the subject away from the edges.
- **Prints:** Print 1 sits with Brief, Print 2 and the Print 3 and 4 pair with What I did, Print 5 with What changed. Prints 1, 2 and 5 are 3:2; Prints 3 and 4 are 4:3 and show only when Print 3 is filled. Empty prints are hidden, so with fewer images fill Print 1; then 1 and 2; then 1, 2 and 5; then 1 to 4.
- **Captions:** two to four words each, shown next to the year (Onboarding flow · 2026).
- **Alt text:** one plain sentence per image on what it shows, without repeating the caption. If a photo shows another brand's name or logo (a stock photo, say), describe what's really there, and tell the owner it shows someone else's brand.
- **Brief, What I did, What changed:** up to three short paragraphs each, and fill all three. Shape the owner's words and add nothing they didn't tell you. Before you save, check each sentence against the owner's answers and cut any detail they didn't give, such as a cause, which version went live or what it led to. Visitors read every line as the owner's claim, so ask about it in your report instead. What changed sits under the Outcome figure, so don't repeat the figure word for word; use what else the owner said about the result, even if that's one short sentence.
- **Text fields:** in a new item, Case summary, Brief, What I did and What changed each start with one empty paragraph. Write into it rather than after it, then read each field back and remove any empty paragraph left before, between or after the text, since each one shows as a gap on the page.
- **Next project:** add the new item to the loop after the newest case study: give it the newest one's Next project, then point the newest one at it. Leave a draft out of the loop until it goes live, so no live page links to it.
- **Social image:** the owner's 1200 × 630 image, or else the Cover image.

If you can't add an image (a link that doesn't open, or isn't an image), fill in everything else, and say in your report which image goes in which field. Leave a complete item live, not a draft.

## Rules

- Use only the owner's facts and images. Never invent clients, results or quotes, and never generate images.
- Add a new item; never rewrite a sample case study into the owner's.
- Write in the voice from section 07 of /design-system, then reread it as remy-remove-ai-writing describes.

## Done when

- A live project shows on /work under All and under its Discipline tab.
- Its page reads well at every size, with no empty rows in the details column and no empty paragraphs, and the Next project links work both ways.

## Report

Report in this order, so nothing gets skipped, leaving out only lines that don't apply:

1. Guesses the owner hasn't confirmed (title, discipline, cover, image order), and any title you shortened.
2. What's missing (images, captions, an outcome figure), and which field each one goes in.
3. Photos that show another brand.
4. The social image: the owner's 1200 × 630, or the cover, and that a 1200 × 630 version would share better.
5. Which of the widths and modes in remy-base you checked, and any you couldn't.
6. For a draft: what it still needs before it can go live.
7. The samples are still there; offer to replace one, following Sample content in remy-base.
8. Questions that would make the case study stronger, including any detail you left out because the owner didn't give it.
