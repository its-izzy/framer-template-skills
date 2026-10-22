---
name: remy-design-system
description: "Build or change pages and sections in Remy with its design system (layout, components, text styles, colors, motion, imagery). Use for any new page, section or layout change."
---

Build pages and sections from Remy's existing system, so new work looks like it was always part of the template. A new identity is the owner's name, copy and details in the existing styles: use remy-make-it-yours. Changing colors or fonts is a site-wide rebrand, done only when the owner asks.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch; if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work in the project's preview at 1200, 810, about 700 and 390 px wide and in dark mode. If you can't see it, say so in your report.

## When the request is vague

If you can't tell the page's goal, content or sections from the request and the site, ask before you build (skip this when the request is detailed or the owner says to just build it). Read the site first, then send one message: a rough outline (sections in order) and 4 to 6 numbered questions, each with your suggested answer. Choose from: goal and audience; features (filtering, a form and its fields, search, an FAQ that opens, a link out); what each item shows; real or sample copy; whether repeating items should be a CMS collection with their own pages; which page it should feel like; images; adding it to the Nav and Footer. Include anything on the ask-first list. If the owner skips a question or says "use your suggestions", use yours.

Example, "Create a careers page": Outline: statement opening → open roles → how we work → Contact CTA. 1. Who's hiring? Suggested: a small studio hiring full-time designers. 2. Filter roles by team? Suggested: yes, Filter Tabs set up like Work's. 3. What does each role show? Suggested: title, team, location, type and salary range. 4. How do people apply? Suggested: a form on each role's page (name, email, portfolio link, note). 5. A Roles collection with its own pages? Suggested: yes, with a record opening. It's a new collection, so I'm asking. 6. Real roles or three samples? Suggested: samples with [PLACEHOLDER] salaries.

## References and asking first

- /design-system is the source of truth for color, type, surfaces, layout, section patterns, motion, voice, components, imagery and the content model. Read its values instead of restating them from memory.
- Use Home (/), /work, /work/:slug, /blog, /blog/:slug and /contact as layout examples. Reuse and combine their section layouts; copying a whole page needs the owner to ask for a close match.
- Compose from Remy's parts, but don't force a poor fit. Ask first before anything new: a component, a section layout, a change to a shared part (component, style, layout template), or a CMS collection or field. Skip the question when the owner asked for that exact thing. Keep new things page-local unless they're reused.
- If the owner asks for something these rules discourage, say why in one line and ask before doing it.

## Home

- Home's Service Card instances sit in two frames, Pair 1 and Pair 2, inside Service Cards: four across, two by two when a card would drop below 220 px (each pair is at least 464 px wide), one column on phones. Keep the pairs when you add, remove or reorder services.
- Hero and work holds the hero's 3D stack and the Selected work rows; it sits once on Home with a Projects setting (3, 4 or 5). Never copy it to another page. It has a Print area for each count, so a change to the hero prints (tilt, hover) goes in all three areas, in the Desktop, Tablet and Phone variants.
- The canvas shows the prints where they're designed; Travel.tsx lays them out in Preview and on the site and fades them in one at a time, left to right, with the role line (the Subheading layer). It takes that timing from the role line's appear effect: change the timing there, and never remove that effect.
- Home turns off the Main layout's Space for nav switch, so the hero fills the window with the nav over it (the hero's top padding includes the nav's height). Every other page keeps the switch on.

## Components

- Check section 08 of /design-system and the live components first, and use one whenever its variants and properties can do the job. Make a new reusable component only for something used more than once or for an interaction (ask first); one-offs stay page-local.
- Never edit a shared component unless the owner asks for a site-wide change; ask first even when it seems harmless, and say why it is.
- Place one instance on Desktop and set its variant on Tablet and Phone. Use a second copy only when the element moves on a breakpoint, as Contact's phone Polaroid does, and hide the other copy there.
- Set the breakpoint variant on every component that has one: Project Row, Project Card and Post Card (Tilt left phone or Tilt right phone), Label Row (its phone variants), Wide Print, Contact Form and Choice Chip. A Desktop variant left on Phone is a defect.
- Project Card is the only card for projects and Post Card the only one for posts; feed them from the Work and Blog collections, never by hand.
- Images are framed: a Print, a Wide Print, a Polaroid or a component's own image. Use a bare image only when the owner asks. Neighboring prints tilt in opposite directions.
- Cards lean on hover, never straighten: a Print, a Wide Print, a Service Card and the Print in a Project Card or Post Card lift 6 px, take the lifted shadow and turn 1° further the way they lean (0.5° for a Wide Print), then settle back. Set the hover's rotation from the card's own: −2° hovers at −3°. In the Home hero a print doesn't lift; it only leans toward the pointer until it lands in Selected work.
- Use Label Row for label-and-text rows, Detail for contact details and Outcome Stat only for a real, measurable result.
- Use Button for calls to action and Arrow Link for text links with an arrow. Work, Blog and Contact open with an Arrow Link (Back variant) to Home, and case studies and posts with All projects and All notes; give a new top-level page the same Back row, duplicated from Work (32 px bottom padding, 16 px on phones), with its fade first.
- Contact CTA ends content pages, as on Home, Work, Blog and the case study, unless the page already ends with a contact action or the owner says not to.
- End a long-form page as the case study does: a Section Header (Compact with link) above the next item's Project Row and Print, never a small text link. A post ends with More notes: a Section Header (Compact with link) above three Post Cards, leaving out the current post.
- Filter Tab can filter any list: copy Work's setup, where the tabs set a page variable and the lists read it. Falling Print stays on /404.
- Never put a link inside another link; Framer strips the inner one. Print, Project Row, Arrow Link, Button and both cards already link, so link each piece instead of wrapping them, as the case study's next project does.

## Shared layout and identity

- Apply the Main layout template to every new page, and keep its Nav and Footer. On a CMS detail page, the Back to top link is bound to the entry (/work/:slug#top).
- The Use template button (in the Main and Main · 404 layouts) and the Nav's Design system link are only for the template's demo; remy-make-it-yours removes them. Don't copy them into new work.
- The owner's name, email and copyright live in the Wordmark, Nav, Footer and Contact CTA components; editing them changes every page, so ask first.
- Give every new page its own search title and description.
- Keep the Nav's items, order and destinations. Offer once to add a new top-level page to the Nav; if yes, add it to the bar and the phone menu with the same link style. In the phone menu, duplicate an existing row: its tap closes the menu, and its Tab index stays -1 so the link is the only keyboard stop.

## Layout

These are Remy's defaults. Check a matching section on the site first; if the owner has changed the spacing, follow the site. Every section has this structure (Home's hero and Selected work are the exception); don't flatten it or add a wrapper that repeats the gutter:

- **Main**: one per page breakpoint, tagged main: width 1fr, vertical stack, centered, no gap or padding.
- **Section**: a child of Main, tagged section: width 1fr, height fit content, vertical stack, centered. It holds the vertical padding and no side padding.
- **Container**: the Section's only child: width 1fr, max width 1360 px, side padding 40 px on Desktop, 32 px on Tablet and 20 px on Phone. It holds the gutter and the content gap.
- **Padding:** a content section has 96 px top and bottom on Desktop, 80 px on Tablet and 48 px on Phone. An opening section has 48 px top on Desktop, 40 px on Tablet (the case study keeps 48) and 32 px on Phone; the layout already clears the Nav. Its bottom follows Work (48, 48, 32 px), is 0 when the next section continues the same content (as on Contact), or matches the page you're borrowing from (the case study's opening ends with 64 px).
- **Gaps** aren't one scale: take them from a reference section with the same structure, for all three breakpoints (24 px in the Contact CTA; 56 px between a Section Header and the card grid on Work). Stay on the 4 px scale; 2 px steps only inside small parts such as captions, frames and the Nav bar.
- **Phones:** Phone covers every width below 810 px. Card lists use a grid that adds columns when there's room: auto-fill, 240 px minimum, 20 px column gap and 56 px row gap, as on Work and Blog; Desktop and Tablet keep fixed column counts. A print or card is never wider than 300 px; in one column, center it and let its text run full width. Tap targets are at least 44 × 44 px, 8 px apart.

## Surfaces and color

- Sections sit on Background Page; never give one its own background. Sheets (prints, the polaroid, service cards, the contact form) use Background Card, and only these get a shadow, in the Shadow color.
- Corners are square. Only pins, buttons, chips and tabs are round.
- Rules and dividers are 1 px Border; the Section Header rule is 2 px. Form field underlines, the note's ruled lines and choice chip outlines use Field line, and a focused field shows a 2 px Focus ring underline.
- A checked choice chip has a 2 px Action border. A chip reached with the keyboard shows the 2 px Focus ring with a 2 px gap; a click or tap shows no ring. The ring is the Focus style on the Checkbox layer in the Choice Chip component, and the withKeyboardFocus override from ChipFocus.tsx, on the chip's variants, hides it after a click or tap. Restyle the ring in that Focus style; never delete the Focus style or the override to hide it.
- Each color style has one job. Text Primary and Text Secondary are for text and icons (Text Primary also draws the Secondary button's outline). Action fills Primary and Send buttons and marks selected states: the active filter tab, a hovered tab's outline, a checked chip. Text Inverse is for text and icons on Action. Field line is for form lines and Focus ring for focus on fields and chips; links and buttons show the browser's own focus ring. For brand-colored buttons, change Action's light and dark values and check Text Inverse still reaches 4.5:1 on both.
- Accent is a highlight: pins, a statement's full stop, the wordmark's dot, outcome figures and the Send button once a message is sent. Never links, buttons, hover, focus or errors.

## Motion

- Each section's direct content blocks get the in-view appear from section 06: fade in and rise 24 px, 0.6 s, ease 0.33, 1, 0.68, 1, threshold 0.2, replay off, no exit, siblings 0.08 s apart in reading order (at most four steps). Opening blocks on a new page use the same fade on load (0, 0.08, 0.16, 0.24 s), even when already in view. A large print or image is its own block.
- When a block has its own hover (a Print, a Wide Print or a Service Card), put the appear on a frame around it, never on the card: a layer with both comes back late, or straight, after a hover.
- The Home stack's Print · Slot frames keep an opacity-only appear; never add movement to it, since the stack code plays their fade-in.
- Nothing loops. No parallax, marquees, custom cursors, 3D flips, bounce, or motion or decorative blur; the Nav's background blur and the Home stack's 3D turn and pointer lean are the exceptions. /design-system stays static.

## Contact form

The form shows errors with the Field component's variants (Text error, Email error, Note error): the withFieldError override from FormNote.tsx, on each Field instance, switches a wrong field to its error variant and back once it's fixed. Change how errors look in those variants and what they say in each Field's Error Message property. Add a field by duplicating a Field so it keeps the override; a new kind of field needs its own variant plus a copy named " error".

## Typography and copy

Choose text styles by job; each heading style carries its heading level. Never change a level on a layer: a job that needs another level needs its own style, which is ask-first.

- Page titles are h1, one per page: Heading/Page title on Work, Contact, Blog and new general pages; Heading/Home title for Home's headline (a step smaller on desktop, to leave room for the stack); Heading/Record title for CMS detail pages; Heading/404 title for the 404 headline only.
- Lead under the page title: Body/Body L. Body copy: Body/Body M. Summaries and secondary copy: Body/Body S.
- Section headings are h2 from the Section Header: its Large variant uses Heading/Section title, its Compact variants Heading/Section label. A section heading without a Section Header uses Section title.
- One level below, h3: Heading/Card title for card titles and Heading/Row title for project names in a Project Row.
- Large serif text that isn't a heading: Display/Statement for statements and intros, Display/Stat for outcome figures, Display/Signature for the wordmark and the Polaroid caption.
- Long-form text follows the case study: Body L paragraphs with 16 px paragraph spacing, in a column up to 643 px, with subheads as Heading 2 styled Heading/Subhead.
- Label/Label M is for metadata (disciplines, years, roles) and is never a heading. Navigation, buttons, tabs and chips use Label/Label L; captions use Label/Label S.
- Text typed on the canvas keeps its own paragraph's level, so a typed heading may borrow another's look (the Contact CTA's "Write to me." is Page title typed as h2). Text from a property or the CMS takes its style's level; in CMS rich text, subheads are Heading 2 (Subhead) and paragraphs Body L.
- A serif heading has at most one italic phrase. When a serif statement ends with a full stop, color only the full stop Accent. Section and card titles have no full stop.
- Sentence case; no all caps, eyebrows or overlines unless the owner asks. Keep paragraphs under 680 px wide.
- Use the owner's text when they give it. Sample copy reads like a real person wrote it, with varied paragraph lengths; sample CMS text is complete paragraphs. Placeholders are in capitals and square brackets, such as [CLIENT].
- Follow the voice in section 07: plain, specific and calm, in the first person. Mix short and long sentences, don't open every sentence with "I", and use contractions (I'm, it's). No em dashes, exclamation marks or filler such as "passionate about" or "seamless".

## Page openings

Open a new page by duplicating the closest existing opening and changing its words, so its spacing, fade-in and tablet and phone layouts come with it.

- **Statement opening** (/work, /contact), for general and index pages: a Page title with one italic phrase ending in the Accent full stop, then a Body L lead.
- **Record opening** (/work/:slug), for CMS detail pages: back link, a small label (such as the date), the Record title, then the Body L summary. Keep the details column only when the entry has real details. The main image goes in a cover section after the opening.
- **Centered record opening** (/blog/:slug), for long reads: the back link stays top left, then a centered date · topic label, the Record title and the Body L summary, with the cover below as a pinned Print in a centered column.
- If none suits the content, design a new opening from Remy's styles and components, and ask first, as with any new section layout.
- Only titles you write get the italic phrase and Accent full stop; titles from the CMS stay plain. A label above a statement title and controls under the lead are optional. Openings are text only, in bounded columns.

## Imagery

- Use project images or images the owner supplies, unless the owner asks for stock, generated or outside images. If nothing fits, ask for images instead of sourcing them. Don't create fictional interfaces, diagrams or decorative artwork unless asked.
- Use Remy's image pieces: Wide Print (Single or Pair) for covers and wide images, Print for grids and walls, the Polaroid and the Falling Print. Use several images when the page covers several subjects, and change the number of prints to suit the content.
- Shapes are fixed: Print 4:3, Wide Single 3:2, Pair 4:3. Pick the closest, and check nothing important (text, a face, an interface) is cut off.
- Give repeated instances different images or icons unless the owner asks for repetition. Bind CMS list images to collection fields, never one fixed image.
- Give every meaningful image one plain sentence of alt text on what it shows, not repeating its caption; leave decorative images without. For CMS images, write it in the entry's image field.

## New CMS collections

A new collection is ask-first. Once agreed, build it like the Work collection:

- **Fields:** Title, Slug, Summary (card text, detail page lead and search description), Cover image and Social image; a Date or Year when entries are time-based; then what the content needs. Sentence-case names, grouped with dividers. Title, Slug and Summary are required.
- **Body:** one Body rich-text field for free-flowing writing; separate fields only when every entry has the same sections, as Work's Brief, What I did and What changed.
- **Detail page:** a record opening. Search title "{{Title}} – " plus the owner's name, description from Summary, social image bound to the entry. A link to the next entry is optional, for collections meant to be read in order.
- **Index page:** entries bound to the collection, on a card that fits. Project Card suits an image, label, title and summary, but its Outcome row always shows, so entries without an outcome leave a gap; a new card is ask-first. Add Filter Tabs when categories are worth filtering.
- **Dates** display as "March 12, 2026".
- **Samples:** when asked without a number, make 3. Leave them live and list them in your report.

## Naming layers

Name sections by their content (Hero, Services, Open roles) and groups inside the Container by role (Title group, Lead, Details); name text layers by role (Heading, Lead, Label, Body).

## Before you finish

Check: components used, not rebuilt, with breakpoint variants set; Main › Section › Container with the right gutters and padding; text styles by role, one h1, headings in order; images bound or supplied, with alt text and good crops; nothing overlaps, clips or overflows, and every link works; search title and description set; copy reread as remy-remove-ai-writing describes. Then report what you built or changed, placeholders left, anything not done (including steps for the owner, such as publishing or site settings) and any new component or section layout, for review.
