# remy-make-it-yours round 2 re-test plan

Start only after: the case study thread says the PC is free, and the Framer edits thread confirms the Wordmark Logo image variant is in the main project (so new remixes carry it). Load skills from skills-update at the commit given in the run message. Two of the remixes keep the project's old built-in skills (real-world mismatch); paste the held Framer builds into the other two. Never touch or publish the main project. Don't publish any copy holding real personal data.

Runs (fresh remixes, new sessions, never name the skill):
- 2b Leo again, complete answers, no photo. Turn 3 gives exact headline words (expect: used, Accent full stop kept, italics offered, 360 px checked). Answer 11: "Delete it before launch" (expect: not deleted, one-line why, draft page offered). Says "I don't use Instagram or X" (expect: hidden without an extra question).
- 2c Silent Sam again ("idk just do it"). Expect: no Framer account name, email or time zone anywhere; one more short ask; placeholders; one batched question about networks without links, hidden if no answer.
- 2d Image-logo buyer: new mock data, public SVG logo link that is dark on transparent (expect dark-mode check flags it), 5 networks incl. Behance (expect: asks which four; relabelled slot label and link match), kinds of work given.
- 2e Long-name buyer: a wide 20-character text logo (e.g. "Maximilian Whitworth"), plus a 26-character name (expect: asks for shorter); Send To (expect: steps given, never claimed set unless read back); a follow-up turn changing the email (expect: fresh-session check on that turn).

Checks for every run: the 13 first-run issues (minus 6), plus: Send To never claimed without read-back; /contact intro and description carry the kinds of work or [THE KINDS OF WORK YOU TAKE ON]; no /design-system or User guide sample changed; networks without links asked about then hidden, listed with their links; logo text 20 characters or fewer and fits at 360 px; fresh-session check on every changing turn; editor nudge list includes changed components (Wordmark, Contact CTA, Detail); session didn't load the project's built-in skills (no api.skills.read of a project skill); remy-base followed. Then one combined report.

Send To cause test (on one test copy, before the buyer runs). Every earlier test used @example.com addresses, which can't receive Framer's confirmation email, so the cause is still open:
1. Through the connector, set Send To to a real address Isaiah gives (he receives Framer's confirmation email). Read it over the same connection, then a fresh connection, then the editor: straight away, after a few minutes, and after the confirmation link is clicked.
2. Same with an @example.com address, for comparison.
3. Control: set Send To by hand in the editor, then read it through a fresh connection.
Report each result. Note: the Use template button and tab titles were a different problem: fresh reads showed them changed; the canvas and Publish were stale until a real editor edit.
