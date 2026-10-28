---
name: remy-launch-check
description: "Review the published or preview Remy site before launch without changing it: accessibility, SEO, links, forms, content, layouts and Remy's own setup. Reports blockers, fixes and passed checks."
---

Review the published or preview site before launch without changing anything, at every size and in light and dark mode.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch (if the owner's plan has them); if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work at the widths and modes remy-base lists, and follow its Before you report steps. If you can't see something, say so in your report.

## General checks

- **Accessibility:** headings, alt text, labels, contrast, focus states, touch targets, reduced motion.
- **SEO:** titles, descriptions, URLs, social images, indexing, redirects, missing or duplicate metadata.
- **Links and forms:** navigation, buttons, anchors, external links, validation, submission states.
- **Content and CMS:** spelling, placeholders, missing content, drafts, inconsistent naming, unclear calls to action.
- **Layouts:** overflow, overlaps, wrapping, image crops, spacing, hidden content, the phone menu.
- **Launch basics:** homepage, favicon, domain, HTTPS, analytics, policy links, obvious performance risks.

For one page in depth, use remy-seo-check or remy-accessibility-check.

## Remy checks

- No Remy Varga, hello@remyvarga.com or San Jose on any page or component, in alt text (every portrait, including the byline on /blog/:slug), in page titles and descriptions, or in the site title, description, favicon and social image. The sample case studies (Halden, Ostra, Fieldnote, Kiln Week, Tern), the six sample posts, the four sample services and the sample portrait are placeholders: any still on the site is a launch blocker.
- Availability on /contact shows a real month.
- The Contact Form's Send To is the owner's address; remind them to send a test message once the site is live.
- Every Work collection item has a Case summary, a Social image and a Next project, and the Next project chain loops. Every Blog collection item has a Summary, a Cover image and a Social image.
- Projects on Home's Hero and Work is 3, 4 or 5, and Home slots 1 up to it each hold exactly one project.
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
- **External links** open in a new tab and don't land on an error or a sign-in page.
- **404:** a made-up address shows the 404 page, and its links work.

## Report

Three lists: launch blockers, recommended fixes, and checks that passed. Give each issue its page, the problem and a suggested fix.
