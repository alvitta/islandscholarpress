# Island Scholar Press reader-copy setup

## Files
- `index-updated.html`: replace the current `index.html` with this file.
- `reader-copy.html`: reader-copy request form with URL referral tracking.
- `submit-review.html`: private review form with optional Amazon and Goodreads prompts.

## 1. Create two Formspree forms
Create one form for reader-copy requests and a second for reviews.

Replace:
- `YOUR_READER_COPY_FORM_ID` in `reader-copy.html`
- `YOUR_REVIEW_FORM_ID` in `submit-review.html`

The pages submit with JavaScript and reveal an on-brand success panel without
sending the visitor to an external confirmation page.

## 2. Add the book file
Replace `REPLACE_WITH_PRIVATE_OR_PUBLIC_PDF_URL` in `reader-copy.html`.

Important: anything stored in a public GitHub Pages repository is publicly
retrievable by someone who knows or discovers the URL. The form creates a
courteous access gate, not true file security.

For stronger control, use a storage provider capable of expiring or signed
download links and have an automation email the link after submission.

## 3. Add public review links
Replace:
- `REPLACE_WITH_AMAZON_REVIEW_URL`
- `REPLACE_WITH_GOODREADS_BOOK_URL`

## 4. Referral links
Share URLs such as:
- `reader-copy.html?ref=FAC023`
- `reader-copy.html?ref=FORMER-PHD`
- `reader-copy.html?ref=VIS-COLLEAGUES`

The `ref` value is submitted invisibly with the form and displayed in the
Formspree submission data.

Use non-identifying codes in public URLs. Keep a private spreadsheet mapping
individual codes to outreach recipients if needed.

## 5. Suggested Formspree organization
Use two separate forms so requests and reviews stay in separate inboxes and
exports:
- `Letters — Reader Copy Requests`
- `Letters — Reviews`

Enable Formspree spam protection. Export submissions periodically to CSV, or
connect Formspree to a spreadsheet/automation service if your plan supports the
integration you choose.

## 6. Recommended data policy
Reader request:
- Name required
- Career stage optional
- Discipline optional
- Email optional
- Explicit checkbox for one follow-up

Review:
- Review required
- Name, role, rating, and email optional
- Explicit permission before quoting comments

Do not treat the optional follow-up permission as newsletter consent.
