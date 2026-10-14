# Portfolio inquiry email setup

## Current status
The inquiry form, bilingual review screen, shared validation schema, same-origin JSON endpoint, payload limit, honeypot, and retry cooldown are implemented. Actual sending is **not configured or tested**. The endpoint returns HTTP 503 with `email_not_configured`; the form never displays success and retains the entered details.

No email domain is configured. Lovable Emails requires a real domain owned by the portfolio owner. No domain, sender, or private credential has been invented. There is no database, authentication, email queue, or marketing-email functionality.

## Required completion after domain setup
1. Set up and verify an owned email sender domain in Lovable’s email setup.
2. Scaffold the managed transactional email templates and send helper. Preserve the generated `SENDER_DOMAIN` and `FROM_DOMAIN`.
3. Register a fixed `portfolio-inquiry` React Email template with subject **New Portfolio Project Inquiry — Baraa**. Render name, email, selected service, title, description, optional timeline/budget, and a server-generated UTC submission timestamp. React text props must escape all visitor content.
4. Wire the validated `/api/inquiry` handler to `sendTemplateEmail` using the fixed recipient **abuwatfabaraa@gmail.com**, fixed template name, and idempotency key `portfolio-inquiry-${submissionId}`. Never accept a recipient, sender, subject, or template from the browser.
5. Return `sent: true` only after the helper confirms provider acceptance. Handle suppression and provider failures without success, and preserve the inquiry in the UI. Honor provider retry-after instructions.
6. Test a real confirmed inquiry through the UI and check email delivery logs before claiming sending works.

`LOVABLE_API_KEY` is required server-side by the generated managed send helper. No separate Resend API key is required for this chosen approach. The actual sender address and domain remain unknown until the owner completes setup. Client cooldown is a usability/spam deterrent, not a distributed server rate limiter; the managed provider supplies delivery rate limits and idempotency.

## Additional content
The three public QA spreadsheets were accessible for evidence review. No unverified aggregate analytics are shown. AI Creative Studio awaits actual images/videos and descriptions. The task-delay project uses a clearly labeled workflow illustration; no production deployment or successful end-to-end testing is claimed.