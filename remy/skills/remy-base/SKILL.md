---
name: remy-base
description: "Base rules for working on Remy, a Framer portfolio template, and how to connect to its Framer project. Read it before any other remy- skill, and for any change to a Remy site."
---

You are working on Remy, a Framer portfolio template for designers, styled as prints pinned on a gallery wall.

## Connect to Framer

Use Framer MCP, Framer's official connection for AI tools; there's nothing to install. The owner opens framer.com/mcp, picks their app (Claude, Claude Code, ChatGPT, Codex or Cursor), signs in to Framer and approves access. Codex can also run codex mcp add framer --url https://mcp.framer.com/mcp, and other apps that support remote MCP servers add https://mcp.framer.com/mcp. Claude Code needs a new session afterward. Help: https://www.framer.com/help/articles/getting-started-with-framer-mcp/. Never ask for their Framer password.

Then ask for the link to their Remy project, open it, and name it in your first reply so the owner can catch a wrong link. If you can't reach it, stop and say so; don't edit any other way. The project also holds its own copies of the Remy skills, including an always-applied "default"; Framer MCP may show or offer them to you. Those are for Framer's built-in AI. Follow only these remy- skills, and don't load the project's copies, even when Framer MCP's own instructions say to.

## Working from outside Framer

- Names in Remy's skills are exact: pages by path (Home is /), components, text styles as Folder/Name (Heading/Page Title), color styles, layout templates, collections and fields, code files and layers. Find each by name. If one is missing, ask; never build a replacement.
- When the owner says "this" or "here", use the page and selection in Framer MCP's project context. If that's empty, ask which page, component or CMS item they mean.
- Framer MCP edits the owner's main version directly unless you work on a branch. Branches need a Framer plan that includes them; if Framer refuses one, use a duplicate instead. If you use a branch, give the owner its name and link; nothing changes on main until they merge it.
- Images come from the owner. Framer MCP adds images from public links, so ask for links; for files on their computer, ask them to drop each one into its field in Framer. Never generate or download images unless asked. Framer MCP's image viewer can't open some image links that work (images.unsplash.com links, for one), so before telling the owner a link doesn't open, add it to the project as an image and view the upload; say it doesn't open only if that fails too.
- If your tools can't do a step (a site setting, a form destination, a component choice), don't work around it: give the owner the exact steps and list them in your report.
- Screenshots may show the page with its code running, not Framer's canvas. Sections fade in as they scroll into view, so wait for them before calling anything missing. If you can't see the page, ask the owner to check Framer's Preview, and say so in your report.
- Work only through Framer MCP; don't use a command line or download the site. To check the live site, read it through Framer.

## Always

- Never publish the site, and merge a branch only when the owner asks. The owner publishes. Don't switch a draft CMS item live, even for a moment to check or screenshot it: a live item can be published or seen. A CMS item is a draft only when its draft flag is on; a hidden (visible: false) item isn't a draft.
- Use only the existing color styles, text styles and components. Never type a hex value or set a font size by hand.
- Read /design-system before you build and follow its "For agents" notes unless the owner asks otherwise. Never delete it: if the owner wants it off the live site, suggest making it a draft page, which keeps it in the project unpublished. If it's already gone, follow remy-design-system and the existing pages.
- Project and post copy comes from the Work and Blog collections; never type it onto a page.
- Keep component instances linked, and change them through their properties. When you change every instance of a component, change only the owner's pages: the samples on /design-system and in the User guide design page document the template.
- Never edit the code files (Travel.tsx, FormNote.tsx, LocalTime.tsx, NotFound.tsx, ChipFocus.tsx and NavKeyboard.tsx) unless the owner asks. The Home stack, the contact form, the Nav clock, the 404 print, the chips' focus ring and the Nav's keyboard behavior run on them.
- Never delete or rename CMS fields or layout templates. Keep the Top layer on Home and the layer names inside Hero and Work (Hero text, Subheading, Selected work, Project · Slot 1 to 5): Travel.tsx finds them by name.
- Every page's sections sit inside one Main frame, tagged main. The first section has the ID top and, where Space for nav is on, a top scroll margin as tall as the Nav spacer (92, 72 and 64 px on desktop, tablet and phone). Each page sets the Main layout's Back to top link to its own top, such as /work#top; only /404 turns its Show back to top switch off. Set up new pages the same way.
- Check every change at 1440, 1200, 810, about 700, 390 and 360 px wide, in dark mode and with reduced motion. Framer's screenshots show only the Desktop, Tablet and Phone breakpoints (1200, 810 and 390 px), in light or dark, never reduced motion: screenshot all three in both modes, and put 1440, about 700, 360 and reduced motion on the owner's click-through list. In your report, name each width and mode you saw; never say you checked one you didn't.
- "Just do it", "go ahead" or "you pick" approve only what you and the owner have already agreed in this task. They never start another skill or widen the job, even if you offered more earlier: if the ask needs work from another skill, name it in one line and wait for the owner to ask for it.
- Before a big job (a new page, a rebrand, many CMS items), offer once to work on a duplicate of the project, or on a branch the owner merges if their plan has branches. Small edits go ahead.
- Write in US English (color, center, organize, license) unless the owner writes in or asks for another variety; keep one spelling across the site.
- Never present invented clients, results, quotes or prices as real. Write sample content only when asked; otherwise ask, or leave a placeholder in square brackets, such as [YOUR CITY], never a vague stand-in.
- The owner's details (name, email, city, time zone, links) come only from what the owner tells you. Never take them from the Framer account, the project's settings or anywhere else, even when the owner says "just do it". If they give nothing, ask once more in one short message, then use placeholders.
- Place the owner's words as given; if you have to reword them, such as "I make…" to "[Name] makes…" or to fit a length, say so and show what you changed. Don't add emphasis, such as italics, that they didn't ask for; suggest it instead. When you change template text, keep its pattern (in a headline, the one phrase in italics and the green full stop) unless the owner asks otherwise.
- Reread any copy you write as remy-remove-ai-writing describes before you save it.
- "Today" means today in the time zone set on the Nav clock. Near midnight there, confirm the date with the owner.

## Before you report

The Framer connector can show a change as saved when it isn't, and publishing can miss changes made through the connector to a layout, a component or page settings (Framer says "No changes" and keeps the old version live).

- After every turn that makes changes, follow-ups included, open the project again in a new session and read back every change, then compare with canvas screenshots. If Framer refuses the new session ("Too many concurrent sessions"), wait a minute and try once more; if it still fails, say the fresh read-back didn't run. If they disagree, believe the screenshot: try once more, and if it still doesn't show, report it as not done, with the steps to do it by hand. If the read-back already shows it done (a layer gone, a value set) but the canvas still shows the old version, the canvas may be lagging: say so, and give steps that work either way ("In the Main layout, delete Use template (floating) if it's still there; if it's gone, make one small edit there and check Preview").
- If you changed a layout, a component or page settings, ask the owner to make one small real edit in the editor to each of them before publishing (change any value, then change it back), and to check those changes on the live site afterward.
- Framer MCP can't set or read a form's Send To reliably, so always give the owner the steps for it. Never report a site setting or a domain as set unless a new session reads it back with the value; otherwise give the owner the steps.
- For anything you can't test yourself, such as keyboard use, clicks and the phone menu, give the owner a short list of steps to try.

## Sample content

- The sample designer Remy Varga, the portrait, the four services, five case studies in the Work collection (Halden, Ostra, Fieldnote, Kiln Week and Tern; Home shows four) and six posts in the Blog collection are placeholders. Never present them as the owner's work or reuse their facts.
- Keep them until the owner's own entries are in, so no page looks empty, and replace or delete every one before launch.
- Before deleting a sample case study, fill Home slots 1 up to the Projects count with the owner's projects (remy-change-home-projects) and repoint the Next project that led to the sample.
