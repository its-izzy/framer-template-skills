---
name: remy-launch-check
description: "Review a Remy site before launch without changing it: content, links, SEO, accessibility and Remy's setup. Use when the owner says they're ready to launch or wants the whole site checked."
---

Review the published or preview site before launch without changing anything, at every size and in light and dark mode.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch (if the owner's plan has them); if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work at the widths and modes remy-base lists, and follow its Before you report steps. If you can't see something, say so in your report.

## How to check

- The live site can lag the project: Framer's canvas and Preview hold the latest edits. Say which one you checked. If the owner wants the live site checked and has edited since publishing, ask them to publish first.
- Report only what you read or saw. If you couldn't read a setting (favicon, domain, analytics, Send To) or try something (clicks, keys, sizes), mark it not checked and give the owner steps; never guess it passed.
- If the owner asks you to fix what you found, this skill still changes nothing: name the skill that does each fix (remy-make-it-yours for sample details, remy-change-home-projects for Home, remy-add-case-study or remy-add-blog-post for items, remy-design-system for shared parts) and wait for them to ask for it. Those skills ask for the owner's details and check their work.

## General checks

- **Accessibility:** headings, alt text, labels, contrast, focus states, touch targets, reduced motion.
- **SEO:** titles, descriptions, URLs, social images, indexing, redirects, missing or duplicate metadata.
- **Links and forms:** navigation, buttons, anchors, external links, validation, submission states.
- **Content and CMS:** spelling, placeholders, missing content, drafts, inconsistent naming, unclear calls to action.
- **Layouts:** overflow, overlaps, wrapping, image crops, spacing, hidden content, the phone menu.
- **Launch basics:** homepage, favicon, domain, HTTPS, analytics, policy links, obvious performance risks.

For one page in depth, use remy-seo-check or remy-accessibility-check.

## Remy checks

- No Remy Varga, San Jose or the sample email (hello@example.com) on any page or component, in alt text (every portrait, including the byline on /blog/:slug), in page titles and descriptions, or in the site title, description, favicon and social image. The sample case studies (Halden, Ostra, Fieldnote, Kiln Week, Tern), the six sample posts, the four sample services and the sample portrait are placeholders: any still on the site is a launch blocker.
- Home's Service Cards show the owner's services, in their words, with their own illustrations; the four sample services or their illustrations still there are a launch blocker (remy-make-it-yours for the words, remy-design-system for the illustrations).
- The categories are the owner's: the Blog Topic options and /blog's Filter Tabs (Process, Systems, Craft), and the Work Discipline options and /work's Filter Tabs (Product design, Brand identity, Design systems, Graphic design, Art direction). If they're still the template's set, ask the owner whether they fit their work; until they say yes, it's a launch blocker (remy-design-system). Each Filter Tab matches an option, and none leads to an empty list.
- Any placeholder in square brackets, such as [YOUR CITY], [CLIENT], [CAPTION] or [VALUE], on a page, in a CMS item, in alt text or in page settings is a launch blocker: other Remy skills leave them where a fact is missing.
- Availability on /contact shows a real month.
- The Contact Form's Send To is the owner's address; remind them to send a test message once the site is live.
- Every live Work collection item has a Case summary, a Social image and a Next project, and the Next project chain loops through the live items. A draft stays out of the loop until it goes live; that's not a blocker. An item is a draft only when its draft flag is on; a hidden (visible: false) item isn't a draft. Every Blog collection item has a Summary, a Cover image and a Social image.
- Projects on Home's Hero and Work is 3, 4 or 5, and Home slots 1 up to it each hold exactly one live project. A draft in a slot leaves Home short on the live site: a launch blocker.
- /design-system (kept as the owner's private reference) is hidden from search engines or a draft page, and /404 is hidden from search engines.
- Every page has one Main frame (the main landmark) around its sections, with the Nav and Footer outside it.

## Remy link check

Open or inspect every link at each size, including the phone menu. For each problem, report the page, where the link sits, where it goes now and where it should go.

- **Demo-only parts:** the Nav's Design system link (bar and phone menu) and the floating Use template button (Main layout, a placeholder remix link) are gone. Any left is a launch blocker.
- **Social links:** the Contact CTA on every page and the Elsewhere row on /contact ship pointing at each network's home page (www.instagram.com, www.linkedin.com, www.dribbble.com, www.x.com). Any still there is a launch blocker: it should open the owner's profile, or the network should be hidden.
- **Email:** every email link uses mailto: with the owner's address, the same in the Contact CTA, the Contact details and the Nav's phone menu. Phone numbers, if added, use tel:.
- **Nav and footer:** Work, Services, About, Blog and Contact open the right page or section (Services and About scroll to them on Home); the Wordmark goes to Home; the Footer's Back to top returns to the very top of every page, with nothing under the Nav.
- **CMS links:** hero prints, project rows and project cards open the matching case study; Next project opens the next one; Post Cards and More notes open the matching post; All projects and All notes go back to /work and /blog.
- **Filters:** each Filter Tab on /work and /blog shows only its items, and All shows everything.
- **Phone menu keys:** on the published site at phone width, open the menu and try Enter on a link, Esc, Tab out past the last link and Shift+Tab back past the menu button. Each should close the menu. Passed only if you tried every one and all worked; one that fails is a recommended fix, and one you couldn't try is not checked, with the steps.
- **External links** open in a new tab and don't land on an error or a sign-in page.
- **404:** a made-up address shows the 404 page, and its links work.

## Report

Four lists: launch blockers, recommended fixes, checks that passed, and not checked (with the owner's steps). Give each issue its page, the problem and a suggested fix. Say whether you checked the live site or the project, and name each width and mode you saw.
