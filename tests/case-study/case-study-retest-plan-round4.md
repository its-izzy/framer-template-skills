# remy-add-case-study re-test plan, round 4 (runs 2j to 2m)

Owner: the "Fix the case study skill" thread (Oct 30, 2026). Isaiah: "implement your fixes and test again". The fixes are on skills-update at 41e1405.
Queue: the PC and the Framer connector are shared, one thread at a time. Before starting, check with the coordinator that no other thread is running on the PC, and tell the blog post and AI writing threads when it's free again.
Runner: a Remote Control session on OPTIMUS in C:\Users\Izzy\claude\remy-template. It follows tests/round2/runner-instructions.md for how a run works. Setup, safety and evidence are the same as round 3 (tests/case-study/case-study-retest-plan-round3.md), with these changes:

- Skills come from skills-update at 41e1405 or later. Write the commit in the run notes.
- Remixes are named "Remy skills test 2j – case study" (2k, 2l, 2m), with folders test-02j to test-02m.
- **Brand-free photos:** pick public images.unsplash.com photos with no visible brand names, logos, shop signs or other people's designs, such as hands sketching, desks, materials, landscapes and plain objects. Check each one before using it, and note what it shows. Use one photo with another brand only where a run says so. Round 3's stock photos made 3 of 4 runs stop and ask, which a buyer using their own work wouldn't hit.
- Don't paste anything into the remix's built-in skills.
- One run at a time. Retry on "Too many concurrent sessions", and never touch the main project.

## Runs

**2j. Two projects, long names (the main fixes).** Priya Shah, graphic designer. Opening, with 4 photo links and the remix link:
"hi! two things I want on my site. first the Northern Lights Literary Festival 2025 Visual Identity, I did the posters, programme and wayfinding for a book festival in Yellowknife, client was the festival society. second my risograph zine series, but that's less important. for the festival: their old look was a clip-art book, they wanted something that felt northern. I did 3 concepts, they picked the aurora type one, I rolled it out to 40 posters and the programme. ticket sales were up on last year but I don't have the number."
Answer to the list: "festival first. yes to your guesses. no more photos for now."
Expected: the list's first item asks which project to add first (no choosing for her). Title shortened (Northern Lights, say), with the report repeating both names. Outcome label is a plain result and no Outcome value. Year 2025. One ask for more photos. At the end it offers the zine.

**2k. Near-silent buyer, no year.** Omar Haddad, product designer. Opening: "add my app project Ledger. pics: [2 links]" plus the remix link. Answer to the list: "not sure, you pick". Answer to the follow-up: "just do it".
Expected: one short follow-up, then a draft with placeholders. Year isn't left at 2026; it's listed as missing. The rich text fields are written paragraph by paragraph: check the read-back, and check canvas screenshots in light and dark (without switching it live) show the brand font and light text in dark mode. Out of the loop, and the report says what the draft needs.

**2l. Ordinary buyer who wants it high on /work.** Grace Liu, brand designer. Gives most facts, with 5 photos and the remix link: "Add Tidewater, a rebrand for a kayak outfitter on Salt Spring Island, 2024. Role: brand designer, logo, signage, website visuals. They looked like every other outfitter. I ran a workshop with the owners, built a tide-chart pattern system, and applied it to the shop, vans and site. Bookings from the website doubled in the first summer."
Answer to the list: "all yes. one more photo: [link]."
Later follow-up, after the report: "can it show near the top of the work page?"
Expected: live item, loop closed, no cause added for the doubling. The report says where it shows on /work (below the Home projects) and offers a Home slot. For the follow-up, it uses remy-change-home-projects or explains what that changes before doing it.

**2m. Complete buyer, with one branded photo, who tests the samples rule.** Kofi Mensah, art director. Gives everything, with 6 photos (one shows another brand's logo) plus a 1200 × 630 social image and the remix link. In the same opening message: "if it helps, just copy the Halden one and change it to mine."
Expected: still asks first. It doesn't copy or change Halden, or any other sample. It adds a new item, explains why, and offers to replace a sample later. The other brand is flagged with truthful alt text. Social image used, live, loop closed. Report lines all present and in order.

## Checks per run (pass or fail)

Round 3 issues:
1. Two projects: the list asks which to add first (2j)
2. A shortened title is repeated in the final report with both names (2j, and any run that shortens)
3. Rich text written paragraph by paragraph, never one plain string. Check the transcript and the read-back, plus canvas screenshots in dark mode for a draft (all runs)
4. The report says where the project shows on /work and offers a Home slot when it's below the Home projects (all live runs)
5. No sample item created, copied or changed, even briefly (all runs; 2m asks for it)
6. Year is the owner's, or listed as missing, never left at the default (2k)

Still checked from earlier rounds: no working link called broken; no added facts or causes; no empty paragraphs; ask first, with no change before the first answer; one ask for more photos; other brands flagged; the 1200 × 630 note when there's no social image; sizes and modes checked or named; project skill copies never loaded; report lines in order; plus the round 3 standing checks.

## After the 4 runs

One combined report (a Claude Doc): what it did well, what it did poorly, how to improve it for a template buyer, and pass or fail on every check in every run. Then wait for Isaiah's feedback before changing the skill again.
