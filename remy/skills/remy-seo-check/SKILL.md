---
name: remy-seo-check
description: Check one Remy page's on-page SEO without changing it: search title and description, social image, indexing, headings, alt text, link labels and CMS page settings.
---

Check the on-page SEO of one page, the one the owner names or is viewing, on the published or preview site and in its settings. Change nothing unless the owner asks. For the whole site, use remy-launch-check.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch; if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work in the project's preview at 1200, 810, about 700 and 390 px wide and in dark mode. If you can't see it, say so in your report.

- Read the rendered tags from the published or preview site with your web tools, and the page, CMS and site settings through Framer MCP. Without Framer MCP, mark each setting you couldn't see as needs manual review.

## Check

- **Title and description:** the published title, description, slug and canonical URL; missing, duplicated, conflicting or placeholder values; and whether the title, description, H1 and visible topic agree.
- **Indexing:** whether the page may be indexed (its search settings, robots tags, canonical URL, draft or published) and is listed in /sitemap.xml. Check whether the live URL is actually indexed if you can; otherwise mark it for manual review. Keep indexable, crawled and indexed apart.
- **Headings:** one H1 and an outline with no skipped levels. Each text style carries its level, so the fix is the style made for that job, not a changed tag.
- **Structure:** one Main frame tagged main holds the sections; the Nav and Footer sit outside it as header and footer.
- **Language:** the site language is set (Site Settings → General → Language); without it, pages have no lang attribute.
- **Images:** descriptive alt text, or empty alt on decorative images; the Service Card illustrations are empty on purpose. Portraits read "Portrait of [Full name]". CMS images take their alt text from the image in each item.
- **Links and buttons:** each has a label that says where it goes.

## Remy's setup

- Home has no title or description of its own; it uses the site title (the full name) and description in Site Settings. Other pages are titled "[Page] – [Full name]".
- /work/:slug and /blog/:slug are titled "{{Title}} – [Full name]", take their description from the item's Summary and their social image from its Social image field. Check every item in the Work or Blog collection for an empty or duplicated Title, Summary or Social image. Other pages share the site's social image.
- Work Summaries are 60 characters or fewer and Blog Summaries about 120, because the cards show them. A short description is expected, not an issue.
- /404 and /design-system are hidden from search engines on purpose; every other page should be indexable.
- "Remy Varga" or the sample case studies and posts in any title, description or alt text, and the template's social image (it shows Remy Varga and the sample projects), are placeholders: issue found, fixed with remy-make-it-yours.

## Rules

- Don't run a full accessibility audit (remy-accessibility-check), audit structured data, suggest visual changes or write new copy.
- If the owner asks for fixes, change only the page, item or site settings involved, and keep new copy to the limits in remy-remove-ai-writing. The site language is set by the owner; give them the steps.

## Report

Mark each item passed, issue found, needs manual review or not applicable, with its impact and where to fix it in Framer.
