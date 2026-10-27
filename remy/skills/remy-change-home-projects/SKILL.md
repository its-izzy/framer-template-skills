---
name: remy-change-home-projects
description: "Change how many projects Remy's Home page shows (3, 4 or 5) and which ones, or swap and reorder them."
---

Change which projects appear on Home (/) and how many: swap one, reorder them, or show 3, 4 or 5.

## Working from outside Framer

- Read remy-base first: it has the Framer MCP setup and the rules for every Remy task. If you can't reach the project, ask the owner to connect Framer and share the project link.
- Names in this skill are exact names in the project. Find each by name; if one is missing, ask, and never build a replacement.
- Framer MCP edits the owner's main version directly unless you work on a branch; if you use one, give the owner its name and link. Never publish, and merge only when the owner asks.
- Images come from the owner, as public links or dropped into their fields in Framer. Never generate or download images unless asked.
- If your tools can't do a step, give the owner the exact steps and list them in your report.
- Check your work in the project's preview at 1200, 810, about 700 and 390 px wide and in dark mode. If you can't see it, say so in your report.

- Projects is a choice (3, 4 or 5) on the Hero and Work instance on Home, not a number field. If your tools can't set it, finish the Home slots and tell the owner: select the hero on Home, then pick the number under Projects in the right panel.

## How it works

- **Projects** on the Hero and Work instance on Home sets how many (3, 4 or 5; 4 to start). **Home slot** in the Work collection sets which project fills each place (None, or 1 to 5).
- Slot 1 is the first row in Selected work and the leftmost print in the hero; each later print lies over the one before.
- The code file Travel.tsx lays out the prints for each count on desktop, tablet and phone. The canvas can't run it, so it shows the designed arrangement; the motion only plays in Preview and on the published site.
- Every project stays on /work: Home projects first, then the rest, each group newest first. On desktop and tablet each Project Card leans by its slot (odd slots and None left, even slots right); on phones they all lean left.

## Steps

1. Read the current Projects value and each project's Home slot, and show the owner the line-up (slot, project).
2. Work out the change. To swap, the new project takes the old one's slot and the old one goes to None. To reorder, renumber the slots. To change the count, set Projects, then fill or clear slots to match. If they don't give the order, ask once, suggesting their strongest project for slot 1.
3. If a project isn't in the Work collection yet, add it with remy-add-case-study first.
4. If the count changes, set Projects (or tell the owner how, as above).
5. Give exactly one project each slot from 1 to the count, and None to every other project.

## How many

- Suggest four; the stack reads best with four. Three and five are designed too.
- Fewer than three real projects: Home needs three. Offer to add one, or to keep a sample on Home for now and replace it before launch.
- More than five: Home shows five, so ask which. The rest stay on /work.

## What goes wrong

- Two projects in one slot: only one shows.
- An empty slot: Home shows fewer projects than the count.
- A slot above the count: the project isn't on Home, but /work still lists it with the Home projects.
- A draft project: it won't show on the published site.

## Rules

Change only Projects and the Home slots. Never move, resize, copy or delete anything inside Hero and Work.

## Done when

- Read back from the Work collection: slots 1 to the count each have one live project, and every other project is None. Projects is set, or you've told the owner how.
- If you can take screenshots, Home at 1200, 810 and 390 px shows one print per Home project and Selected work lists them in slot order.
- You've given the owner the final line-up and what changed.

## Then ask the owner to check Preview

At desktop, tablet and phone sizes, in Preview or the branch preview:

- The prints fade in with the line under the headline, from left to right.
- Resting the pointer on a print brings it forward; on phones a tap does, and a second tap opens the project.
- Scrolling down sends each print into its row beside its project, where its pin appears, and scrolling up returns them.
- On /work, the Home projects come first.
