# Measurement without tracking pixels

The sites promise no analytics. Keep that promise. Measure with the tools that already exist:

- GitHub repo traffic, clones and referrers (owner-only Insights).
- FormSubmit emails: the form includes `source`, `page` and `date` fields.
- Replies in the inbox.
- A plain notebook or spreadsheet you update every Friday.
- Ask new contacts: "How did you find this?" One question, no tracking.

## Weekly scorecard

Copy this into a table or a Markdown file. One row per week.

| Week | Artifacts shipped | Personalized sends | Replies | Audits completed | Calls | Paid conversations | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 |  |  |  |  |  |  |  |
| 2 |  |  |  |  |  |  |  |
| 3 |  |  |  |  |  |  |  |
| 4 |  |  |  |  |  |  |  |

## Definitions

| Metric | Definition | Source |
| --- | --- | --- |
| Artifact | A public page, report, check, template, post or release that did not exist last week. | URL |
| Personalized send | One email written for one recipient with a verified observation. | Sent folder |
| Reply | A human response that is not an auto-reply. | Inbox |
| Audit completed | A real page scanned, reviewed by a human, and the report delivered. | Report URL + email |
| Call | A real conversation, not a calendar hold. | Notes |
| Paid conversation | A discussion with a scope, budget or timeline. Not a "maybe". | Notes |
| Paid pilot | Written scope, price, start date and deliverable. | Signed scope |

## Rates worth watching

- **Reply rate** = replies ÷ personalized sends.
- **Audit conversion** = audits completed ÷ replies.
- **Paid conversion** = paid pilots ÷ audits completed.
- **Artifact rate** = artifacts shipped per week.

Do not compare these to "industry benchmarks" you cannot source. Compare them to your own previous four weeks.

## Signals that are not success

- Impressions without a click.
- Stars without a user.
- A like from someone who will never reply.
- A "we should collaborate" email with no artifact.
- A launch-day spike with no second-week retention.

Track stars and clones if they are useful, but label them **distribution signals**, not revenue or product-market fit.

## Where to put the numbers

- `GOALS.md`: the 90-day targets and current values.
- A private weekly note: the raw sends, replies and links. Do not publish anyone's name without permission.
- Public recaps: aggregate only, with dates. "10 audits completed, 3 replies, 1 paid pilot" is fine if true. "Hundreds of happy users" is not.

## Privacy

- Do not add Google Analytics, Plausible, Umami, pixels or session replay to a page that says "no analytics".
- Do not put email addresses in a public repo or a screenshot.
- If you publish a teardown, use a public URL and public information only. No private dashboard screenshots.
- Delete contact messages when they are no longer needed. See the privacy pages for the exact promise.

## Day-0 GitHub traffic baseline (14-day ending 26 Oct 2026)

Pulled from the GitHub traffic API (owner-only data, real numbers). This is a baseline, not a trend.

| Repo | Views (uniques) | Clones (uniques) |
| --- | --- | --- |
| launchgrade | 11 (4) | 402 (108) |
| repograde | 0 (0) | 82 (30) |
| fastpress-start | 0 (0) | 34 (22) |
| youlauncher | 1 (1) | 75 (43) |
| hire-me | 0 (0) | 63 (31) |
| outreach | 0 (0) | 74 (42) |
| .github | 0 (0) | 120 (62) |
| agency | 0 (0) | 0 (0) |
| placement | 0 (0) | 0 (0) |
| skills | 0 (0) | 0 (0) |

How to read this honestly:

- The absolute numbers are tiny. Treat them as plumbing, not interest.
- The traffic API cannot separate our own automation (CI clones on every push, our own audit fetches) from other people. A 402-clone count on launchgrade in two weeks almost certainly includes many of our own CI runs. Do not quote "402 clones" as traction.
- The agency, placement and skills repos shipped on 26 Oct, so their zeros are just age.
- What would actually matter: a rising view count on days we did not ship anything, or clones that keep growing for two weeks without pushes. Watch for that, not the raw totals.
- Re-pull this same table weekly (Free, owner-only Insights). Add one row per week below; keep old rows for comparison.

## Monthly review

1. Which channel produced the most **replies**, not the most impressions?

2. Which artifact is still getting links or replies a week later?
3. Which offer made people ask "how much?" That is a buying signal.
4. Which task felt busy but produced no artifact or conversation? Stop it.
5. Is every public number still true? If not, fix it today.
