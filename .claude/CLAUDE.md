# VA conventions

Standing rules for VA (virtual assistant) work on Zack's email, docs and messages.

## Links in emails and drafts

- **No `google.com` in any URL, ever.** That covers Google redirect links (`https://www.google.com/url?q=...&source=gmail&ust=...&sa=E`) and Google Drive links (`drive.google.com/...`). Replace redirects with the direct URL they point to. For files, link a copy on Zack's own sites instead of Drive, e.g. the EPK at `https://investors.redeyezack.co.uk/RedEyeZack_EPK_2026-10.pdf`. If a file only exists on Drive, ask Zack where to host it rather than sending a Drive link.
- **Don't put links into drafts through the Gmail connector.** Tested 28 Oct 2026: `create_draft` and `update_draft` rewrite every link into a `google.com/url` redirect when saving, in both the HTML and plain-text parts. That includes bare text like `redeyezack.co.uk/x`; a link without `https:` becomes a dead `javascript:void(0)`. The `get_draft` view shows these redirects even on links Zack added by hand, so check the `RAW` format before deciding a draft is broken. To get clean, clickable links into an email, do one of these:
  - Zack adds the links himself in Gmail: select the text, press Ctrl+K (⌘K on Mac) and paste the direct URL.
  - Give Zack a page with the email and a "Copy email" button that copies rich HTML, which he pastes into the draft in Gmail. Gmail keeps the direct links when the email is pasted in like this.
  - If a draft already has redirect links, give Zack the list of direct URLs to put back. Don't save the draft through the connector again.
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
