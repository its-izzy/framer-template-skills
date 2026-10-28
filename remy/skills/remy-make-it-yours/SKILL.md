---
name: remy-make-it-yours
description: "Replace Remy's sample designer with the owner: name, logo, location, clock, contact details, social links, portrait, About, blog byline, search titles and site settings."
---

Replace the sample designer, Remy Varga, with the owner everywhere except the Work and Blog collections, whose sample entries are replaced with remy-add-case-study and remy-add-blog-post.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch; if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work in the project's preview at 1200, 810, about 700 and 390 px wide and in dark mode. If you can't see it, say so in your report.

## 1. Ask in one message

One numbered list, each item with a short example; say anything they don't have yet can stay a placeholder:

1. Full name, for the footer, page titles, alt text and About (Remy Varga)
2. Logo text, usually the first name; the Accent full stop is added (Remy)
3. City, time zone, and a 12-hour or 24-hour clock (San Jose, Pacific time, 12-hour)
4. Email
5. Links for the networks they use: Instagram, LinkedIn, Dribbble, X
6. A one-line role (Independent Product and Brand Designer)
7. A portrait photo, at least 1200 px wide, and a short caption (Remy, at work)
8. When they're next free for new work (Booking from [month and year])
9. For About: a two- or three-sentence intro, their background, their approach, and their career as years and roles (2019–2023, Senior product designer, Pliant)
10. One or two sentences for the byline under every blog post (I'm Remy, a designer working across product, brand and systems.)
11. Keep /design-system as their private reference, hidden from search, or delete it before launch?

Wait for answers. Anything missing becomes a placeholder in capitals and square brackets, such as [YOUR EMAIL]. A link can't hold a placeholder: leave it as it is and list it.

## 2. Change

1. Wordmark: the logo text. Keep the Accent full stop.
2. Footer: the copyright line, © with the current year and the full name.
3. Nav: the city in the bar and in the phone menu ("Based in [City] ·", followed by the clock); the Local Time clock's Time Zone (an IANA name such as America/Vancouver) and Clock (12-hour or 24-hour); the phone menu's email (text and mailto link). Remove the Design system link from the bar and the phone menu.
4. Main layout: delete the floating Use template button (the Use template (floating) layer, which links to a placeholder remix link) on Desktop, Tablet and Phone.
5. Contact CTA: the email (text and mailto link) and each social link's address.
6. Contact Form: "Dear Remy," becomes the owner's first name. Set the form's Send To to the owner's email if your tools can, then read it back: if it's empty or unconfirmed, tell the owner to select the Contact Form and set or confirm Send To, or messages go nowhere.
7. /contact: the Detail rows Name, Email (value and mailto link), Based in, Availability and Elsewhere (each network's link), and both Polaroids' image, caption and alt text (one shows only on phones).
8. Home: the role line under the statement (the Subheading layer in Hero text, inside Hero and Work); change its words only, since the stack code finds it by name and times the prints from its fade. Write the role in Title Case, whatever case the owner typed it in ("[Full name], Independent Product Designer"), here and in the site title. Then, in About, the Polaroid's image, caption and alt text, the intro, and the Background, Approach and Career rows (years and roles, and the city on the current role).
9. /blog/:slug: in the Written by byline, the Polaroid's image and alt text, and the bio.
10. Portraits: with the owner's photo, put it in every Polaroid above with their caption and the alt text "Portrait of [Full name]". Without one, keep the sample photo but don't put the owner's name on someone else's face, which misleads visitors and screen reader users: set each caption and alt text to [YOUR PORTRAIT], and keep the caption they gave for the report.
11. Search titles: replace "Remy Varga" with the full name on /work, /blog, /contact and /404, and in the case study and blog post title patterns ("{{Title}} – [Full name]").
12. Site settings: site title ("[Full name] – [Role]", with the role as worded in the role line from step 8) and description (one sentence from their About intro, under about 155 characters), plus their own favicon and 1200 × 630 social image if they have them; the template's are Remy's.
13. Unused networks: turn off the visibility of each one in the Contact CTA and the Elsewhere row; don't delete them, so they can come back.
14. /design-system: delete it if the owner wants it gone; if they keep it, check it's hidden from search. Change nothing else on it: its samples are the template's documentation.

For anything your tools can't reach, give the owner the text and the steps.

## Rules

- Use only what the owner tells you; never invent facts, years or employers.
- Leave the Home hero statement and the services as they are; offer remy-design-system if the owner wants them rewritten.
- Leave the demo pages /test-3-projects and /test-5-projects alone; list them for the owner to delete before launch.
- Place the owner's words exactly as given. Don't add emphasis such as italics that they didn't ask for; suggest it instead.
- Write anything new in the voice from section 07 of /design-system, and reread it as remy-remove-ai-writing describes.

## Check before you report

The Framer connector can show a change as saved that never reached the project, for example after the project stops responding during an edit. So:

1. Open the project again in a new session and read back every change.
2. Take canvas screenshots of Home, /contact and a blog post at Desktop and Phone, in light and dark, and compare them with what you read back. If a screenshot still shows something you removed or old text, believe the screenshot: try that change once more, and if it still doesn't show, report it as not done, with the steps to do it by hand.
3. Ask the owner to check the same things after they publish: the browser tab titles on /work, /blog and /404, and that no Use template button shows. If you couldn't view a width (such as about 700 px), say so.

## Done when

- Searching the pages, components, layout templates, alt text, page titles and descriptions finds no "Remy", "Varga", "San Jose" or hello@remyvarga.com, and no "Pacific time" unless the owner is on Pacific time. /design-system, the User guide design page and the two demo pages are the template's own and may keep the name Remy.
- The logo, the Nav and the role line fit at every size; if a long name crowds the menu button, suggest a shorter logo text, such as the first name.
- No Design system link in the Nav, and no Use template button on any page, in the read-back and in the screenshots.
- The email links open the owner's address, and every visible social link opens their profile.

## Report

What you changed, page by page and component by component; anything that didn't stick, with the steps to do it by hand; every placeholder left, including the portrait and the caption to use with it; every link still pointing at a network's home page, hidden ones included; and what the owner still has to do: Send To, if it isn't set and confirmed; site settings your tools couldn't reach; the demo pages and the sample case studies and posts to replace.
