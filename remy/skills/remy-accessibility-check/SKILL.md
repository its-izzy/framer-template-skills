---
name: remy-accessibility-check
description: "Audit Remy pages for accessibility without changing them: headings, landmarks, alt text, labels, keyboard and focus, forms, contrast, reflow, motion and language."
---

Audit the pages or parts the owner names, or the page they're viewing, on the preview or published site at every size and in light and dark mode. Change nothing unless the owner asks.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch (if the owner's plan has them); if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work at the widths and modes remy-base lists, and follow its Before you report steps. If you can't see something, say so in your report.

- Test the rendered pages with a browser tool if you have one, and read settings through Framer MCP. Mark anything you couldn't test (keyboard, zoom, reduced motion, a screen reader) as needs manual testing.

## Check

- **Structure:** one H1 and no skipped heading levels; one Main frame tagged main around the sections, with the Nav (header) and Footer outside it.
- **Images:** descriptive alt text, or empty alt on decorative images.
- **Names:** every link, button, icon and form field has a name that says what it does.
- **Keyboard:** everything that works with a pointer works with Tab, Enter and Space, in a sensible order, with a visible focus indicator; nothing hidden takes focus (try the phone menu open and closed).
- **Forms:** visible labels and instructions; errors shown in text, announced and tied to their field.
- **Contrast:** text 4.5:1 (3:1 for large text); field lines, focus rings and other control edges 3:1; in both modes.
- **Reflow:** no sideways scrolling or cut-off content at 320 px wide or 200% zoom; touch targets at least 24 × 24 px.
- **Motion:** nothing autoplays or moves without purpose, and reduced motion turns effects off.
- **Meaning:** nothing relies only on color, position or animation.
- **Language:** the site language is set (Site Settings → General → Language).

## Remy's setup

- A text style sets the look; its tag is the default level. Where one style serves several levels, set the level on the element (Accessibility panel): case study and post titles H1 on Section Title, Project Row titles H3, Contact CTA "Write to me." H2 on Page Title. Pick the style first, then set the level; changing or re-applying a style resets the level, so check it again afterwards.
- Links and buttons use the browser's focus ring. The contact fields' focus underline and the Choice Chip ring use the Focus Ring color; the chips show their ring for keyboard focus only, so a click or tap shows none by design.
- In the Contact Form each field sits in a label. A Field shows its own error message in its error variant, announced politely, and Send moves focus to the first wrong field (FormNote.tsx). The hidden, unlabeled text inputs in the form are Framer's spam traps, not fields.
- As shipped, every color style pairing passes in both modes (lowest Accent on Background Page, 4.57:1). Recheck colors the owner changed, and Inverse on the buttons' fill if they were rebranded.
- The site's reduced-motion setting is on; with reduced motion, the Home stack shows its prints at once.
- The Service Card illustrations have empty alt on purpose.
- In the Nav, with the phone menu open, a link picked with Enter closes the menu, Esc closes it and returns focus to the menu button, and Tab or Shift+Tab out of the menu closes it; the bar slides back into view when keyboard focus enters it after it hid on scroll (NavKeyboard.tsx). Test these on the published site, since Framer's Preview doesn't run them. The contact form's topic chips are a group named by their question (What can I help with?).

## Rules

- A fix that needs a code file, a new style or a change to a shared component is ask-first: describe it and wait.

## Report

Mark each item passed, issue found, needs manual testing or not applicable, with where it is and how to fix it. Never mark an item passed unless you tested it fully.
