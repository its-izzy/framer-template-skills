You are working on Remy, a Framer portfolio template for designers, styled as prints pinned on a gallery wall.

Sections and layers can't be @ linked, so Remy's skills name them exactly, with the page or component they sit in.

## Always

- Never publish the site. The owner publishes. Don't switch a draft CMS item live, even for a moment to check or screenshot it: a live item can be published or seen.
- Use only the existing color styles, text styles and components. Never type a hex value or set a font size by hand.
- Read [/design-system](framer://page/Eha__ofhd) before you build and follow its "For agents" notes unless the owner asks otherwise. Never delete it: if the owner wants it off the live site, suggest making it a draft page, which keeps it in the project unpublished. If it's already gone, follow remy-design-system and the existing pages.
- Project and post copy comes from the [Work](framer://cms/Uxpr_Zwmx) and [Blog](framer://cms/dNyURhvHD) collections; never type it onto a page.
- Keep component instances linked, and change them through their properties. When you change every instance of a component, change only the owner's pages: the samples on /design-system and in the [User guide](framer://design-page/gIQGosbo5) document the template.
- Never edit the code files ([Travel.tsx](framer://code-file/codeFile%2FwSq_6q5), [FormNote.tsx](framer://code-file/codeFile%2FZiL2Bvn), [LocalTime.tsx](framer://code-file/codeFile%2Fer18XLU), [NotFound.tsx](framer://code-file/codeFile%2FHM1kwKk), [ChipFocus.tsx](framer://code-file/codeFile%2FFAWOKNU) and [NavKeyboard.tsx](framer://code-file/codeFile%2FMjhLh31)) unless the owner asks. The Home stack, the contact form, the Nav clock, the 404 print, the chips' focus ring and the Nav's keyboard behavior run on them.
- Never delete or rename CMS fields or layout templates. Keep the Top layer on [Home](framer://page/augiA20Il) and the layer names inside [Hero and Work](framer://component/Qn2M8ncuc) (Hero text, Subheading, Selected work, Project · Slot 1 to 5): [Travel.tsx](framer://code-file/codeFile%2FwSq_6q5) finds them by name.
- Every page's sections sit inside one Main frame, tagged main. The first section has the ID top and, where Space for nav is on, a top scroll margin as tall as the Nav spacer (92, 72 and 64 px on desktop, tablet and phone). Each page sets the [Main](framer://layout-template/HL8ISrmY9) layout's Back to top link to its own top, such as /work#top; only [/404](framer://page/G9aqTSexZ) turns its Show back to top switch off. Set up new pages the same way.
- Check every change at 1440, 1200, 810, about 700, 390 and 360 px wide, in dark mode and with reduced motion. If you can't view a width or mode, say so in your report.
- Before a big job (a new page, a rebrand, many CMS items), offer once to work on a duplicate of the project. Small edits go ahead.
- Write in US English (color, center, organize, license) unless the owner writes in or asks for another variety; keep one spelling across the site.
- Never present invented clients, results, quotes or prices as real. Write sample content only when asked; otherwise ask, or leave a placeholder in square brackets, such as [YOUR CITY], never a vague stand-in.
- The owner's details (name, email, city, time zone, links) come only from what the owner tells you. Never take them from the Framer account, the project's settings or anywhere else, even when the owner says "just do it". If they give nothing, ask once more in one short message, then use placeholders.
- Place the owner's words as given. Don't add emphasis, such as italics, that they didn't ask for; suggest it instead. When you change template text, keep its pattern (in a headline, the one phrase in italics and the green full stop) unless the owner asks otherwise.
- Reread any copy you write as remy-remove-ai-writing describes before you save it.
- "Today" means today in the time zone set on the Nav clock. Near midnight there, confirm the date with the owner.

## Before you report

- Read back every change before you report it, follow-ups included. If something didn't stick, try once more, then report it as not done, with the steps to do it by hand.
- Never report a form's Send To, a site setting or a domain as set unless you've read it back with the value; otherwise give the owner the steps.
- For anything you can't test yourself, such as keyboard use, clicks and the phone menu, give the owner a short list of steps to try.

## Sample content

- The sample designer Remy Varga, the portrait, the four services, five case studies in the [Work](framer://cms/Uxpr_Zwmx) collection (Halden, Ostra, Fieldnote, Kiln Week and Tern; Home shows four) and six posts in the [Blog](framer://cms/dNyURhvHD) collection are placeholders. Never present them as the owner's work or reuse their facts.
- Keep them until the owner's own entries are in, so no page looks empty, and replace or delete every one before launch.
- Before deleting a sample case study, fill Home slots 1 up to the Projects count with the owner's projects (remy-change-home-projects) and repoint the Next project that led to the sample.
