# VA conventions

Standing rules for VA (virtual assistant) work on Zack's email, docs and messages.

## Links in emails and drafts

- Never use Google redirect links (`https://www.google.com/url?q=...&source=gmail&ust=...&sa=E`). Replace each one with the direct URL it points to.
- Keep every link as short as possible:
  - link to `https://`, and drop `www.` where the site works without it
  - show the short form as the link text, e.g. `destinationenglish.co.uk/appointment/2`
  - remove tracking parameters (`source=`, `ust=`, `sa=`, `utm_...`) unless the link needs them to work
- When asked to fix links, check **all** drafts, not just the one mentioned.
- Leave quoted text from earlier messages alone in reply drafts unless asked. Editing a reply draft through the Gmail connector can detach it from its thread and strip images from the quoted part. Flag these links to Zack instead.
- Check the draft has no attachments before updating it. The Gmail connector drops attachments that aren't re-sent with the update.

## Current facts (keep emails consistent with these)

- The India trip (winter 2026–27) is postponed. Don't say Zack will be in India, Goa or Pune this winter.
- Zack is available for gigs in the UK from 1 November 2026. Gig drafts end with: "I'm available from 1 November onwards."
- Mentioning past folklore festivals in Morocco, Turkey, India and Vietnam is fine.

## Where VA work is kept

- Z-Note (Zack's own notes app, source in `zackq207/z-note`) holds VA folders and artifacts: campaign plans, checklists, drafts and summaries.
- Z-Note's notes live on Zack's Mac (`~/Library/Application Support/Z-Note/znote-data/`), not in the repo. A cloud session can't write them directly, so hand work over in a form Zack can drop into Z-Note, and say where it should go.
- Mailchimp footer: keep the current postal address (London postcode). Zack has decided this; don't suggest changing it or paying for a PO box.

## Formatting for Zack

Zack can't read plain text dumps. Everything handed to him must be formatted for easy reading, or not given at all.

- Use real formatting: headings, short bullet lists, bold labels, tick boxes, spacing between sections.
- Never hand over `.txt` files, raw copied text, `[ ]` / `[x]` checklists or log output. Give a formatted page (HTML artifact), a Z-Note note (rich HTML), a doc, or formatted chat text.
- Notes to paste into Odoo or Z-Note must paste as formatted text (headings, bullets, tick boxes). If something can only be copied as plain text, don't offer it. Give a link to the formatted version instead.
- Copy buttons on pages copy formatted text only, with no plain-text fallback.
- Any note (Z-Note or Odoo) that relates to an HTML artifact starts with a clickable link to it, before anything else. Use a short, clear link text, e.g. "📘 Open Angela's course notes", not a bare URL. List every related artifact there, one per line. Exception: a homework page's link goes in the Homework & preparation section at the bottom.

## Students (Destination English)

**Angela is the working model for Zack's premium service:** the 30-minute weekly conversation class plus extras outside the class:
- a course plan with flexible topics, saved as a course notes page
- interactive homework pages with grammar game links
- quick checks and results
- tidy lesson notes in Odoo and Z-Note

Build every new premium student the same way, using Angela's setup as the template, and keep improving the template rather than one-off copies.

Each student's Odoo CRM card is the single record of their progress (Angela is card 223: `destinationenglish.co.uk/odoo/crm/223`). If it isn't on the card, it didn't happen.

- **Pipeline stages:** Enquiry → Level test → Test month → Regular → Paused / Finished.
- **Tags:** level (e.g. Pre-Int) and lesson day.
- **One log note per lesson** on the card, in this format:
  ```
  Lesson N – <date>
  Covered: …
  Homework: <destinationenglish.co.uk/student/... link>
  Result: <scores, weak spots>
  Next: …
  ```
- **Course topics are flexible:** a course has a list of topics that must all be done by its last lesson (Angela: Lesson 4). The order isn't fixed. The student's pace decides, so Zack moves topics between lessons as he goes. Each topic has a lesson and a status (Not started / Started / Done). A topic started in one lesson and continued in another shows in both lesson plans. Flag any topic not finished in a past lesson, and anything not done by the last lesson.
- **The course notes page is the live plan.** Zack moves topics and ticks items there, and the page saves itself (Angela: `claude.ai/artifact/LASyTzFxfn9zbiUKm5K22B`). Z-Note notes are copies made from it: when asked to update Z-Note, read the page first and rebuild the dashboard and lesson notes from what it holds.
- **Lesson plans and lesson notes:** every lesson uses the same sections, in this order, so Lesson 1, 2, 3… always match:
  1. Lesson plan (tick boxes)
  2. Results
  3. Still to cover
  4. After the lesson (Odoo log note, what was written in Odoo)
  5. **Homework & preparation**: a clearly marked, separate section at the end, never part of the lesson plan. It has three parts: Homework for the student (with the homework page link), Homework tasks, Preparation for me.
  Keep every heading even when a section is empty, and write "None" or "Add after the lesson".
- **One activity always set** for the student's next step (next lesson, or a homework check).
- **Homework and lesson pages** go on the website as `destinationenglish.co.uk/student/...` pages, linked from the lesson's log note. Don't give students claude.ai links or emailed PDFs.
- **Z-Note:** each student has a folder (Angela: `2026 Projects / Active / 1 DE / Angela Private Lessons`) holding:
  - **"<Name> – Master dashboard"** (pinned): the course notes link at the top, the student's details, an overview table of all lessons, then every lesson in full.
  - **"<Name> – Lesson N (<date>)"**: one note per lesson, with the course notes link at the top and the lesson in exactly the same 5-section layout as the dashboard and the course page.
  - Generate all of them from the same content so they never disagree, and update the dashboard whenever a lesson note changes.
- **Where to do the work:** student updates need Odoo, the website and Z-Note, so do them in a session on Zack's Mac. A cloud session can't reach them. If you're in a cloud session, say so at the start, do only what's possible, and give Zack a ready-to-paste log note for the card, formatted (see Formatting for Zack).
- **End of every student task:** confirm what was logged on the card, or list exactly what still needs logging.
