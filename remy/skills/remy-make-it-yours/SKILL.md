---
name: remy-make-it-yours
description: "Make Remy yours: replace the sample designer with the owner's name, logo, city, contact details, links, portrait, About, services, project categories and blog topics. Read remy-base first."
---

Replace the sample designer, Remy Varga, with the owner everywhere except the Work and Blog collections, whose sample entries are replaced with remy-add-case-study and remy-add-blog-post.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch (if the owner's plan has them); if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work at the widths and modes remy-base lists, and follow its Before you report steps. If you can't see something, say so in your report.

## 1. Ask in one message

One numbered list, each item with a short example; say anything they don't have yet can stay a placeholder:

1. Full name, for the footer, page titles, alt text and About (Remy Varga)
2. Logo: their name as text, up to 20 characters, usually the first name, with the Accent full stop added (Remy); or their own logo, as a public link to an SVG or PNG with a transparent background
3. City, time zone, and a 12-hour or 24-hour clock (San Jose, Pacific time, 12-hour)
4. Email
5. Profile links for up to four networks they use. Instagram, LinkedIn, Dribbble and X are set up; another network, such as Behance or their Framer profile, can take the place of one they don't use (instagram.com/remyvarga)
6. A one-line role, and the kinds of work they take on (Independent Product and Brand Designer; product, brand and systems work)
7. A portrait photo, at least 1200 px wide, and a short caption (Remy, at work)
8. When they're next free for new work (Booking from [month and year])
9. For About: a two- or three-sentence intro, their background, their approach, and their career as years and roles (2019–2023, Senior product designer, Pliant)
10. One or two sentences for the byline under every blog post (I'm Remy, a designer working across product, brand and systems.)
11. The four services on Home, each a title of two or three words and one sentence, plus an image if they have one (Product design: Research, flows, prototypes and interface design, from first sketch to shipped release.)
12. Project categories, which filter /work (Product design, Brand identity, Design systems, Graphic design, Art direction), and blog topics, which filter /blog (Process, Systems, Craft): keep them, or send their own
13. /design-system is their private reference for the site's styles: keep it published but hidden from search, or make it a draft page so it isn't on the live site at all?

Wait for answers. Anything missing becomes a placeholder in capitals and square brackets, such as [YOUR EMAIL]. A link can't hold a placeholder: leave it as it is and list it.

Run this skill only when the owner asks to make the site theirs or to change these details, never as the next step of another task. Before you change anything, say in one short message what will change: the shared parts (logo, Nav, Footer, Contact CTA) show on every page; name which details become placeholders, that renamed categories and topics change every project and post that uses them, and that you'll remove the Design system links and the Use template button. Then wait for a yes; "just do it" counts as one only once you've said this.

## 2. Change

1. Wordmark: the logo text, up to 20 characters with spaces, so it fits the Nav on the smallest phones (about 24 fit at 360 px; 20 leaves room for wide letters). If the owner's is longer, ask for a shorter version, such as the first name or initials, and use the first name until they answer. Keep the Accent full stop. With their own logo file, switch the Wordmark to its Logo image variant, put the image in its Logo property (or tell the owner to drop the file there), and set the image's alt text to their full name. Images don't change with dark mode, so check it on the dark background too; if it's hard to see there, tell the owner and ask for a version that works on both.
2. Footer: the copyright line, © with the current year and the full name.
3. Nav: the city in the bar and in the phone menu ("Based in [City] ·", followed by the clock); the Local Time clock's Time Zone (an IANA name such as America/Vancouver) and Clock (12-hour or 24-hour); the phone menu's email (text and mailto link). Remove the Design system link from the bar and the phone menu.
4. Main layout: delete the floating Use template button (the Use template (floating) layer, which links to a placeholder remix link) on Desktop, Tablet and Phone.
5. Contact CTA: the email (text and mailto link) and each social link's address.
6. Contact Form: "Dear Remy," becomes the owner's first name. Send To, where messages go, must end up as the owner's email: a form that sends nowhere, or to the template's address, loses them real enquiries. Set it with your tools if they can (Framer MCP: patch the form's email destination on the Contact Form's main Form layer; its Tablet and Phone versions follow it) and read it back. In tests the address read back in the same session but was gone in every new session, so the write doesn't save: never report it as set, and list Send To as still to do until the owner confirms it in Framer. Always give the owner the steps to confirm it: select the Contact Form, select Form, check their email is under Send To (add it if not; if it isn't their Framer account's email, click Verify next to it and confirm the email Framer sends), and after publishing, send a test message from the live form to check it arrives. Without an email from the owner, leave Send To as it is and list it as still to do.
7. /contact: the intro's kinds of work ("across [kinds of work]") and the page's search description, in the owner's words: if they didn't list them, use what their own answers say (their About intro, say) and tell them where it came from, or else [THE KINDS OF WORK YOU TAKE ON]; the Detail rows Name, Email (value and mailto link), Based in, Availability and Elsewhere (each network's link), and both Polaroids' image, caption and alt text (one shows only on phones).
8. Home: the role line under the statement (the Subheading layer in Hero text, inside Hero and Work); change its words only, since the stack code finds it by name and times the prints from its fade. Write the role in Title Case, whatever case the owner typed it in ("[Full name], Independent Product Designer"), here and in the site title. Then, in About, the Polaroid's image, caption and alt text, the intro, and the Background, Approach and Career rows (years and roles, and the city on the current role).
9. /blog/:slug: in the Written by byline, the Polaroid's image and alt text, and the bio.
10. Portraits: with the owner's photo, put it in every Polaroid above with their caption and the alt text "Portrait of [Full name]". Without one, keep the sample photo but don't put the owner's name on someone else's face, which misleads visitors and screen reader users: set each caption and alt text to [YOUR PORTRAIT], and keep the caption they gave for the report. Change only the Polaroids and Details in steps 7 to 9. The samples on /design-system and in the User guide design page use the same components but document the template, so leave them as they are.
11. Search titles: replace "Remy Varga" with the full name on /work, /blog, /contact and /404, and in the case study and blog post title patterns ("{{Title}} – [Full name]").
12. Site settings: site title ("[Full name] – [Role]", with the role as worded in the role line from step 8) and description (one sentence from their About intro, under about 155 characters; if you reword it, say so), plus their own favicon and 1200 × 630 social image if they have them; the template's are Remy's.
13. Networks: put each profile link the owner gave in its slot in the Contact CTA and the Elsewhere row. A network that isn't set up (Behance, Framer, GitHub) takes the slot of one they don't use: change that slot's label (a text layer in the Contact CTA component, and in the Elsewhere variant of the Detail component) and its link in both places, and read both back, so no label points at another network. If the slot's link property is named after the old network (X), rename it to the new one so the editor matches. The samples on /design-system change with the components, which is expected. With more than four, ask which four to show. If they want all of them shown, don't add a slot in this skill, even when they ask for it outright: a fifth slot changes the shared Contact CTA and Detail components across the site, including the /design-system samples. Say that, name remy-design-system as the skill that adds it, and wait for a yes before running it. Unless they've said they don't use it, before hiding any network they gave no link for, ask about all of them in one line ("You didn't give links for LinkedIn and X. Hide them, or send the links?"), since they may just have forgotten. If they say hide, or don't say, turn off its visibility in both places: a visible link that opens a network's home page looks broken. Don't delete them, so they can come back, and list each hidden one with the link it still holds.
14. Services: change only Home's four Service Card instances (in Pair 1 and Pair 2 inside Service Cards), through their Title, Description and Image properties, and rename each instance and its fade frame to match ("Service Card · [Title]", "Service Card · [Title] · fade"). Keep titles to two or three words so they fit the narrowest card. Without their own image, keep the sample one and list it. The images are decorative, so leave their alt text empty. If the contact form's chips name the sample services, offer to match them to the owner's. For fewer or more than four services, don't change the layout here: it's two pairs of cards, so say that, name remy-design-system as the skill for it, and wait for a yes.
15. Categories and topics: rename each option in place, in the Work collection's Discipline field or the Blog collection's Topic field, never the field itself. An option keeps its place in every item and in the filters when renamed, because the filters follow the option, not its name. Then change the matching Filter Tab on /work or /blog: its Label and its layer name ("Filter Tab · [Name]"). For fewer, turn off the tabs they don't want and keep the options, since sample items still use them; list them. For more, add each as a new option, add a tab set up like the others (its Label, the click that sets the page's filter to the new option, and the selected-state check), and add the option to the All tab's list, so All stays unselected while it's chosen. Then update every place the names are written out: the /blog intro (Lead) and the search descriptions of /work and /blog.
16. /design-system: keep it, hidden from search or as a draft page, as the owner chose. It's the owner's private reference, the other Remy skills read it, and the User guide design page links to it, so never delete it, even if the owner asks. Always tell them why in one line ("Other Remy skills and your User guide use it, so I've made it a draft page instead") and offer a draft page. A draft page stays in the project but isn't published; if your tools can't make one, give the owner the steps. Change nothing else on it: its samples are the template's documentation.

For anything your tools can't reach, give the owner the text and the steps.

## Rules

- Use only what the owner tells you, never their Framer account's name or time zone; never invent facts, years or employers.
- Home hero statement: when the owner gives exact words, use them. Change the words only (the stack code finds the Hero text layer by name), keep the Accent full stop, and offer a phrase to put in italics, as in the sample. Check it at 360 px; if it runs longer than the sample there, suggest a shorter version. If the owner wants the statement or the services written for them, draft them from their own answers, show them, and wait for a yes before you place them.
- Place the owner's words exactly as given. Don't add emphasis such as italics that they didn't ask for; suggest it instead.
- Write anything new in the voice from section 07 of /design-system, and reread it as remy-remove-ai-writing describes.

## Check before you report

Follow Before you report in remy-base after every turn that changes something, follow-ups included. For this skill:

1. Take canvas screenshots of Home, /contact and a blog post at Desktop and Phone, in light and dark.
2. Before the owner publishes, ask them to make one small real edit in the editor to the Main layout, to the search titles of /work, /blog, /contact and /404, and to each component you changed, such as the Wordmark (change any value, then change it back). After they publish, ask them to check the browser tab titles on those pages, and that no Use template button shows.

## Done when

- Searching the pages, components, layout templates, alt text, page titles and descriptions finds no "Remy", "Varga", "San Jose" or the sample email (hello@example.com), and no "Pacific time" unless the owner is on Pacific time. /design-system and the User guide design page are the template's own and may keep the name Remy.
- The logo text is 20 characters or fewer, and the logo, the Nav and the role line fit at every size, 360 px included. If you can't view 360 px, ask the owner to check Preview at the smallest phone size; don't say it fits unless you saw it.
- No Design system link in the Nav, and no Use template button on any page, in the read-back and in the screenshots.
- The email links open the owner's address, and every visible social link opens their profile.
- Home's services and the /work and /blog tabs show the owner's words, or the samples they chose to keep, each listed in the report; every tab still filters to its own items.

## Report

What you changed, page by page and component by component; anything that didn't stick, with the steps to do it by hand; every placeholder left, including the portrait and the caption to use with it, and the Nav clock if it's still on Pacific time because no city was given; every network you hid, by name, with the link it still holds, and any visible link still pointing at a network's home page; and what the owner still has to do: Send To; site settings your tools couldn't reach; the sample case studies and posts to replace.

End with a list headed "Sample content still on your site", one line each, so the owner can see at a glance what's still Remy's. List every sample left unchanged: each sample case study by name with its sample client, and the sample posts, with the skill that replaces them; the portrait; any sample service, service image, category or topic they kept; any link still pointing at the sample email or a network's home page; Send To, unless the owner has confirmed it; and any template wording still on their pages in the sample designer's voice or promising something for them, such as the /contact reply time ("I'll reply within a few working days"), the form's line on how details are used, and the headings and lead-ins on /work, /blog and /contact, so they can keep or rewrite each. If nothing is left, say so.
